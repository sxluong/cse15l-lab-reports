Initially you want to get ahold of your unique CSE15L account within this website: [Link](https://sdacs.ucsd.edu/~icc/index.php). After you have entered,
choose one of the two ways to login. As you get in, searching for the email associated to CSE 15L.
![image](https://user-images.githubusercontent.com/122576207/212774882-d3b2e78d-64c3-431f-8f1f-7df8ee0d1275.png)
![image](https://user-images.githubusercontent.com/122576207/212775004-c5c5e9c4-a540-4d05-9838-ca78932bfd34.png)

Notice the username^. In my case it is cs15lwi23aiv.

The next step requires you to install Visual Studio Code. If you do already have it preinstalled like I do, don't worry! However, it is easy to install as
all you are required to do is to visit [website](https://code.visualstudio.com) then download and install visual studios. The reason we need visual studios is to access a terminal where we can then "ssh" or connect to a remote server. Also, visual studios has git preinstalled.
![image](https://user-images.githubusercontent.com/122576207/212795682-619eb865-d73c-4a84-abd8-65f41618de4e.png)
<img width="1654" alt="image" src="https://user-images.githubusercontent.com/122576207/212795867-77e8def3-a989-4cb6-8d67-a31e568018b0.png">

Now, once that you have the IDE opened you, want to access the terminal by clicking 'view' and then 'terminal' which will be located on the access bar on top. In the command prompt you want to type exactly "ssh cs15lwi23zz@ieng6.ucsd.edu" but change the ending after 23 to be your unique username, the username we found at the beginning of the guide. 
Since it is obviously your first time sshing into a remote server, you will be presented with this:
![image](https://user-images.githubusercontent.com/122576207/212797614-9fac74d9-91a4-4eeb-abae-ac316d79e463.png)
Just say yes.
It will then ask for a password, which you will then enter your triton password. If it is denied, then simply reset it. If you need help refer to the [tutorial](https://docs.google.com/document/d/1hs7CyQeh-MdUfM9uv99i8tqfneos6Y8bDU0uhn1wqho/edit). 
It should look like this :
<img width="1568" alt="image" src="https://user-images.githubusercontent.com/122576207/212798193-4393e2fe-b126-41f0-b009-dc56cb7b0502.png">
<img width="1568" alt="image" src="https://user-images.githubusercontent.com/122576207/212798217-d4d026ec-52a3-4311-9041-3de5048cb1c7.png">

Now that you have access to the remote server, you can try some commands out.
![image](https://user-images.githubusercontent.com/122576207/212798369-d57fc77d-a580-428c-add3-ae9ebe5fa026.png)
From the example code I displayed, I noticed many things. The command ‘ls’ listed the files in the current home directory. I then “step” within the perl5 file by using ‘cd’ where can then see and configure all the contents within. The command ‘pwd’ tells me the “absolute path” and the current working directory I’m in. If you follow cd with ‘..’, it simply goes back to the root directory. Lastly, what I found amusing was how I could make another directory using ‘mkdir (name of directory)’ and it would pop up in my files. I made sure of the presence of the directory by doing ‘ls’.

Hooray! You have managed to connect to a remote server and write commands.



