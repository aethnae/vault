***

```ad-info
```$ mkdir thesis``` creates a new directory called "thesis". Since `thesis` is a relative path (i.e., does not have a leading slash), the new directory is created in the current working directory
```

Note that `mkdir` is not limited to creating single directories one at a time. The `-p` option allows `mkdir` to create a directory with nested subdirectories in a single operation:

```zsh
$ mkdir -p ../project/data ../project/results
```

***

```ad-warning
title: Good names for files and directories
Complicated names of files and directories can make your life painful when working on the command line. Here we provide a few useful tips for the names of your files and directories.

1.  Don’t use spaces.
    
    Spaces can make a name more meaningful, but since spaces are used to separate arguments on the command line it is better to avoid them in names of files and directories. You can use `-` or `_` instead (e.g. `north-pacific-gyre/` rather than `north pacific gyre/`). To test this out, try typing `mkdir north pacific gyre`and see what directory (or directories!) are made when you check with `ls -F`.
    
2.  Don’t begin the name with `-` (dash).
    
    Commands treat names starting with `-` as options.
    
3.  Stick with letters, numbers, `.` (period or ‘full stop’), `-` (dash) and `_` (underscore).
    
    Many other characters have special meanings on the command line. We will learn about some of these during this lesson. There are special characters that can cause your command to not work as expected and can even result in data loss.
    

If you need to refer to names of files or directories that have spaces or other special characters, you should surround the name in quotes (`""`).

```

***

##### Creating Files in the Terminal

```zsh
nano draft.txt
```

or

```zsh
touch my_file.txt
```

1. The `touch` command generates a new file called `my_file.txt` in your current directory. You can observe this newly generated file by typing `ls` at the command line prompt. `my_file.txt` can also be viewed in your GUI file explorer.

2. When you inspect the file with `ls -l`, note that the size of `my_file.txt` is 0 bytes. In other words, it contains no data. If you open `my_file.txt` using your text editor it is blank.

3. Some programs do not generate output files themselves, but instead require that empty files have already been generated. When the program is run, it searches for an existing file to populate with its output. The touch command allows you to efficiently generate a blank text file to be used by such programs.

***

##### Moving files and directories

```zsh
mv thesis/draft.txt thesis/quotes.txt
```

The first argument tells `mv` what we’re ‘moving’, while the second is where it’s to go. In this case, we’re moving `thesis/draft.txt` to `thesis/quotes.txt`, which has the same effect as renaming the file.

Let’s move `quotes.txt` into the current working directory. We use `mv` once again, but this time we’ll use just the name of a directory as the second argument to tell `mv` that we want to keep the filename but put the file somewhere new. (This is why the command is called ‘move’.):

```zsh
mv thesis/quotes.txt .
```

***

##### Copying files and directories

The `cp` works very much like `mv`, except it copies a file instead of moving it. We can check that it did the right thing using `ls` with two paths as arguments - like most Unix commands, `ls` can be given multiple paths at once:

```zsh
cp quotes.txt thesis/quotations.txt
ls quotes.txt thesis/quotations.text
```

***

##### Using wildcards for accessing multiple files at once

`*` is a **wildcard**, which matches zero or more characters. Let’s consider the `shell-lesson-data/exercise-data/proteins` directory: `*.pdb` matches `ethane.pdb`, `propane.pdb`, and every file that ends with ‘.pdb’. On the other hand, `p*.pdb` only matches `pentane.pdb` and `propane.pdb`, because the ‘p’ at the front only matches filenames that begin with the letter ‘p’.

`?` is also a wildcard, but it matches exactly one character. So `?ethane.pdb` would match `methane.pdb` whereas `*ethane.pdb` matches both `ethane.pdb`, and `methane.pdb`.

Wildcards can be used in combination with each other e.g. `???ane.pdb` matches three characters followed by `ane.pdb`, giving `cubane.pdb ethane.pdb octane.pdb`.

When the shell sees a wildcard, it expands the wildcard to create a list of matching filenames _before_ running the command that was asked for. As an exception, if a wildcard expression does not match any file, Bash will pass the expression as an argument to the command as it is. For example, typing `ls *.pdf` in the `proteins` directory (which contains only files with names ending with `.pdb`) results in an error message that there is no file called `*.pdf`. However, generally commands like `wc` and `ls` see the lists of file names matching these expressions, but not the wildcards themselves. It is the shell, not the other programs, that deals with expanding wildcards.

***

```ad-summary
title: Key Points
-   `cp [old] [new]` copies a file.
    
-   `mkdir [path]` creates a new directory.
    
-   `mv [old] [new]` moves (renames) a file or directory.
    
-   `rm [path]` removes (deletes) a file.
    
-   `*` matches zero or more characters in a filename, so `*.txt` matches all files ending in `.txt`.
    
-   `?` matches any single character in a filename, so `?.txt` matches `a.txt` but not `any.txt`.
    
-   Use of the Control key may be described in many ways, including `Ctrl-X`, `Control-X`, and `^X`.
    
-   The shell does not have a trash bin: once something is deleted, it’s really gone.
    
-   Most files’ names are `something.extension`. The extension isn’t required, and doesn’t guarantee anything, but is normally used to indicate the type of data in the file.
    
-   Depending on the type of work you do, you may need a more powerful text editor than Nano.

```

