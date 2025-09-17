Important Notes

Common Operating System- MacOS, Windows,Linux etc.

Command Line CLI- text based interface 
Ex: DOS or UNIX

Graphical User Interfaces- (GUI) use pictures and menus to display commands. Ex: Windows or Mac OS

Specialized operating systems- hand- held personal device  (IOS, Android, Raspbian, etc)

Command Line Interface- helps you understand how to navigate through files,  you can  operate your PC even if the GUI is broken. Open source  software  often expects  you to know CLI basics to install programs and to move  or change files. Lastly  to secure  your computer against a hacker who knows  CLI and terminal programs. 

Terminal: A text based command window
aka: command prompt
aka: shell

Windows- Start- Run- cmd, Kali Linux- Click Ctrl- Alt- t on Desktop

Window Prompt: an indicator that the computer is ready to receive commands- uses a symbol like >

Linux Prompt- an indicator that the computer is ready to receive  commands  uses symbol  like $ and >. 

Path- the list of folders or " directory tree" in which your file is stored.  the prompt is always focused on a specific folder so any commands will affect  the files in that folder. Every file has a path- where it is inside all the folders  in your computer. 

Linux Help Command- whenever you need help with a command type  "man"  and the command name.This will give you the manual for that command  including all possible options.

To exit man page type Q and enter. Also when your screen gets too full  type clear and enter.


Path Navigation Commands- pwd- find which path im currently in.
ls- list the contents of the current directory
ls -1- list contents in long format.
ls -a- list the contents including hidden files. 
ls- is an example of command which can take options  -a  is an example  of an option . The 
options change behavior of the command.



Two Important Tips

A command needs air around it, whenever you type a command  make sure  there is space  before and after it
Correct- ls -a or echo word or man pwd
Incorrect- ls-a or echoword or manpwd

Unix is case sensitive so LS is not same as ls, same applies  to file names  myfile.txt, MYfile.txt and MYFILE.txt are three seperate files. 

What hidden files all have in common
They all have dot in front of them

Path Navigation Commands

Change to Directory- cd foldername

Change to parent directory- cd.. (this takes you up one folder level)

Change to your home directory- 
. cd ~

Change to a folder in you home directory-
. cd ~/Documents




try It: Type cd ~/Documents then pwd, which is the whole path  of your location
/home/kali/Documents/

Now type cd then pwd- what is the whole path of your location?
/home/kali/

What happens if you type cd/ ?
You change to the /directory (the root directory)

What happens if you just type cd?

Notice this takes you back to the /home/kali directory



File & Directory Management

.cp file1 file2- copy a file- this command will make a copy of file1  in the current directory and calls it file2

mv file1 /newplace/file1- move file1 to file1 in the new place  directory  or can be used to rename a file.

mv file1 file2- rename file1 to file2 in this directory. 

touch filename: create an empty file with a name

rm: remove file (aka delete)




File & Directory Management (cont'd)

.mkdir- make a directory (Directories can only be removed if they are empty)
Example: $mkdir Superfolder

. rmdir- remove directory (You must get out of the directory before you try to  delete it )
Example: $rmdir Superfolder

To return to homedirectory type cd ~ 

Type mkdir Stufffolder the use ls to make sure your folder is created

To change into Stufffolder directory- command use cd StuffFolder 

Type touch stuffing.txt ~Documents/stuffing.txt, how many copies now ?  2 copies  we copied.

Try it: Removing Files and Directories:

Removing StuffFolder with rmdir- it won't work because  it is not empty  and your still inside the directory.

To go up one direction command used should be cd

Type cd StuffFolder to go back in 

Type mv stuffing. txt ~ /Downloads/ trash.txt

Type cd to go up one level out of the StuffFolder, can you remove it ?  the answe is yes.


Cool Tricks 
Use automatic File Completion
. Type a command
. Then the first letters of the file 
. Hit Tab- will try to fill in the possible choice

.Hit UP and DOWN arrow keys, each previous command  you typed will appear.
Keep using UP key to scroll through until you find it.

Reading Files

cat: display a file all at once why use cat instead of less? 
Faster
Dont have to type Q to exit goes right to the prompt.

less- display a file on one page at a time 
press [space-bar] if you wnat to see the next page 
type [q] if you wnat to quit reading 

Type cat /etc/passwd- notice that the text streamed  throught the end.

Type less/ etc/ passwrd- Use the space bar to page down through  the text.  At the end use [q] to exit.


About Sudo

You must be an administrator: SuperUser, there is a built  in SuperUser  called root.

They put sudo infornt of the command: sudo <command> = superuser 

Example: sudo mkdir ThingsToLearn

To switch over to the root account: sudo su

To identify who is the actice user:whoami

Try It: Sudo

change into directory: cd ~/Documents 

On prompt type whoami

To list what is on the root user home folder type , ls  /root  you will get a permission denied message

Now use sudo successfully list the contents of the /root folder
Type: sudo ls/ root

Change to being the root user 
Type sudo su

Use whoami again to identify the current user, username changed to root  but you still on kali's home folder

Change back to being kali user 
Type su kali 

Remember: sudo is not needed to return the orriginally  logged in user. If you wanted to switch to a different user you would need their password.