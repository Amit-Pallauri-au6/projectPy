# Junk file Organizer

> as we all have struggled with organizing files manually someday, so the aim of this project is to show you how you can organize random files as per alphabate, size and their extensions.

## Requirements

### Modules Used

1. import os - to get, create, scan all the files from the directories
2. import sys - to achieve the list of command line arguments passed to a Python script
3. import shutil - to move the files from one directory to another
4. import ntpath - to get the exact path of the file

### Approach Used

1. For SIZE based organization - I have used a variable(size) to store the size of the file and then checking the file size by using the if and elif conditions and then arranging the files into their specific folders by creating new directories as per the size of the files. All the files are first moved into (Organized Directory) then inside this folder all the other directories are created accordingly. The files which are in Bytes are stored inside a new directory called BYTES and just like that all the different files are arranged in the subsequent folders( BYTES, KB, MB, GB)

2. For EXT based organization - I have created a dictionary and saved all the possible extensions I can think of to access the extensions and afterwords moving the files to their specified directories. Checking the extension of the file in the computer directory and then compairing it with the dictionary values of extensions if matched then creating the new directory named Organized and inside it moving the different files according to the specified new directories.

3. For Alphabet based organization - First the no of files are accessed from the directory and then according to the starting letter the files are arranged into their subsequent directories named according to the first name of the files.
All the files are stored in a single directory named as Organized.

### Instructions to run

To run the command in cli, you have to paste the fileOrganizer.py file inside that folder where all the junk files are present and then open the Cli and pass the following commands

- if you want to organize by size : python fileOrganizer.py size
- if you want to organize by alphabate : python fileOrganizer.py alpha
- if you want to organize by extention : python fileOrganizer.py ext

`if you don't pass any particular organizing criteria, by default it will organize as per alphabate`
