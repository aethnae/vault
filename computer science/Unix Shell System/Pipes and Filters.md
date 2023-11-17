***

```ad-info
`wc` is the ‘word count’ command: it counts the number of lines, words, and characters in files (from left to right, in that order).
```

The `-m` and `-w` options can also be used with the `wc` command, to show only the number of characters or the number of words in the files.

```ad-faq
title: Why Isn't It Doing Anything?
What happens if a command is supposed to process a file, but we don’t give it a filename? For example, what if we type:

`$ wc -l`

but don’t type `*.pdb` (or anything else) after the command? Since it doesn’t have any filenames, `wc` assumes it is supposed to process input given at the command prompt, so it just sits there and waits for us to give it some data interactively. From the outside, though, all we see is it sitting there: the command doesn’t appear to do anything.

If you make this kind of mistake, you can escape out of this state by holding down the control key (Ctrl) and typing the letter C once and letting go of the Ctrl key. **Ctrl+C**

```

***

##### Capturing output from commands

```zsh
wc -l *.pdb > lengths.txt
```

The greater than symbol, `>`, tells the shell to **redirect** the command’s output to a file instead of printing it to the screen. (This is why there is no screen output: everything that `wc` would have printed has gone into the file `lengths.txt` instead.) The shell will create the file if it doesn’t exist. If the file exists, it will be silently overwritten, which may lead to data loss and thus requires some caution.

We can now send the content of `lengths.txt` to the screen using `cat lengths.txt`. The `cat` command gets its name from ‘concatenate’ i.e. join together, and it prints the contents of files one after another. There’s only one file in this case, so `cat` just shows us what it contains:

```zsh
cat lengths.txt
```

```ad-tip
title: Output Page by Page
We’ll continue to use `cat` in this lesson, for convenience and consistency, but it has the disadvantage that it always dumps the whole file onto your screen. More useful in practice is the command `less`, which you use with `less lengths.txt`. This displays a screenful of the file, and then stops. You can go forward one screenful by pressing the spacebar, or back one by pressing `b`. Press `q` to quit.
```

***

##### Filtering output
Next we'll use the `sort` command to sort the contents of the `lengths.txt` file.
We will also use the `-n` option to specify that the sort is numerical instead of alphanumerical. This does *not* change the file; instead, it sends the sorted result to the screen:

```zsh
sort -n lengths.txt
```

-->

```zsh
  9  methane.pdb
 12  ethane.pdb
 15  propane.pdb
 20  cubane.pdb
 21  pentane.pdb
 30  octane.pdb
107  total
```

We can put the sorted list of lines in another temporary file called `sorted-lengths.txt` by putting `> sorted-lengths.txt` after the command, just as we used `> lengths.txt` to put the output of `wc` into `lengths.txt`. Once we’ve done that, we can run another command called `head` to get the first few lines in `sorted-lengths.txt`:

```zsh
sort -n lengths.txt > sorted-lengths.txt
head -n 1 sorted-lengths.txt
```

```zsh
  9  methane.pdb
```

Using `-n 1` with `head` tells it that we only want the first line of the file; `-n 20` would get the first 20, and so on. Since `sorted-lengths.txt` contains the lengths of our files ordered from least to greatest, the output of `head` must be the file with the fewest lines.

