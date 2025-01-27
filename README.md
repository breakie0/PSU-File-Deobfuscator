# PSU File Deobfuscator

# What is this tool?
This tool is to co-exist with the [psu generic parser](https://github.com/Agrathejagged/tenora-works) by [Agrathejagged](https://github.com/Agrathejagged).
If you've used the psu parser before you'll know that it doesn't support some PSU data files. this tool can filter out these files from a directory.
It also can rename the md5 hashed filenames to the original names for a reader friendly experience.

# Why does this exist?
That main reason for this tool existing is to help with PSU file management / usability. As someone who has needed to use PSU data files in some capacity,
this was made to make the process alot less time consuming. That is the main purpose, reducing time consumption.

NOTE: This tool is not designed for your game directory data files! You should copy the DATA directory and/or backup files before using this tool for safety!

The tool is seperated into 2 sections, Validating files and Renaming files.

# Validating
  What can it do:
    - Goes through a directory and checks for valid files that the [psu generic parser](https://github.com/Agrathejagged/tenora-works) can open.
    - Remove / Relocate files parser cannot open.
    
  How to use:
    - Select the source folder of PSU DATA files.
    - Destination folder is where you want to move files the [psu generic parser](https://github.com/Agrathejagged/tenora-works) can't open.
    - Check files: Checks the selected source directory and returns the amount of valid and invalid [psu generic parser](https://github.com/Agrathejagged/tenora-works) data files.
    - Move bad files: Removes all the files incompatible with [psu generic parser](https://github.com/Agrathejagged/tenora-works) and moves them to the destination folder.

# Renaming
  What can it do:
    - Goes through a directory and renames PSU data files to the original names using a mapping file.
    
  How to use:
    - Select the source folder of your PSU DATA files.
    - Select the mapping file, Mapping file contains the filenames as well as filenames that aren't md5 hashed, in this repo there is "AOTI filelist.txt" that contains most of the filenames.
    - Clean mapping file: When checked, renaming files will clean any potential problems in the mapping file.
    - Rename files: Goes through the selected folder and renames any PSU files contained in the mapping file.

# Console
  In case you need to see whats happening under the hood.

