### Live Mentors
#### Full Stack Software Development
##### &copy; All Rights Reserved by Live Mentors, 2024
---

[Back to Goals](./00_goals.md)

# Command Line Interface & Shells

Most of our learning of `Command Line Interface (CLI)` will be done through self-study and class exercises, and reinforced with projects 1-3.

## What is a File?

- A file is a list of bytes (data) and an identifier aka reference
- A file cannot contain other files
- If you create a new file with different identifiers but the same bytes, it is a copy of the file.
- If you just change the identifier, you have moved the file.
- If you keep the identifier but change the bytes, the file has been changed aka mutated

- File extension helps determine which program on your computer the file is associated with.
  - Ex: `"homework.docx"` is associated with Microsoft Word
- File extensions and file formats are **NOT** the same
- File extension is just the characters that appear after the period while the file format speaks to the way in which the data in the file is organized.

## What is a Folder?

- A Folder can also be called a `directory`
- A way to store files in groups and put them under a common heading. Think of it similar to putting paper files into paper folders.
- Folders hold one or more files, and a folder can be empty until it is filled.
- Folders can also contain other folders, and many levels of folders within folders known as "subfolders" or "subdirectories".
- `Parent` and `child` are terms often used to describe the relationship between directory and a subdirectory.

## Folder Hierarchy

A folder hierarchy is an organizational structure of one or more folders

<img src="./assets/com1.png" width="80%" style="border: 1px solid white">

Here are a few more examples of what a folder structure might look like:

<img src="./assets/com2.png" width="80%" style="border: 1px solid white">

## What is Path?

- A path is either `relative` or `absolute`

- `Relative path` - points to a specific location in a file system relative to the current directory you are working in.

- `Absolute path` - refers to the same location in a file system relative to the root directory

Here are examples using file paths:

- Absolute path

  - `/home/student/projects/Full_Stack/README.md`

- Relative path
  - `./Full_Stack/README.md`

## Important Keys

- `Command (mac) / Ctrl (PC)` - Known as a modifier key it is used in combination with other keys, enabling other keys on the keyboard to perform secondary functions.

- `Option (mac) / Alt (PC)` - Known as modifier key similar to Ctrl, enables other keys on the keyboard to perform secondary functions as well.

- `Tilde ( ~ )` - Located below the escape key. Allows us to get the the "home" directory on a computer via command line.

- `` Backtick ( ` ) `` - Located on the same key as Tilde commonly used in programming languages and command line.

- Angled Brackets - `< >`
- Curly Brackets - `{ }`
- Square Brackets - `[ ]`
- Parentheses - `( )`

## Keyboard Shortcuts

You may try to memorize these as these are quite useful and would make your code writing lickety-split.

**Mac Shortcuts:**

- `Command + x` - Cut
- `Command + c` - Copy
- `Command + v` - Paste
- `Command + z` - Undo
- `Command + y` - Redo
- `Command + s` - Save current document
- `Command + t` - Open a new tab or window
- `Command + f` - Find items in a doc
- `Command + a` - Select all

**Windows Shortcuts:**

- `Ctrl + x` - Cut
- `Ctrl + c` - Copy
- `Ctrl + v` - Paste
- `Ctrl + z` - Undo
- `Ctrl + y` - Redo
- `Ctrl + s` - Save current document
- `Ctrl + n` - Open a new tab or window
- `Ctrl + f` - Find items in a doc
- `Ctrl + a` - Select all

## What is the command line?

- The command line is a text based terminal app where we can interact with our computer with text commands.
- It has a long history, and was used to interact with computers before we had graphical user interfaces (like Windows) or a computer mouse.

- Below is an example of what command line looks like:

   <img src="./assets/comp3.png" width="90%" style="border: 1px solid gray">

## Why use the command line?

- `Faster:` The command line is faster to use than a GUI, although it does take some time to get comfortable with in the beginning. You could issue multiple commands to do something rather than having to constantly keep clicking and dragging.
- `Access:` The command line provides us access to parts of the operating system that would normally be off limits. For example, we can modify permissions, change settings, create and view hidden files, etc.
- `Software:` There are many tools and software that can only be used with the command line. For example, node.js.

## Set Up Command Line Environment

Let's open the command line in the "Terminal".

- Open Visual Studio Code

- On the very top menu find the menu item labeled `"Terminal"`.

- Click `New Terminal` or press `` control + ` `` to bring up the Terminal

   <img src="./assets/com4.png" style="border: 1px solid gray">

- Also try the alternative method of opening the Terminal by pressing `` control + ` `` to bring up the Terminal and hide it. It toggles the viewing of Terminal.

When you open a new Terminal window, you'll be in a directory (aka folder). By default, you'll be in the home directory that is shown as `~` in the Terminal.

But how do we see where we currently are and what is in the current directory we are in? How do we create a folder or a file?

## What is Command Line?

1. The command line is a text interface for your computer (known as `Terminal` on `OSX/Linux` and Command prompt on Windows)
1. It's a program that takes in commands, which it passes on to the computer's operating system to run
1. You can navigate through files and folders on your computer, just as you would with Windows Explorer on Windows or Finder on Mac OSX

## Apple OSX Command Line

Below is an image of the Apple OSX Command Line:

<img src="./assets/com11.png" width="70%" style="border: 1px solid gray">

<br>

There is a differance in commands on Windows and Mac

- The commands that we use here will be for Linux or Mac OSX or WSL. (Linux and Mac OSX are descendants of a common parent and are very similar).

## Why use the Command Line?

- Many apps are designed with CL interface and then the GUI is added. So you can **accomplish more** with CLI.
- We will use software and tools that can only be run from the command line.
- Commands can be stored in shell scripts and run through a timer (cron) or be run if an event happens on your computer.
- Command line commands make it very apparent what is being sent to the computer. There is nothing hidden.
- It's easier to work with remote machines, e.g. computers on AWS or a Linux server on a virtual private sharing provider on the internet.
  - https://www.wired.com/2012/07/command-line/

## What can you do with the Command Line?

- You can navigate folders
- Display files
- Create and delete files
- Run shell scripts
- Start apps
- Kill apps
- Use Git for version control
- Use Node.js

## Linux CLI Learning Objectives

1. Show current directory and contents of directory
1. Moving between directories
1. Creating files and directories
1. Write text to a file
1. View contents of a file
1. Deleting files and directories
1. Copying and pasting files and directories
1. Moving/cutting files and directories
1. Running multiple commands
1. Changing permissions
1. Run as administrator
1. Connecting to another computer or server
1. A few more useful commands
1. Using a basic text editor

# Your Command Line Demo

**Mac Users:**

- `Command + Spacebar`
- Type 'Terminal', and press enter.

**Windows:**

- Open Ubuntu Linux Prompt

## Which directory am I in?

- To find out where you are, type `pwd`. It stands for **print working directory**.

   <img src="./assets/com12.gif" width="60%" style="border: 1px solid gray">

- Type `pwd` before writing any commands to make sure you know where you are.

## Clear Screen

- To clear your Terminal, you may run the clear command ...

   <img src="./assets/com13.gif" width="60%" style="border: 1px solid gray">

## Listing Files

- Let's take a look at the files we have in our bootcamp folder. The `'ls'` command let's us do that.

   <img src="./assets/com14.gif" width="60%" style="border: 1px solid gray">

- `'ls'` stands for list. It lists all the files in that directory.

- To get more details about the file, we can use `"ls -l"`.
- `"ls -a"` also lists the hidden files (those that begin with a period).

   <img src="./assets/com15.gif" width="90%" style="border: 1px solid gray">

Now try `"ls -al"` and see what you get. Ubuntu provides an alias `"ll"` that shows you all this and does more.

## Changing Directories

- We can change directories by typing the `'cd'` command.
- `'cd'` stands for change directory

   <img src="./assets/com16.png" width="90%" style="border: 1px solid gray">

- `'cd'` or `'cd ~'` may be used to go to the `"Home"` directory as well.

   <img src="./assets/com17.png" width="90%" style="border: 1px solid gray">

## Creating Directories and Files Within Them

- Let's create a folder. We can do that with the `'mkdir'` command.
- `'mkdir'` stands for 'make directory'.

   <img src="./assets/com18.gif" width="90%" style="border: 1px solid gray">

- This will create a folder in `bootcamp` called "LiveMentors".

- We can create files using the `touch` command. Let's create a html file called 'index.html'.

   <img src="./assets/com19.gif" width="90%" style="border: 1px solid gray">

- Check your folder. Do you see the newly created file?

## Removing Files

- Now let's say we want to delete the index.html file. We can do that with this:

   <img src="./assets/com20.gif" width="90%" style="border: 1px solid white">

- The `'rm'` command stands for remove.
- Check the folder. Has it been deleted?

**Warning:**
Once you delete a file using the rm command, it's permanent!

The file does NOT get moved to the Trash/Recycle bin. It's permanently deleted, so be very careful when you use this command!

## Moving Up a Directory

- What if we want to go back to bootcamp?

   <img src="./assets/com21.gif" width="90%" style="border: 1px solid white">

- Unlike windows, the space between `cd` and `..` is required.

## Invoking VSCode from the CLI

To use "code <filename>" to open a file in VS Code from the command line:

1. Launch VS Code.
1. Open the Command Palette `(Shift-Ctrl-P or Shift-Cmd-P)` and type `'shell command'` to find the Shell Command: Install `'code'` command in PATH command.
1. Restart the terminal for the new $PATH value to take effect.
1. Now you'll be able to type `'code .'` in any folder to start editing files in that folder.

Reference: https://code.visualstudio.com/docs/setup/mac (edited)

## Writing Text to a File

- We may use an editor like VSCode to open a file and edit it.

- However, if we are working on command line, we would need to use a CLI editor like **nano** or **vim** or **emacs**. These are very powerful editors that have been around for a long time, but have a learning curve. If you have time, please ask for tutorials on one of these.

   <img src="./assets/com22.png" width="90%" style="border: 1px solid white">

## Reading Text From a File

- There are many ways to accomplish this, some of which are as follows. Try them and find one that you like ...

   <img src="./assets/com23.png" width="90%" style="border: 1px solid gray">

## How to get help?

- If you are not sure how to use a command, you may Google it, or try something like the following:

   <img src="./assets/com24.png" width="90%" style="border: 1px solid gray">

- You may use man pages, when provided by the author of the command, and when you want the most authentic and detailed information about the command. These are not always available.

## Deleting a Directory

- Deleting a directory is harder than deleting a file, but there are progressively more aggressive commands you may use ...

   <img src="./assets/com25.png" width="90%" style="border: 1px solid gray">

- For more details, Google or visit:
- https://www.cyberciti.biz/faq/delete-or-remove-a-directory-linux-command/

## Copying Files

- You would use the `"cp"` command to copy files (and directories).
- Syntax is `cp source destination`

   <img src="./assets/com26.png" width="90%" style="border: 1px solid gray">

## Moving Files

You would use the `"mv"` command to move files (and directories).

Syntax is `mv source destination`

Try to run the previous copy commands, but this time move the file app.html to the mywebapp folder. Check the results.

## Running Multiple Commands

- I just created a new directory, changed dir into that directory and created a file called app.html. With the && syntax, if the first command fails, the second will not be run.

   <img src="./assets/com27.png" width="100%" style="border: 1px solid gray">

## Changing Permissions

<img src="./assets/com28.png" width="90%" style="border: 1px solid gray">

Above I set the permissions like so ...

- 7 tells me the permissions for the current User
- 5 tells me the permissions for Group that the user owns
- 4 tells me the permissions set for Others

What do these numbers mean? See below:

<img src="./assets/com29.png" width="70%" style="border: 1px solid gray">

- 7 implies read, write and execute (rwx)
- 5 implies read and execute (r-x)
- 4 implies read only (r--)

Why these numbers? See below:

   <img src="./assets/com30.png" width="70%" style="border: 1px solid gray">

<br>

Try a few on your own, and use the wiki for reference:

- https://en.wikipedia.org/wiki/chmod

<img src="./assets/com31.png" width="70%" style="border: 1px solid gray">

## Administrator Permissions

Each Linux system has a `"root"` user that is a Super User and has no restrictions. Other users may get root like permissions by using `"sudo"` (Super User Do) before passing the command.

<img src="./assets/com32.png" width="70%" style="border: 1px solid gray">

`Sudo` allows one to login as another user

<img src="./assets/com33.png" width="70%" style="border: 1px solid gray">

... or login as `"root"`:

<img src="./assets/com34.png" width="70%" style="border: 1px solid gray">

the `"-"` tells the shell to use the startup files for root. The `"#"` warns you that you are connected as `"root"`.

## Few Useful Commands & Other Tips

Below are a few useful commands:

<img src="./assets/com35.png" width="70%" style="border: 1px solid gray">

<br>

<img src="./assets/com36.png" width="70%" style="border: 1px solid gray">

## Command Line Cheatsheets

### Command Line - Directory Navigation

The following commands allow for navigation of your directories and checking to see the current directory you are in:

<img src="./assets/com5.png" width="90%" style="border: 1px solid gray">

### Command Line - File/Folder Commands

The following commands allow for manipulation of files and folders:

<img src="./assets/com6.png" width="90%" style="border: 1px solid gray">

<br>

<img src="./assets/com7.png" width="90%" style="border: 1px solid gray">

### Command Line - Other

The following commands will be used less often but are still important to know:

<img src="./assets/com8.png" width="90%" style="border: 1px solid gray">

<br>

<img src="./assets/com9.png" width="90%" style="border: 1px solid gray">

<br>

<img src="./assets/com10.png" width="90%" style="border: 1px solid gray">

<!-- 

## Exercise 1: Advanced Navigation and File Creation

1.  Navigate to your home directory.
2.  Create a directory called "command_line_homework" if it doesn't already exist.
3.  Inside "command_line_homework," create a subdirectory named "exercise1."
4.  Navigate into "exercise1."
5.  Create a text file named "data.txt" with the content "This is exercise 1."

## Exercise 2: File Manipulation and Text Processing

1.  Navigate to the `"command_line_homework/exercise1"` folder.
2.  Create a new directory called `"notes"` and navigate into it.
3.  Inside the `"notes"` directory, create three text files: `"note1.txt"`, `"note2.txt"`, and `"note3.txt"`.
4. Add the content `"Text for note 1"`, `"Text for note 2"` and `"Text for note 3"` in these files respectively.
5.  Combine the contents of `"note1.txt"`, `"note2.txt"` and `"note3.txt"` into a single file named `"combined_notes.txt"`. Hint: you may use the redirection operator `>>` to the output from the three files into the combined file.
6.  Return to the `"exercise1"` folder.
7.  Use a command to count and display the number of words in `"combined_notes.txt"`

## Exercise 3: Advanced File Operations and Filters

1.  Navigate to the `"command_line_homework/exercise1"` folder.
2.  Create a backup directory called `"backup_data"` and navigate into it.
3.  Move the `"data.txt"` file from the `"exercise1"` folder to `"backup_data"`.
4.  Rename `"data.txt"` in `"backup_data"` to `"data_backup.txt"`.
5.  Navigate back to the `"exercise1"` folder.
6.  Use `echo` command to add the current date and time at the end of "combined_notes.txt" and save it as `"combined_notes_timestamped.txt"`
7.  Move `"combined_notes_timestamped.txt"` to the `"backup_data"` directory.
8.  Navigate to the `"backup_data"` directory.
9.  List the file contents of the `"backup_data"` directory and verify the files and timestamps.

## Exercise 4: Text Processing and Pipelines 

1.  Navigate to the `"command_line_homework/exercise1"` folder.
2.  Display the contents of `"combined_notes.txt"` on the terminal using the `cat` command.
3.  Use the `grep` command to find and display lines in `"combined_notes.txt"` that contain the word `"important"`.
4.  Redirect the output of the `grep` command to a new file called `"important_notes.txt"` in the `"exercise1"` folder.
5.  Use `sed` to replace all instances of `"important"` with `"crucial"` in `"combined_notes.txt"` and save the result as "crucial_notes.txt". (Hint: the syntax of `sed` command is `sed 's/from/to/g' file`)
6.  Use `wc` to count the number of lines and words in `"crucial_notes.txt"` and display the counts on the terminal.
7.  Create a backup of `"crucial_notes.txt"` in the `"backup_data"` directory. 

-->

---
---