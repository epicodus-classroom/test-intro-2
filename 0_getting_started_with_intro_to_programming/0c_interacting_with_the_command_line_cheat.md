## Terminology
<hr />

* **Path**: The unique location of a file or folder in the file system hierarchy. Example:  `Users/Andrea/Pictures/fun-day.jpg` is the path for the image called `fun-day.jpg`.

* **Directory**: Another name for a folder in file system hierarchy. Example: `Users/Andrea/Pictures/fun-day.jpg` is a path that has 3 directories:  `Users`, `Andrea` and `Pictures`.

* **Subdirectory**: A directory within another directory. Example: In the path, `Users/Andrea/Pictures/fun-day.jpg` , `Andrea` is a subdirectory of `Users` and `Pictures` is a subdirectory of `Andrea`.

* **Home Directory**: The topmost level of your user directory; the directory where you begin when you open the terminal.  (To view your home directory in the _Finder_ (the graphical user interface on the Mac), click somewhere on the desktop, click on the **Go** menu at the top of the screen, and select the **Home** menu option. To get to your home directory in the _Terminal_, type `cd ~` at the command line prompt.)

## Frequently Used Commands:
<hr />

For reference, here are all the commands we learned about in this lesson. Feel free to reference this as much as you need! Pretty soon, these will become second-nature:

* `$ pwd`: prints the path to the current working directory to the screen.
* `$ ls`: lists out the directories (folders) and files in the current working directory.
* `$ ls directory-name`: lists out the directories and files in the specified directory.
* `$ cd directory-name`: changes the current directory to the one specified.
* `$ cd ..`: change current directory up one level to the parent directory.
* `$ cd ~`: change the current directory to the home directory (`/Users/Guest` on Epicodus computers).
* `$ mkdir new-directory-name`: creates a new directory (folder) in the current working directory unless otherwise specified.
* `$ touch new-file-name`: creates a new, empty file in the current working directory unless otherwise specified.
* `$ mv file-name new-file-name`: moves the contents of the first file into the second file, essentially renaming the file. First file is removed.
* `$ cp file-name new-file-name`: creates an exact copy of the contents of the first file into the second file. Both files exist.
* `$ rm file-name`: deletes the file.
* `$ rm -r directory-name`: deletes the directory and all of the files within it. Be very careful with this command.
* `$ cat file-name`: prints out the contents of the specified file to the screen.
* `$ cd Desktop` change directory to a directory named Desktop (located inside of the current directory)
* `$ cd /Users/Guest` change to /Users/Guest directory (which happens to be the home directory on the Epicodus computers)
* `$ cp Documents/hi.txt .` copy the file `hi.txt` from the Documents directory to whatever directory you are currently working in
* `$ mv Documents/hi.txt .` move the file `hi.txt` from the Documents directory to whatever directory you are currently working in
