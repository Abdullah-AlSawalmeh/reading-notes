#The Command Line

A command line, or terminal, is a text based interface to the system.
You are able to enter commands by typing them on the keyboard and feedback will be given to you similarly as text.

Within a terminal you have what is known as a shell. This is a part of the operating system that defines how the terminal will behave and looks after running (or executing) commands for you.
There are various shells available but the most common one is called bash which stands for Bourne again shell.
Terminal = Command line running bash.

You can open as many command lines as you want with the GUI. 
There must be a space between the command and the first command line argument also options are typically used to modify the behaviour of the command.
Options are usually listed before other arguments and typically start with a dash ( - ).

There are 2 types of paths we can use, absolute and relative. Whenever we refer to a file or directory we are using one of these paths. Whenever we refer to a file or directory, we can, in fact, use either type of path (either way, the system will still be directed to the same location).

The file system under linux is a hierarchical structure. At the very top of the structure is what's called the root directory. It is denoted by a single slash ( / ). It has subdirectories, they have subdirectories and so on. Files may reside in any of these directories.

Absolute paths specify a location (file or directory) in relation to the root directory. You can identify them easily as they always begin with a forward slash ( / )
Relative paths specify a location (file or directory) in relation to where we currently are in the system. They will not begin with a slash.

In linux everything is  actually  a file. A text file is a file, a directory is a file, your keyboard is a file (one that the system reads from only), your monitor is a file (one that the system writes to only) etc.

In other systems such as Windows the extension is important and the system uses it to determine what type of file it is. Under Linux the system actually ignores the extension and looks inside the file to determine what type of file it is.

Other systems such as Windows are case insensitive when it comes to referring to files. Linux is not like this. As such it is possible to have two or more files and directories with the same name but letters of different case.

Be aware of case sensitivity when dealing with command line options. For instance with the command ls there are two options s and S both of which do different things.

Use quotes or escape characters to avoid the spaces in the folders names or paths.

To make a file or directory hidden all you need to do is create the file or directory with it's name beginning with a . or rename it to be as such. Likewise you may rename a hidden file to remove the . and it will become unhidden.



#Terminal commands and options used with it 

echo $SHELL  === > > > If you would like to know which shell you are using you may use
pwd === > > > which stands for Print Working Directory, It tells you what your current or present working directory is.
ls === > > > It's short for list, used to know what is there in the working directory.
ls -l === > > > indicates we are going to do a long listing, long listing means:
	1. First character indicates whether it is a normal file ( - ) or directory ( d )
	2. Next 9 characters are permissions for the file or directory (we'll learn more about them in section 6).
	3. The next field is the number of blocks (don't worry too much about this).
	4. The next field is the owner of the file or directory (ryan in this case).
	5. The next field is the group the file or directory belongs to (users in this case).
	6. Following this is the file size.
	7. Next up is the file modification time.
	8. Finally we have the actual name of the file or directory.
ls /etc === > > >  When we do this it tells ls not to list our current directory but instead to list that directories contents.
ls -a === > > > it does show hidden files and directories.
cd === > > > In order to move around in the system, If you run the command cd without any arguments then it will always take you back to your home directory.
file ==== > > > to know what type a file is, image, text ... etc 


#Shortcuts
You can traverse your commands history using the up and down arrow keys.
Here are some more building blocks you may use to help build your paths:
	1. ~ (tilde) - This is a shortcut for your home directory. eg, if your home directory is /home/ryan then you 	could refer to the directory Documents with the path /home/ryan/Documents or ~/Documents
	2. . (dot) - This is a reference to your current directory. eg in the example above we referred to Documents 	on line 4 with a relative path. It could also be written as ./Documents (Normally this extra bit is not 	required but in later sections we will see where it comes in handy).
	3. .. (dotdot)- This is a reference to the parent directory. You can use this several times in a path to keep 	going up the hierarchy. eg if you were in the path /home/ryan you could run the command ls ../../ and this 	would do a listing of the root directory.

If you use Tab Completion before encountering the space in the directory name then the terminal will automatically escape any spaces in the name for you.



