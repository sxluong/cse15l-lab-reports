<h1> The command `less` </h1>

Brief Introduction : The `less` command allows one to view the contents of a specific file one screen at a time. It essentially takes you to another tab/screen in the bash terminal where you can navigate the contents using your arrows and mouse. It also allows you to search for certain patterns using `/` followed by whatever you're searching for. And to exit the screen you can just enter `q` <Enter>. `less` has many more different command options to seamlessly view the contents of a file.  

<h2>I am using `less -E`</h2>

input: `less -E Paris-WhatToDo.txt`

output/interation: <down><down><down> until I reach the end of the text file -> *exit*
  
Comments/Analysis: Though I am unable to show the command function, I have described it above. This is useful for a situation in which you scroll through many text files and don't want to constantly type `q` to exit the file when you reach the end of the pages. This is more so a convenience than usefulness.

  
input: `less -E vallarta-History.txt`
  
output/interation: <down><down><down> until I reach the end of the text file -> *exit*
  
Comments/Analysis: It was essentially the same as the previous command however the scrolling took perhaps a little shorter.
  
<h2> I am using `less -f`</h2>
  
input: `less -f berlitz2`
  
output: 
  
<img width="693" alt="image" src="https://user-images.githubusercontent.com/122576207/224836268-259efbe8-6a65-426d-88a3-49932ea80ee0.png">

Comments/Analysis: For context: "berlitz2" is a directory, not a file type. Knowing the functionality of `less` we know that it won't work on directories. However, the inclusion of the option `-f`, it essentially forces an opening with non-regular files (directory). We were able to "open" the directory but it displayed an error.

input: `less -f berlitz1`

output:
<img width="1413" alt="image" src="https://user-images.githubusercontent.com/122576207/224838181-97ac967b-2357-4b29-bbb5-c09c8957d0f7.png">
  
Comments/Analysis: As the command above, it brought me to another screen and displayed an error.

  
  <h2> I am using `less -N` </h2>
  
  input : `less -N HistoryMadrid.txt`
  
  output: 
  
  <img width="820" alt="image" src="https://user-images.githubusercontent.com/122576207/224841521-86d5352d-4ffc-41e8-a26e-ac70480a4e2a.png">

Comments/Analysis: The addition of "-N" simply displayed the line numbers on the side of each line. This is especially useful for keeping track of of what line you're currently reading in bash. Considering some text files are so vast and long, line numbers are useful.
  
  input : `less -N HistoryLasVegas.txt`
  
  
  output: 
  
  <img width="749" alt="image" src="https://user-images.githubusercontent.com/122576207/224860118-7aa0b7fc-d6ab-46b5-99ae-c87c5abe7f17.png">

  
  Comments/Analysis: Wow! More line numbers.
  
  
  
  <h2> I am using `less -p` </h2>
  
  
  input: `less -p the HistoryMadrid.txt`
  
  output:
  <img width="1246" alt="image" src="https://user-images.githubusercontent.com/122576207/224862849-a72fe8a7-22c3-48f3-9ebd-3340eb477725.png">

  Analysis/Comments: This command brought me to the first occurence of "on" which was at Bronze. However, this command doesn't get the whole word but also accounts for substrings so that might be an issue. This would be useful for finding the place of the first word that you were looking for on a big text file. Say you recalled the first occurence of something being so interesting and it included that specific word-> this would be useful. 
  
  input: `less -p water HandRHawaii.txt`
  
  output: <img width="1121" alt="image" src="https://user-images.githubusercontent.com/122576207/224863225-98aa5c79-ea2b-4b7f-a7ee-0c49d542d421.png">
  
  Analysis/Comments: I chose to search for the first occurence of water because it is hawaii. As it is suppose to, it started exactly at the first occurence of "water".
  
  
  
  <h2>Source: </h2>
  
  [Phoniex_nap](https://phoenixnap.com/kb/less-command-in-linux)
  
  

  
  
  
  
  
  
  
