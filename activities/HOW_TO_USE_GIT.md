# Git

Git is a modern Version Control System, and has largely taken over from
earlier VCSs, like Subversion (`svn`) and Concurrent Versions System (`cvs`).
Most new projects use `git`.

Version control means that as you make incremental changes to your files, you
can mark snapshots of your code to easily revert back to. Perhaps the most
important feature is the ability for multiple people to work on the same
codebase, and easily update their local code with changes pushed to the server
by other programmers.

# To check out our class repository...

...simply run...

```
$ git clone https://github.com/reynoldsnlp/W18_DIGHT360.git
```

in the `bash` command line shell. (Do not copy the `$` prompt. It is just a
conventional way to mark that this command is given to `bash`.) This command
will create a folder in your current directory named `W18_DIGHT360`.

# Navigating in bash

The command line `bash` (Bourne Again SHell), is found in almost every Linux
distro, and is now also available inside Windows 10.

Open the terminal (aka bash shell) type `pwd` (Present Working Directory). That
shows you your current location in the directory structure.

To "MaKe a DIRectory" you simply type `mkdir [new directory]`.

To "Change Directory" you simply type `cd [new directory]`. Try going into the
directory you just created. (Names are case-sensitive.) I would just type the
first couple letters of the name and then tab to autocomplete. Bash knows when
you've typed enough to know which thing you have in mind. Using [tab] saves a
lot of effort and avoids typos. Type `pwd` again to see where you are now and
compare it with your original pwd output.

To LiSt the contents of a directory,  just type `ls`.

To move up to a parent directory, just type `cd ..`. Bash interprets one dot as
the current directory and two dots as the parent directory. `pwd` should now
give the same output as when you first started the terminal.

Now you can just move around your file system. Use `pwd`, `ls`, and `cd` (and
[tab]!) until all of them are automatic.

You can also spend some time creating files and deleting files. Deleting files
in bash is risky because you can't undo it, so always be careful that you don't
have typos.

When `pwd` and `ls` print to the screen, they are using a channel called
`stdout` (standard out). You can redirect a process' stdout to a file using `>`.
Try `pwd > MY_FIRST_FILE.txt`, then `ls` to see that you created a file. To read
the file `cat MY_FIRST_FILE.txt`. `cat` = conCATenate, so named because it 
combines multiple files and sends them to `stdout`.

To delete (ReMove) the file `rm MY_FIRST_FILE.txt`.

Last, you can use `echo` to send any string to stdout. Try `echo "is there an echo
in hear?"`

Try making a few files using `echo` and `>`.


# Updating your git repository

You can always update your repository by using...

```
$ git pull
```

This attempts to merge your local changes (if there are any) with changes that
have been pushed to the server by other contributors.

I strongly recommend that you never change any of the files in the repository.
First make a copy of the file (`cp <old_file> <new_file>`), then do whatever you want with the COPIED file.

