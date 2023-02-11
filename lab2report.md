<h1>Part 1: </h1>
My code:

```
import java.io.IOException;
import java.net.URI;
import java.io.IOException;
import java.net.URI;

class Handler implements URLHandler {
    // The one bit of state on the server: a number that will be manipulated by
    // various requests.
    String[] wordsArray = new String[20];
    int count = 0;

    // sized 20 just in case
    @Override
    public String handleRequest(URI url) {
        if (url.getPath().equals("/")) {
      
            String to_return = "";
            for (int i = 0; i < 20; i++) {
                if (wordsArray[i] != null) {
                    to_return += wordsArray[i] + "\n";
                }
            }
            return to_return;
        } else {
            System.out.println("Path: " + url.getPath());
            if (url.getPath().contains("/add-message")) {
                String[] parameters = url.getQuery().split("=");
                wordsArray[count] = parameters[1];
                count += 1;
                return "added";
            }
            return "404 Not Found!";
        }
    }
}
```

```
class StringServer {
    public static void main(String[] args) throws IOException {
        if (args.length == 0) {
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }
        int port = Integer.parseInt(args[0]);
        Server.start(port, new Handler());
    }
}
```


Initially my website is a blank page which should be evident given that I have not inserted any strings into the website.
![image](https://user-images.githubusercontent.com/122576207/215294855-99dace63-db29-4331-9406-5d654fbdfcd0.png)
Next, I will add a message. 
![image](https://user-images.githubusercontent.com/122576207/215294940-9c663ac6-1781-475d-aa2d-74876eafdce7.png)

The "added" message indicates that I have added a string. The string being added is "Hello" as shown in the url after the "=" sign. The url goes through
my handlerequest function. It gets parsed by multiple if statements. In this case of adding the message, since the link "http://localhost:2024/add-message?s=Hello"
contains the key word "add-message", the method parses the query inserting it into an array. `String[] parameters = url.getQuery().split("=");` is the statement that does so.
The first element in the array contains the s and the second contains the string itself (positioned at 1 in the array). Using this knowledge, I can add the string into the global array. Then I will add one to the global variable 'count' which keeps the position of each incoming string that is being added.
I created outside the scope of the function to store all the strings that I have added.
Nevertheless, as I go back to the page shows "Hello" imprinted when I go back to the original URL without a query. 
![image](https://user-images.githubusercontent.com/122576207/215295275-265fa590-9fdd-4205-ab2e-9a157f5cc264.png)

The reason it prints out is because, in my method, if the path is simply "/", this indicates to my function to go through all the added strings and return(or print) them. I also ensure to keep the order and skip a line with `\n`.

I will add another string once more.
![image](https://user-images.githubusercontent.com/122576207/215295347-fd8c45d2-8b46-4db1-b418-d05ca941f719.png)
![image](https://user-images.githubusercontent.com/122576207/215295356-bfe9add1-d854-4478-81bb-955b0d76bc5e.png)

Vuola!

<h1>Part 2:</h1>

Failure inducing input:
```
public void testReversednew() {
    int[] input1 = { 1, 2, 3, 4 };
    int[] input2 = { 1 };
    int[] input3 = { 1, 2, 3 };

    assertArrayEquals(new int[] { 4, 3, 2, 1 }, ArrayExamples.reversed(input1));
    assertArrayEquals(new int[] { 1 }, ArrayExamples.reversed(input2));
    assertArrayEquals(new int[] { 3, 2, 1 }, ArrayExamples.reversed(input3));
  }
  ```
  All the tests fail because the code does not even return the correct array. It adds null values to the array we were passed as a reference in the argument of the function.
Associated code:
```
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }
 ```

An input that doesn't induce a failure:
```
  public void testReversednew() {
    int[] input1 = {};
   

    assertArrayEquals(new int[] {}, ArrayExamples.reversed(input1));
  }
```
Associated code: ^ same and before
This only passes because it is an empty array. An empty array will pass in teh function and an empty array will spit out because it doesn't even go through the loop that is suppose to instantiate the new reveresed values.
The symptom : 
<img width="1013" alt="image" src="https://user-images.githubusercontent.com/122576207/215297345-e72ce9cb-e228-4360-859b-6f1a678220e9.png">
There were many differences as indicated by the "38 more" errors statement.


Fixing code->
Before:
```
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }
  ```
  After:
  ```
  static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for (int i = 0; i < arr.length; i++) {
    newArray[i] = arr[arr.length - i - 1];
    }
    return newArray;
  }
  ```
  I tweaked the code just a little. The logic with the for loop was correct as you want to add to an array reversing through the passed in array. I just tweaked the return statement to return the new array that we instantiate and add to. The new array is also added.
  
  <h1>Part 3:</h1>
  I never really knew how to debug using Jnit tests. Neither did I know I change the localhost id other than 8000. I am glad to have learned this as I will continue to apply this knowledge in my future coding adventures.
