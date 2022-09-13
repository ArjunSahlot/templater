# templater
Store templates for frequently created files and generate them from the command line!

## How to download
1. Download this repository
2. Add the path of the donwloaded repository to your path
3. If you get a permission denied error, then you will need to give the "temp" file permission to execute, `chmod +x /path/to/file`
4. If you run the following in your terminal/command prompt and get a help message, then you are good to go! `temp -h`

## How to use
This executable will store all the template files in the ".templates" folder in your home directory.

### To add a template file
Add it to the ".templates" folder. You can even organize it in folders. Check out the example at the bottom.

### To generate a template file
If you completed all the download instructions and can see in the help message, then you can use temp properly. You need 2 items to generate a temp file. The location of the template file, the new location of generated file. You can enter it in using `temp -p folder1 folder2 file.txt -n file.txt`

### Example
If you want a template file for competitive programming, and you code in 2 languages (say C++ and Python). Then you can create a folder inside the ".templates" folder for competitive programming, and then inside of that you can have a c++ file and a python file.
<pre>
Folder structure:
.templates
└── competitive
    ├── cpp
    └── py
</pre>
Then you can use this command to create a starter file in your current directory, `temp -p competitive cpp -n answer.cpp`

Note: You don't have to put an extension in the template files. I find it easier to remove the extensions so that I can put the path as `competitive cpp` for a cpp competitive file instead of `competitive temp.cpp`.
