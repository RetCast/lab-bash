![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# Lab | Bash

## Introduction

In this lab we are going to practice with [`bash`](<https://en.wikipedia.org/wiki/Bash_(Unix_shell)>), a shell and command-line language!

## Setup

1. Fork the repo in your git hub account and then clone the folder "lab-bash" to your machine and navigate to it folder.

2. Check the contents of the folder using the "ls" command

```shell
$ ls
```

and you should see the following:

```shell
exercises  inputs  lorem  lorem-copy  modules  outputs  README.md
```

3. Stay in the same directory/folder and complete the following exercises.

## Exercises

1. Using the echo command print in console "Hello World". Here is some info about echo command [https://discuss.codecademy.com/t/what-are-practical-uses-of-the-echo-command/394788]
  **Answer: echo "Hello World"**
2. Create a new directory called `new_dir`.
**Answer: mkdir new_dir**
3. Delete/Remove the directory `new_dir`.
**Answer: rm -r new_dir/**
4. Copy the file `sed.txt` from the `lorem` folder and paste it to the folder `lorem-copy` folder.
**Answer: cp lorem/sed.txt lorem-copy/**
5. Copy the other two files from the `lorem folder` to `lorem-copy` folder in just one line using semicolon `;`.
**Answer: cp lorem/at.txt lorem-copy/ ; cp lorem/at.txte  lorem-copy/**
6. Show the `sed.txt` file content from the `lorem` folder.
**Answer: cat lorem/sed.txt**
7. Show the `at.txt` file and `lorem.txt` file contents from `lorem` folder.
**Answer: cat lorem/at.txt; echo " " ; cat lorem/lorem.txt**
8. Print the first 3 rows in `sed.txt` file from lorem-copy folder.
**Answer: head -n3 lorem-copy/sed.txt**
9. Print the last 3 rows in `sed.txt` file from lorem-copy folder.
**Answer: tail -n3 lorem-copy/sed.txt**
10. Add `Homo homini lupus.` at the end of `sed.txt` file in the `lorem-copy` folder.
**Answer: echo "Homo homini lupus" >> lorem-copy/sed.txt**
11. Print the last 3 rows in `sed.txt` file from `lorem-copy` folder. You should see `Homo homini lupus.`.
**Answer: tail -n3 lorem-copy/sed.txt**
12. `sed` command is used to replace the text in a file. Use the `sed` command to replace all occurances of `et` with `ET` in the file `at.txt` file present in the folder `lorem`. You can use the following link to refer to `sed` commands [https://www.linode.com/docs/guides/manipulate-text-from-the-command-line-with-sed/]
**Answer: sed -i 's/et/ET/g' lorem/at.txt**
13. Check the contents of the sed.txt file using `cat` command.
**Answer: cat lorem/at.txt**
14. Find who is the system user. 
**Answer: whoami**
15. Find the current path of the directory you are in.
**Answer: pwd**
16. List all files with the extension `.txt` in lorem folder.
**Answer: $ ls *.txt (It only works if I am inside the current directory)**
17. Count the rows in `sed.txt` file from lorem folder. Look concatenate `cat` and `wc` with the pipe `|`.
**Answer: cat lorem/sed.txt | wc -l**
18. Count the **files** which start with `lorem` in all directories.
**Answer: set lorem* ; echo "$#"**

## Bonus

20. Store your `name` in a variable with `read` command.
**Answer: $ read input1 input2 input3**
**Daniel Retana Castañeda**
21. Print that variable.
**Answer: $ echo $input1; echo $input2; echo $input3
Daniel
Retana
Castañeda**
22. Create a new directory named with variable `name`.
**Answer: $ mkdir $input1**
23. Remove that directory.
**Answer: rm -r $input1**
