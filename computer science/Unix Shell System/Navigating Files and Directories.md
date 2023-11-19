***

```ad-info
```$ pwd``` prints the current working directory
```

At the top is the **root directory** that holds everything else. We refer to it using a slash character, `/`, on its own; this character is the leading slash in `/Users/nelle`.

Inside that directory are several other directories: `bin` (which is where some built-in programs are stored), `data` (for miscellaneous data files), `Users` (where users’ personal directories are located), `tmp` (for temporary files that don’t need to be stored long-term), and so on.

We know that our current working directory `/Users/nelle` is stored inside `/Users` because `/Users` is the first part of its name. Similarly, we know that `/Users` is stored inside the root directory `/` because its name begins with `/`.

```ad-important
title: Slashes
Notice that there are two meanings for the ```/``` character. When it appears at the front of a file or directory name, it refers to the root directory. When it appears *inside* a path, it's just a seperator.
```

***

```ad-info
`ls` prints the names of the files and directories in the current directory. We can make its output more comprehensible by using the `-F` **option** which tells `ls` to classify the output by adding a marker to file and directory names to indicate what they are:

-   a trailing `/` indicates that this is a directory
-   `@` indicates a link
-   `*` indicates an executable
```

`ls` has lots of other **options**. There are two common ways to find out how to use a command and what options it accepts — **depending on your environment, you might find that only one of these ways works:**

1. We can pass a `--help` option to the command (available on Linux and Git Bash), such as:

	```zsh
	
     $ ls --help
     
	```
 
2.  We can read its manual with `man` (available on Linux and macOS), such as:

	```zsh
	
	$ man ls
	
	```

##### The ```man``` command
This command will turn your terminal into a page with a description of the `ls` command and its options.

To navigate through the `man` pages, you may use **↑** and **↓** to move line-by-line, or try **B and Spacebar** to skip up and down by a full page. To search for a character or word in the `man` pages, use **/** followed by the character or word you are searching for. Sometimes a search will result in multiple hits. If so, you can move between hits using **N** (for moving forward) and **Shift+N** (for moving backward).

To **quit** the `man` pages, press **Q**.

##### General Syntax of a Shell Command

![[Pasted image 20221210170427.png|center|250]]

`ls` is the **command**, with an **option** `-F` and an **argument** `/`. We’ve already encountered options which either start with a single dash (`-`) or two dashes (`--`), and they change the behavior of a command. [Arguments](https://swcarpentry.github.io/shell-novice/reference.html#argument) tell the command what to operate on (e.g. files and directories). Sometimes options and arguments are referred to as **parameters**. A command can be called with more than one option and more than one argument, but a command doesn’t always require an argument or an option.

You might sometimes see options being referred to as **switches** or **flags**, especially for options that take no argument. In this lesson we will stick with using the term _option_.

***

```ad-summary
title: Key Points
-   The file system is responsible for managing information on the disk.
    
-   Information is stored in files, which are stored in directories (folders).
    
-   Directories can also store other directories, which then form a directory tree.
    
-   `pwd` prints the user’s current working directory.
    
-   `ls [path]` prints a listing of a specific file or directory; `ls` on its own lists the current working directory.
    
-   `cd [path]` changes the current working directory.
    
-   Most commands take options that begin with a single `-`.
    
-   Directory names in a path are separated with `/` on Unix, but `\` on Windows.
    
-   `/` on its own is the root directory of the whole file system.
    
-   An absolute path specifies a location from the root of the file system.
    
-   A relative path specifies a location starting from the current location.
    
-   `.` on its own means ‘the current directory’; `..` means ‘the directory above the current one’.

```

