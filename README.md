<section id="header">
  <div align="center">

  # How to Use the Command Line Vim Text Editor
  **Written by [Amar Panjwani](https://www.linkedin.com/in/amarpan/)** <br> Technical Writer

  <div id="socialbuttons" align="center">

  [![Portfolio Badge](https://img.shields.io/badge/-amarpan.github.io-magenta?style=flat&logo=)](https://amarpan.github.io)
  <br>
  [![LinkedIn Badge](https://img.shields.io/badge/-amarpan-blue?style=flat&logo=Linkedin&logoColor=black)](https://www.linkedin.com/in/amarpan/)
  <br>
  ![Stars](https://img.shields.io/github/stars/amarpan/how-to-use-the-vim-text-editor?style=social)
  ![](https://visitor-badge.laobi.icu/badge?page_id=amarpan.how-to-use-the-vim-text-editor)
  ![Forks](https://img.shields.io/github/forks/amarpan/how-to-use-the-vim-text-editor?style=social)
  <br>
  ![Version](https://img.shields.io/badge/version-1.0-gold)

  ### If you find this tutorial helpful, please consider giving it a :star:

</div>
</div>

This tutorial describes how to open, edit, and save a plain text file using the Vim text editor in a command line interface (CLI).

</section>

## Why Use Vim
Vim offers a rich selection of keyboard-based shortcuts that make editing, inserting, deleting, and searching for specific use-cases speedy and efficient.

## Background Information
Derived from the Vi text editor, Vim stands for "Vi IMproved". 

Notable upgrades include:

1. Multi-Level Undo
2. Multiple Windows Mode
3. Syntax Highlighting

## Modes - Input and Command
Vim has two main modes of operation: insert and command.
### 1. Insert Mode
In insert mode, anything typed by the user is output to the opened file. However, the user can't give shortcut commands to alter text or return to the command line. 
 
For example, a user would use insert mode to type up a paragraph. However, a user would and could not use insert mode to give a command like `dl` to delete the line the cursor is on. 

Press `i` to enter insert mode.
 
Press `ESC` to exit insert mode and enter command mode.

**Note:** Insert mode can be verified if an "-- INSERT --" message is shown in the bottom-left hand corner of the screen.

### 2. Command Mode (Default)
In command mode, anything typed by the user is processed as shortcut commands to alter the contents of the file in some shape or form. While in command mode, Vim does not input plain text into the file itself.

For example, a user would use command mode to input a command like `dl` to delete the line the cursor is on. A user would not use command mode to type up a paragraph.

## How to Use - The Basics
1. Create a new file and open it in Vim.
    - a. Type `vim note.txt`

<img src="./screenshots/empty-vim-file.png" width="">

2. Enter input mode.
    - a. Press the `i` key.

<img src="./screenshots/insert-mode.png" width="">

<br>  

**Note**: The -- INSERT -- status message in the bottom-left corner signals that you can now insert text.

3. Write in some text.
    - a. Type in a message (Example: I love Linux.)

<img src="./screenshots/enter-text.png" width="450">

4. Exit insert mode.
    - a. Press the `ESC` key.
    
<img src="./screenshots/exit-insert-mode.png" width="450">  <br> 
    
**Note**: The -- INSERT -- message has now dissapeared.

5. Save the file (write it to disk).
    - a. Type `:w` + `ENTER` 
    
<img src="./screenshots/write-to-file.png" width="450">

<img src="./screenshots/file-written.png" width="450">  

<br> 

6. Exit (quit) Vim and return back to the command line. 
    - a. Type `:q` + `ENTER` 
    
<img src="./screenshots/quit-vim.png" width="450">  
    
<br>

**Note:** Alternatively, typing `:wq` + `ENTER` writes the file and quits to the command line is one step. 

## Advanced Command Shortcuts

The best thing about Vim are its shortcuts.
 
**Warning:** Vim is case-sensitive, meaning it interprets the same letter as two different commands based on upper or lower casing. 

### Navigation
While navigation using the directional cursor keys or mouse is supported, it is recommended to use the following letter keys for quicker access to keyboard-based shortcuts:

|      Event      |    Command    
|:---------------:|:---------------:
| Up              |`k`        
| Left            |`h`
| Down            |`j` 
| Right           |`l`
| Scroll up half a window   |`CTRL-U`
| Scroll down half a window | `CTRL-D`

### Deleting Text
Move the cursor over the desired text and use the following:<br>
**Note**: The following commands can also be prepended with a number for a multiplied effect.
|      Event      |    Command    
|:---------------:|:--------------:
|Delete character |`x`
|Delete word      |`dw`
|Delete line      |`dd`
|Undo last operation |`u` 
|Redo last operation  |`CTRL-R` <br>or<br> `:redo` + `ENTER`

### Entering Text
|      Event      |    Command    
|:---------------:|:--------------:
|Insert blank line above and enter insert mode        |`O`
|Insert blank line below cursor and enter insert mode |`o`

### Useful Commands
|      Event      |    Command    
|:---------------:|:--------------:
Force quit without saving | `:q!` + `ENTER` 
Display line numbers      | `:set number` + `ENTER` 
Turn off line numbers     | `:set nonumber` + `ENTER` 
View help guides          | `:help`   


### Moving the Cursor by Criteria
Move the cursor to the...
|      Event      |    Command    
|:---------------:|:--------------:
next occurrence of a specific character on the current line | `f` + `character`  
previous occurrence of a specific character on the current line | `F` + `character` 
beginning of the next word | `w`
beginning of the previous word | `b`
end of the next word | `e` 
beginning of the next sentence | `)`
beginning of the current sentence | `)`
beginning of the next paragraph | `}`
beginning of the current paragraph | `{`
top line of the screen | `H`
middle line of the screen | `M`
bottom line of the screen | `L` 

## Searching for a String
|      Event      |    Command    
|:----------------:|:--------------:
Find the next occurrence of a string | `/` + `string` + `ENTER`  
Find the previous occurrence of a string | `?` + `string` + `ENTER` 
Repeat the last search | `n`  
Repeat the last search in the opposite direction | `N` 

## More Information

You may wish to consult the following resources for additional information on this topic. While these are provided in the hope that they will be useful, please note that we cannot vouch for the accuracy or timeliness of externally hosted materials.

- [Official Vim Documentation](https://www.vim.org/docs.php)

<div align="center">

### ***If you found this tutorial helpful, please consider giving it a :star:
   
Copyright :copyright: 2021-2022

## More Tutorials from Amar Panjwani

  [How to Write a Coding Bootcamp README](https://github.com/amarpan/how-to-write-a-README)

 [How to Change Z Shell Themes](https://github.com/amarpan/how-to-install-and-configure-zshell)

 [How to Create a GitHub Profile](https://github.com/amarpan/how-to-create-a-github-profile)














