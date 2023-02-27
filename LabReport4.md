<h2>Step 4:</h2>

<img width="635" alt="image" src="https://user-images.githubusercontent.com/122576207/221687611-2007881f-80ca-4091-8811-ff8d19d08ed5.png">

As per usual, I ssh into my remote server using the command `ssh cs15lwi23aiv@ieng6.ucsd.edu`. I swiftly was able to do this using the shortcut command `<ctrl-R>` and inserting `s`, which got me to the full ssh command. I then typed in my credentials to the request and successfully got in.

<h2>Step 5: </h2>

<img width="662" alt="image" src="https://user-images.githubusercontent.com/122576207/221688562-612c30e7-d84a-43ef-9c38-c38c7a1127aa.png">

I forked the repository on the github website. Now that I have it in my repository, I then typed `git clone https://github.com/sxluong/lab7.git` and clicked `<enter>` which led to the succesful clonage of the repository to my remote server.


<h2>Step 6: </h2>

<img width="995" alt="image" src="https://user-images.githubusercontent.com/122576207/221688239-296fa996-bab2-4805-b0fc-89a4be2945f9.png">

I typed in the command `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` using `<ctrl-R>` and the key `javac` to search for the full compilation command. Furthermore, I followed with the command `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` which I also found using `<ctrl-R>` and the key `j` as it was the first to pop. After running the test, I noticed that I needed to fix the code after the tests failed.

Note: I clicked `<enter>` on all the commands

<h2>Step 7:</h2>

<img width="409" alt="image" src="https://user-images.githubusercontent.com/122576207/221689737-0bac3032-c7fc-440a-8916-d9209822597e.png">

<img width="554" alt="image" src="https://user-images.githubusercontent.com/122576207/221690736-5a28d979-bc96-429c-b1b3-800049469032.png">

To dissect and solve the problem, I use the vim editor to change and save the code. I typed `vim ListExamples.java` using the shortcut `<ctrl-R>` and using the key `vim`. I had to traverse through the code; my following steps were `<down>...` to line 43 and `<right>...` to the position of the 1 on index1. I needed to edit it. I did so by clicking `<i>` which turns the editor on. I change the 'index1' to 'index2' which completes the logic. I then saved the edit by first exiting out of editor mode using `<ctrl-C>`. I then saved the changes using the command `:wq`, which saves the vim editor and then exits.

Note: I clicked `<enter>` on all the commands

<h2>Step 8:</h2>

<img width="1009" alt="image" src="https://user-images.githubusercontent.com/122576207/221691027-227f245a-71d1-4210-bec2-48829a64e368.png">

I typed in the command `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` using `<ctrl-R>` and the key `javac` to search for the full compilation command. Furthermore, I followed with the command `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` which I also found using `<ctrl-R>` and the key `j` as it was the first to pop. After running the test, I notice it now passes all the tests as expected!

Note: I clicked `<enter>` on all the commands

<h2>Step 9:</h2>

<img width="339" alt="image" src="https://user-images.githubusercontent.com/122576207/221691999-d744b514-0e44-4d05-af7e-5d982f1a2ae5.png">


<img width="541" alt="image" src="https://user-images.githubusercontent.com/122576207/221692047-57da784c-9952-42ed-a40f-2f35e5467231.png">

<img width="522" alt="image" src="https://user-images.githubusercontent.com/122576207/221696193-49afd7ee-c262-4483-b1d3-5a14e6975fe7.png">

Here I manually typed all the git commands. I added all the files that I made/edited to the staging area by doing `git add .`. I then committed the file changes by doing `git commit -m "first-commit`. Now that the history is intantiated, we can push the local repository to the online repository. I did this by doing `git push`. As you can see, it was a success!

Note: I clicked `<enter>` on all the commands
