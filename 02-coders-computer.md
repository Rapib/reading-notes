# 02 - The Coder's Computer

It is necessary to set up the computer before coding starts. 

Pick a text editor can do the following: 
* code completion 
* syntax highlighting 
* extensions 
* theme

As it will save developer time and help speed up the process. In addition, it will help point out the mistakes that developer made. Basic editor doesn't do any of the above, eg Word, notepad

Belows are the common Linus commands that we will use. 

## Linux command:
> Command + (argument): 

> file

what type of file a file or directory 

> pwd 


list location, path 



> ls [options] [location] 

option examples:

–l < long list 

-a < list the contents, including hidden files (start with a .)


/etc < not to list our current directory but instead to list that directories contents 
Show what it inside a directory 

> List all files in folder Hi

```
cd ~/Hi
ls -la

OR

ls -la ~/hi

OR

cd ~

cd hi

ls -la
```
> cd .. 

Go up one level (… = 2 level, …. = 3 level) 
*just cd < home directory 
 

> cd FOLDER-NAME OR 'Folder that has space' use (') quote OR Folder\ Name use (\ ) backslash does is escape (or nullify) the special meaning of the next character

Change folder/directory 

*if put a letter, it will list all folders start with that letter 

*use tab to prefill folder name (>When you start typing a path (anywhere on the command line, you're not just limited to certain commands) you may hit the Tab key on your keyboard at any time which will invoke an auto complete action. If nothing happens then that means there are several possibilities. If you hit Tab again it will show you those possibilities. You may then continue typing and hit Tab again and it will again try to auto complete for you. 

It's kinda hard to demonstrate here so it's probably best if you try it yourself. If you start typing cd /hTab/<beginning of your username>Tab you'll get a feel for how it works.) [^1]

  

*cd pro/course/hi  (can be more specific) 

 


> tree 

List all files inside folder as a tree format 

 

> clear 

Clear the output of the cmd line (get rid of text only, doesn’t change anyting) 

 

> Arrow up, down 

Go back to used command 

 
 

> mkdir FOLDER-NAME 

Create folder 

 

> touch FILENAME.EXTENSION 

Create file 

***Paths***
 
 *Relative path*
 
A file or directory location relative to where we currently are in the file system.
 
*Absolute path*
 
A file or directory location in relation to the root of the file system.
 
/ - root directory
 
~ (tilde) - This is a shortcut for your home directory. eg, if your home directory is /home/ryan then you could refer to the directory Documents with the path /home/ryan/Documents or ~/Documents
                      
. (dot) - This is a reference to your current directory. eg in the example above we referred to Documents on line 4 with a relative path. It could also be written as ./Documents (Normally this extra bit is not required but in later sections we will see where it comes in handy).
                      
.. (dotdot)- This is a reference to the parent directory. You can use this several times in a path to keep going up the hierarchy. eg if you were in the path /home/ryan you could run the command ls ../../ and this would do a listing of the root directory. [^2]
 
 > ***Linux is Case Sensitive***

^C 

Stop what is going on  

 > Markdown .md file always end with 1 empty line (no 2 lines) 
  
  ## Things I want to know more about
  
  More linux commands
  

[^1]: https://ryanstutorials.net/linuxtutorial/navigation.php 

[^2]: https://ryanstutorials.net/linuxtutorial/navigation.php 
  
