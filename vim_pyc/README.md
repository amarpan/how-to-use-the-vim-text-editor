<!-- 
***Rememember this isn't your first rodeo - readme-writing-tutorial was your first rodeo and that was super successful!
1. Write it according to PYC Style Guidelines (also gives you sellability to other clients as well as your own branding revenue on panyoucan.org or gatips.com blog)
2. Change specs to adhere to Linode Style Guidelines
--> 



<div align="center">

# Introduction to the Vim Text Editor
<h3 align="center" id="author">
   Written by <a href="https://www.linkedin.com/in/profpan396/">Professor Pan, M.Ed.</a> 
   <div align="center">
<a href="https://profpan396.github.io/portfolio" target="_blank">
        <img
          src="https://img.shields.io/badge/-profpan396.github.io/portfolio-magenta?style=flat&logo=Blackberry&logoColor=black">
      </a>
<a href="mailto:profpan396@gmail.com" target="_blank">
    <img src="https://img.shields.io/badge/-profpan396@gmail.com-aqua?style=flat&logo=Gmail&logoColor=black">
 </a>
 <a href="https://www.github.com/profpan396/" target="_blank">
        <img
          src="https://img.shields.io/badge/-github.com/profpan396-junglegreen?style=flat&logo=GitHub&logoColor=black">
      </a>

 <a href="https://www.linkedin.com/in/profpan396/" target="_blank">
      <img src="https://img.shields.io/badge/-linkedin.com/in/profpan396-blue?style=flat&logo=Linkedin&logoColor=black">
 </a> 
  <a href="https://medium.com/@profpan396">
    <img src="https://img.shields.io/badge/-medium.com/@profpan396-pink?style=flat&logo=medium&logoColor=black">
 </a>
 <a href="https://twitter.com/profpan396" target="_blank">
      <img src="https://img.shields.io/badge/-twitter.com/in/profpan396-skyblue?style=flat&logo=Twitter&logoColor=black">
 </a>


 </h3>

![](https://visitor-badge.glitch.me/badge?page_id=profpan396.vim_pyc)
</div>

## What Vim Is and Isn't 
Vim is a text editor used for editing plain text as well as code-based programs. It does not, however, format text or offer the same advanced features as word processing software suites. 

## Why Use Vim
Vim offers a rich selection of keyboard-based shortcuts that make editing, inserting, deleting, and searching for specific use-cases speedy and efficient.

## Background Information
Vim is derived from the original Vi text editor, and stands for "Vi IMproved". 
Notable differences between Vi and Vim are:

1. Multi-level Undo
2. Multiple Windows Mode
3. Syntax Highlighting

## Modes - Input, Command, and Last-Line
Vim has three main modes of operation: insert, command, and last-line.
### 1. Insert Mode
In insert mode, anything typed by the user is output to the opened file. However, the user can not give shortcut commands to alter text or return to the command line. 
 
For example, a user would use insert mode to type up a paragraph. However, a user would and could not use insert mode to give a command like ```dl``` to delete the line the cursor is on. 

To enter insert mode, press ```i```.
 
To exit insert mode and enter command mode, press ```ESC```.

***Note: Insert mode can be verified if an "-- INSERT --" message is shown in the bottom-left hand corner of the screen.



### 2. Command Mode (Default)
In command mode, anything typed by the user is processed as shortcut commands to alter the contents of the file in some shape or form. While in command mode, vim does not input plain text into the file itself.

For example, a user would use command mode to input a command like ```dl``` to delete the line the cursor is on. A user would not use command mode to type up a paragraph.
 
### 3. Last-Line Mode
When a user is in command mode and prepends a keyboard shortcut with a ```:```, vim enters last-line mode - meaning the cursor is now moved to the bottom line of the screen. An important distinction between command mode and last line mode is that all last line commands must be terminated with a ```ENTER```.

For example, a user would save the contents of a file using a commmand like ```:w``` + ```ENTER```. 

## How to Use - The Basics
| Step | Instructions | Screenshot  |
|------------ | ----- | ------------|
| 1. Create a new file and open it in Vim.  | Run ```vim note.txt``` | <img src="./screenshots/empty_vim_file.png" width="">  Note: The tildes (~) represent empty lines and dissapear as lines of text are added.  
| 2. Enter input mode. | Press the ```i``` key. | <img src="./screenshots/insert_mode.png" width="">  The -- INSERT -- status message in the bottom-left corner signals to us that we can now insert text.
| 3. Write in some text. | Type in a message  Example: I love Linux! | <img src="./screenshots/enter_text.png" width="450">  
| 4. Exit insert mode. | Press the ```ESC``` key.   | <img src="./screenshots/exit_insert_mode.png" width="450">  Note: The -- INSERT -- message has now dissapeared.
| 5. Write the file to the disk (save it). | Type ```:w``` + ```ENTER```   | <img src="./screenshots/write_to_file.png" width="450">  <img src="./screenshots/file_written.png" width="450">  The "w" in :w stands for "write", and we can see the file is now officially written to the disk, meaning saved. 
| 6. Quit vim and return back to the command line. | Type ```:q``` + ```ENTER```  | <img src="./screenshots/quit_vim.png" width="450">  <img src="./screenshots/back_to_command_line.png" width="450">  Alternatively, ```:wq``` + ```ENTER``` or ```ZZ``` writes the file and quits to the command line is one step. 

## How to Use - Advanced Command Shortcuts

The best thing about vim are its shortcuts.
 
Warning: vim is case-sensitive, meaning it interprets the same letter as two different commands based on upper or lower casing. 

### Navigation
While navigation using the directional cursor keys or mouse is supported, it is recommended to use the following letter keys for quicker access to keyboard-based shortcuts:

|      Event      |    Command    
|-----------------|---------------
| Up              |```k```        
| Left            |```h```
| Down            |```j``` 
| Right           |```l```
| Scroll up half a window   |```CTRL-U```
| Scroll down half a window | ```CTRL-D```

### Deleting Text
Move the cursor over the desired text and use the following: 
|      Event      |    Command    
|-----------------|---------------
|Delete character | ```x```
|Delete word      |```dw```
|Delete line      |```dd```
|Undo last operation | ```u``` 
|Redo last operation  |```CTRL-R``` or ```:redo``` + ```ENTER```

### Entering Text
|      Event      |    Command    
|-----------------|---------------
|Insert blank line above and enter insert mode        | ```O```
|Insert blank line below cursor and enter insert mode |```o```

### Useful Commands
|      Event      |    Command    
|-----------------|---------------
Force quit without saving | ```:q!``` + ```ENTER``` 
Display line numbers      | ```:set number``` + ```ENTER``` 
Turn off line numbers     | ```:set nonumber``` + ```ENTER``` 
View help guides          | ```:help```   


### Moving the Cursor by Criteria
Move to the cursor to the...
|      Event      |    Command    
|-----------------|---------------
next occurence of a specific character on the current line | ```f``` + ```character```  
previous occurence of a specific character on the current line | ```F``` + ```character```  
beginning of the next word | ```w``` 
beginning of the previous word | ```b``` 
end of the next word | ```e``` 
beginning of the next sentence | ```)``` 
beginning of the current sentence | ```)``` 
beginning of the next paragraph | ```}``` 
beginning of the current paragraph | ```{``` 
top line of the screen | ```H``` 
middle line of the screen | ```M``` 
bottom line of the screen | ```L``` 

## Searching for a String
|      Event      |    Command    
|-----------------|---------------
Find the next occurence of a string | ```/``` + ```string``` + ```ENTER```  
Find the previous occurence of a string | ```?``` + ```string``` + ```ENTER``` 
Repeat the last search | ```n```  
Repeat the last search in the opposite direction | ```N``` 















