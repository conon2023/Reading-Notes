Reading-Notes
My notes during the Tech Educators Coding Booting 

# READ 02 - THE CODER'S COMPUTER EXAMPLE MODULE #   
## The command Line - Your Window into the Computer ##
**_What is a command line?_**
-*A command line, or terminal, is a text based interface to the system. Inputs are text via the keyboard and outputs are equally by texts and on screen.

The command line typically presents you with a prompt. Next is the command and then the command line. There must be a space between the first command and the first command line argument. 

### OPENNING A TERMINAL 
#### On a mac:
Go to applications and then utilities

### On a Linux:
Go to applications. Then go to system or applications and finally to utilities. Someimtes you may be able to right click on the desktop and find the option 'open terminal'. 

### On Windows:
An SSH client will be required if you intend to remotely log into another machine. **Putty**, which is free, is a good one.

### THE SHELL, BASH 
The shell is within the terminal and it that part of the operating system which showcases the terminal's **behavior and looks** after running or executing. The most common shell is called **bash**, which stands for **Bourne again shell.**
The command called **echo** will display a system variable stating the shell you are using. 

### SHORTCUTS
Once you have entered a command before, you can use the up and down arrow keys to go through all of them. To edit previously entered commands, use the left and right arrow keys.

## Basic Navigation - Exploring the System!
This is about moving around. Most tasks will generally reference or be able to get to the correct system location. Some of these tasks include: 

**PWD** - which stands for **Print Working Directory**. PWD command will always tell the user where he is i.e. It lets the user know what the current or present working directory is. 

**ls** - the listing command. 
This **list** (ls) command allows the user know the content of our current location. 
Running a list with no arguement as shown above will simply output a plain listing of the current location. 
_Here are a few examples:_

**ls**
The command above lists the contents of our current directory. 

_**ls -l**_
This command has a single line option (-l). It a short listing with various attributes like normal(-) or directory (d); permission for file or directory, number of blocks, owner of the file, group file or directory belongs to, file size, file modification time and actual name of the file or directory. 

_**ls /etc**_
The command above will not list current directory but will, instead, list the directory's contents. 

_**ls -l/etc**_
ls will output a long listing of the directory /etc.

### Paths
This is a means to access a particular file or directory (location) in the system. 

#### Absolute and Relative Paths ####
In the **linux system,** the filing system is **hierarchical** The **root directory** is at the very top and denoted by a single slash ( / ). Then there are subdirectories and files may reside in any of these directories. 

**Absolute paths** specify a location (file or directory) in relation to the root directory. It usually begins with a forward slash ( / ). 

**Relative paths** specify a location (file or directory) in relation to where we currently are in the system and will not begin with a slash.

## More on Paths
~ (tilde) - This is a shortcut for your home directory. eg, if your home directory is /home/ryan then you could refer to the directory Documents with the path /home/ryan/Documents or ~/Documents

. (dot) - This is a reference to your current directory. eg in the example above we referred to Documents in a relative path. It could also be written as ./Documents (Normally this extra bit is not required but in later sections we will see where it comes in handy).

.. (dotdot)- This is a reference to the parent directory. You can use this several times in a path to keep going up the hierarchy. eg if you were in the path /home/ryan you could run the command ls ../../ and this would do a listing of the root directory.

Here are some examples:
user@bash: pwd
/home/ryan
user@bash:ls ~/Documents
user@bash: file1.txt file2.txt file3.txt

user@bash: ls ./Documents
file1.txt file2.txt file3.txt

user@bash: ls /home/ryan/Documents
file1.txt file2.txt file3.txt

user@bash:
user@bash: ls ../../
bin boot dev etc home lib var

user@bash:
user@bash: ls /
bin boot dev etc home lib var



## Moving around a bit ##
We use the change director (cd) command to move around the path. 
## cd[location]
The cd command without any arguement will always take you back to the home directory. 

## Tab Completion##
Tab completion is an auto complete feature that helps us complete the paths we are already typing.

## Everything is a File ##
In the Linux system, it is important to understand that everything is basically a file. 
Texts, directories are all files. Keyboards are files we read from while monitors are files we read to. 

## Linux - An Extensionless System ##
Sytems like windows use file extensions which is a set of 2 - 4 characters after a full stop at the end of the file. For example we have file.exe, file.txt, file.png/gif/jpg, to determine denote what type of file that is. In Linux, however, the system actually ignores the extension. Rather, it looks inside the file to determine what type of file it is. Take a a file **chidi.png** for instance, even if I rename it **chidi.txt** or just **chidi**, Linux would still happily treat the file as an image file. This can make it a bit dificult to know what type of file it is in Linux. Forunately for users, there is a command called **file** which we can use to find what file it is. And that is: **file [path]

## Linux is Case Sensitive
Unline windows, Linux sees every file, directory and command as distinct. In essence, it is case sensitive.  

## Spaces in Names
A space on the command line is how we seperate items. It identies what is the program name as well as each command line argument. Linux does not allow for spaces in directory and file names. This is beacause it will see the two as distinct. To deal with this, we can either use **quotes** or the **escape (\)** character. So, it will be **\cd "James Monday"** or **\cd James\ Monday**

## Hidden Files and Directories
In Linux, we are able to identify a hidden file or directory when its name starts with a **. (full stop)**. To make a file or directory hidden, simple create  or rename it with a .(fullstop) starting it.   
The command **ls** that we have seen previously will not list hidden files and directories. But when we inclide the line option **-a** it will show hidden files and directories. 



# GROWTH MINDSET June 06, 2023.   
_***What is a Growth Mindset?
This is a fundamental belief that I can do more and be better than I am through hardwork and consistent effort. This belief butresses the notion applied effort towards a goal will yield better dividend than one's inate talents and ablities.   

## Three (3) Ways to Keep the Growth Mindset Alive
1. Always have the end in mind.   
![Have the end in mind](https://www.bing.com/images/search?view=detailV2&ccid=1xinw2dj&id=1695B3DA25A10CA6031AED040B17E27AA1FA30D6&thid=OIP.1xinw2djbwBKKkJ6bddtqwAAAA&mediaurl=https%3A%2F%2Fi.pinimg.com%2F474x%2Fa6%2Fb5%2Fe5%2Fa6b5e5ce637a5867ba1c10267bef71d8.jpg&cdnurl=https%3A%2F%2Fth.bing.com%2Fth%2Fid%2FR.d718a7c367636f004a2a427a6dd76dab%3Frik%3D1jD6oXriFwsE7Q%26pid%3DImgRaw%26r%3D0&exph=474&expw=474&q=free+stock+image+showing+consisten+effort&simid=608048635243732048&form=IRPRST&ck=3F90DB4C26AF175F2E9487F81B60F5D1&selectedindex=13&ajaxhist=0&ajaxserp=0&pivotparams=insightsToken%3Dccid_eI%252FNkp8W*cp_77AB35F76B0FAA514731E19387C56B5D*mid_609019225602032F66FD71387B299A07F55D7E12*simid_608015323476005874*thid_OIP.eI!_Nkp8We9OZHR!_daucNdgHaHa&vt=0&sim=11&iss=VSI&ajaxhist=0&ajaxserp=0)
2. Consisten effort towards a goal will pay better dividend than talent and abilites.   
(https://www.bing.com/images/search?view=detailV2&ccid=ta79peMq&id=8541229BA43F9F8A429C982B95092F37BAB26052&thid=OIP.ta79peMqDQ64wha71HQLPAHaDl&mediaurl=https%3A%2F%2Fi.pinimg.com%2Foriginals%2Fa8%2Fdf%2Fed%2Fa8dfedd37a83cbe2d021008cf2fcef5f.png&cdnurl=https%3A%2F%2Fth.bing.com%2Fth%2Fid%2FR.b5aefda5e32a0d0eb8c216bbd4740b3c%3Frik%3DUmCyujcvCZUrmA%26pid%3DImgRaw%26r%3D0&exph=436&expw=900&q=free+stock+image+showing+consisten+effort&simid=607997155764088089&form=IRPRST&ck=1FA3FC4381C945D41057B0CD388EA138&selectedindex=1&ajaxhist=0&ajaxserp=0&vt=0&sim=11)
3. Taking a short break when it seems all overwhelming and coming back later on have been known to help.
(https://www.bing.com/images/search?view=detailV2&ccid=vupylNDk&id=C5FEEDA2D19CE3666245AFFC43A4DDB135A8873D&thid=OIP.vupylNDkkgtcj4-zykCWhAHaDt&mediaurl=https%3a%2f%2fhealthyvoyager.com%2fwp-content%2fuploads%2f2017%2f09%2frelax-05.jpg&cdnurl=https%3a%2f%2fth.bing.com%2fth%2fid%2fR.beea7294d0e4920b5c8f8fb3ca409684%3frik%3dPYeoNbHdpEP8rw%26pid%3dImgRaw%26r%3d0&exph=1024&expw=2048&q=free+stock+image+showing+people+relaxing&simid=607997915990995328&FORM=IRPRST&ck=20AE48DBA3A6DE6103DC1A576FC8771D&selectedIndex=0&idpp=overlayview&ajaxhist=0&ajaxserp=0
4. Consult those knowledgeable in the field when all else fails.   
![]<img src="tykeu.jpg" alt="Consult Others" width="300" height="200">

**Chidi Ononye.   
Tech Education Student
