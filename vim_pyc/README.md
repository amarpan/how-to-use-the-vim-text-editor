<!-- 
***Rememember this isn't your first rodeo - readme-writing-tutorial was your first rodeo and that was super successful!
1. Write it according to PYC Style Guidelines (also gives you sellability to other clients as well as your own branding revenue on panyoucan.org or gatips.com blog)
2. Change specs to adhere to Linode Style Guidelines
--> 



<div align="center">

# Introduction to the Vim Text Editor
<h3 align="center" id="author">
   Written by <a href="https://www.linkedin.com/in/profpan396/">Professor Pan, M.Ed.</a><br> 
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
Vim is an advanced text editor used for editing plain text and code-based programs. It does not, however, format text and offer the same features as word processing software suites. 

## Background Information
Vim is derived from the original Vi text editor, and stands for "Vi IMproved". 
Major differences between Vi and Vim are:

1. Multi-level Undo
2. Multiple Windows Mode
3. Syntax Highlighting

## Modes - Command and Input
Vim has two main modes of operation - Command and Insert Mode. 
### 1. Command Mode
In command mode, vim accepts all user input as shortcut commands to alter text in some shape or form. However, the user can not input plain text in the file itself.
### 2. Insert Mode
In insert mode, anything typed by the user is output to the opened file. However, the user cannot give shortcut commands to alter text or return to the command line. <br><br>
Press ```i``` to enter input mode.
If an -- INSERT -- message is displayed in the bottom-left hand corner, then vim is in insert mode.
Press ```ESC``` to exit insert mode and enter command mode.

<!-- ## How to Use - The Basics
Vim should come pre-installed with every Linux distribution, but just in case it is not, run the following command: 
```sudo ________ ``` -->

| Step | Instructions | Screenshot  |
|------------ | ----- | ------------|
| 1. Create a new file and open it in Vim.  | Run ```vim note.txt``` | <img src="./screenshots/empty_vim_file.png" width=""> <br> Note: The tildes (~) represent empty lines and dissapear as lines of text are added.  <br>
| 2. Enter input mode. | Press the ```i``` key. | <img src="./screenshots/insert_mode.png" width=""> <br> The -- INSERT -- status message in the bottom-left corner signals to us that we can now insert text. Before this, entering text did absolutely nothing.
| 3. Write in some text. | Type in a message <br> Example: I love Linux! | <img src="./screenshots/enter_text.png" width="450"> <br> 
| 4. Exit insert mode. | Press the ```ESC``` key.  <br> | <img src="./screenshots/exit_insert_mode.png" width="450"> <br> Note: The -- INSERT -- message has now dissapeared.
| 5. Write the file to the disk (save it). | Type ```:w``` + ```ENTER```  <br> | <img src="./screenshots/write_to_file.png" width="450"> <br> <img src="./screenshots/file_written.png" width="450"> <br> The "w" in :w stands for "write", and we can see the file is now officially written to the disk, meaning saved. 
| 6. Quit vim and return back to the command line. | Type ```:q``` + ```ENTER``` <br> | <img src="./screenshots/quit_vim.png" width="450"> <br> <img src="./screenshots/back_to_command_line.png" width="450"> <br> Alternatively, ```:wq``` + ```ENTER``` writes the file and quits to the command line is one go. 

## How to Use - Advanced Shortcuts

The best thing about vim are its shortcuts. 
Warning: vim is case-sensitive, meaning it interprets the same letter as two different commands based on casing. 

### Navigation
While navigation using the directional cursor keys is supported, it is recommended to use the following letter keys for quicker access to command line shortcuts:

Up - ```k``` <br>
Left - ```h``` <br>
Down - ```j``` <br>
Right - ```l``` <br>

Sroll up half a window - ```CTRL-U```
Sroll down half a window - ```CTRL-D```

### Deleting Text
Delete character cursor is on - ```x``` <br>
Delete word cursor is on - ```dw``` <br>
Delete line cursor is on - ```dd``` <br>
Undo last operation - ```u``` <br>
Redo last operation - ```CTRL-R``` or ```:redo```+ ```ENTER```

### Entering Text
Append (insert after cursor) - ```a```
Insert blank line above cursor and enter insert mode - ```O```
Insert blank line below cursor and enter insert mode - ```o```

### Useful Commands

Force quit without saving - ```:qa!``` + ```ENTER``` <br>
Display line numbers - ```:set number``` + ```ENTER```
Turn off line number display - ```set nonumber``` + ```ENTER```
View help guides - ```:help```
Close a help window - ```:q```
Split the screen with another empty file - ```CTRL-W``` + ```n```
Alternate which split screen uses the cursor - ```CTRL-W``` + ```w```













