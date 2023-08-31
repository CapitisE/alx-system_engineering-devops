### 0. Where am I?
`pwd` prints the absolute path name of the current working directory.
### 1. What’s in there?
`ls` displays the contents list of your current directory.
### 2. There is no place like home
`cd` displays the contents list of your current directory.
### 3. The long format
`ls -l` displays the current directory contents in a long format.
### 4. Hidden files
`ls -la` displays the current directory contents, including hidden files (starting with .) and using the long format.
### 5. I love numbers
`ls -lna` displays current directory contents. `l` for long format, `n` allows user and group IDs to be displayed numerically and `a` displays hidden files.
### 6. Welcome
`mkdir /tmp/my_first_directory` creates a script that creates a directory named `my_first_directory` in the `/tmp/` directory.
### 7. Betty in my first directory
`mv /tmp/betty /tmp/my_first_directory` moves the file `betty` from `/tmp/` to `/tmp/my_first_directory`.
### 8. Bye bye Betty
`rm -r /tmp/my_first_directory/betty` deletes the file `betty` in `/tmp/my_first_directory`.
### 9. Bye bye My first directory
`rmdir /tmp/my_first_directory` deletes the directory `my_first_directory` in the `/tmp` directory.
### 10. Back to the future
`cd -` changes the working directory to the previous one.
### 11. Lists
`ls -la . .. /boot`  lists all files (including hidden ones) in the current directory and the parent of the working directory and the `/boot` directory (in this order), in long format.
### 12. File type
`file /tmp/iamafile` prints the type of the file named `iamafile` in the `/tmp` directory.
### 13. We are symbols, and inhabit symbols
`ln -s /bin/ls __ls__` creates a symbolic link to `/bin/ls`, named `__ls__` in the current working directory.
### 14. Copy HTML files
`cp -u *.html ..` copies all the HTML files from the current working directory to the parent of the working directory- only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory.
### 15. Let’s move
`mv [[:upper:]]* /tmp/u` creates a script that moves all files beginning with an uppercase letter to the directory `/tmp/u`.
### 16. Clean Emacs
`rm -r *~` creates a script that deletes all files in the current working directory that end with the character `~`.
### 17. Tree
`mkdir -p welcome/to/school` creates a script that creates the directories `welcome/`, `welcome/to/` and `welcome/to/school` in the current directory.
### 18. Life is a series of commas, not periods
`ls -pam` lists all the files and directories of the current directory, separated by commas (,). `p` means that directory names should end with a slash (/), `a` will list hidden files and `m` seperates the input with commas.
### 19. File type: School
`0 string SCHOOL School data !:mime School` creates a magic file `school.mgc` that can be used with the command `file` to detect `School` data files. `School` data files always contain the string `SCHOOL` at offset 0.

This exercise should be mostly easy once you go through the Resources for the project- a few might be slightly difficult, but it's nothing Google can't solve.

The task on magic files, however, is a different piece of cake. Further study is needed to understand the format of magic files and how to apply that understanding to the question. Here are some resources I used:
+ [A Quick guide to Magic files](https://0xpius.hashnode.dev/a-quick-guide-to-magic-files) by Pius Gabula
+ [magic (5) - Linux Manuals](https://www.systutorials.com/docs/linux/man/5-magic/)
+ [magic - Format of the /etc/magic file](https://www.ibm.com/docs/en/zos/2.5.0?topic=formats-magic-format-etcmagic-file)

