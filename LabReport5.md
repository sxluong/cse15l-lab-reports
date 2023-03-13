<h1> The command `less` </h1>

Brief Introduction : The `less` command allows one to view the contents of a specific file one screen at a time. It essentially takes you to another tab/screen in the bash terminal where you can navigate the contents using your arrows and mouse. It also allows you to search for certain patterns using `/` followed by whatever you're searching for. And to exit the screen you can just enter `q` <Enter>. `less` has many more different command options to seamlessly view the contents of a file.  

<h2>I am using `less -E`</h2>

input: `less -E Paris-WhatToDo.txt`

output/interation: <down><down><down> until I reach the end of the text file -> *exit*
  
Though I am unable to show the command function, I have described it above. This is useful for a situation in which you scroll through many text files and don't want to constantly type `q` to exit the file when you reach the end of the pages. This is more so a convenience than usefulness.

  
input: `less -E vallarta-History.txt`
  
output/interation: <down><down><down> until I reach the end of the text file -> *exit*
  
It was essentially the same as the previous command however the scrolling took perhaps a little shorter.
  
<h2> I am using `less -f`</h2>
  
input: `less -f berlitz2`
  
output: 
  
<img width="693" alt="image" src="https://user-images.githubusercontent.com/122576207/224836268-259efbe8-6a65-426d-88a3-49932ea80ee0.png">

For context: "berlitz2" is a directory, not a file type. Knowing the functionality of `less` we know that it won't work on directories. However, the inclusion of the option `-f`, it essentially forces an opening with non-regular files (directory). We were able to "open" the directory but it displayed an error.

input: `less -f berlitz1`

output:
<img width="1413" alt="image" src="https://user-images.githubusercontent.com/122576207/224838181-97ac967b-2357-4b29-bbb5-c09c8957d0f7.png">
  
As the command above, it brought me to another screen and displayed an error.

  
  <h2> I am using `less -N` </h2>
  
  input : `less -N HistoryMadrid.txt`
  
  output: 
  
  <img width="820" alt="image" src="https://user-images.githubusercontent.com/122576207/224841521-86d5352d-4ffc-41e8-a26e-ac70480a4e2a.png">


