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
An SSH client will be required if you intend to remotely log into another machine. Putty, which is free, is a good one.

### THE SHELL, BASH 
The shell, within the terminal, is that part of the operating system that will showcases the terminal's behavior and looks after running or executing. While there are various shells available, the most common is called **bash**, which stands for **Bourne again shell.**
To know the shell you are using, use a command called **echo** to display a system variable stating it. 

### SHORTCUTS
Once you have entered a command before, use the up and down arrow keys to go through all. To edit the commands, use the left and right arrow keys.


## Basic Navigation - Let's Explore the System!
Navigation is basically about moving around the system. Most tasks will generally reference or be able to get to the correct system location.  

**PWD**
This stands for **Print Working Directory**
It lets the user know what the current or present working directory is. This command will always tell the user where he is. 

**ls**
Now we know where we are. It is important we know what is in where we are. This is exaclty what the **list** (ls) command does. 
Running list with no arguement as we have shown above will simply output a plain listing of our current location. 
However, there are other ways we could run the list command that will give more powerful outcomes.
_Here are a few examples:_
**ls**
ls in its most basic form will list the contents of our current directory. 
_**ls -l**_
ls with a single line option (-l). This indicates a long listing with various attributes like normal(-) or directory (d); permission for file or directory, number of blocks, owner of the file, group file or directory belongs to, file size, file modification time and actual name of the file or directory. 
_**ls /etc**_
In this case, ls will not list the current directory but will, instead, list that directories contents. 
_**ls -l/etc**_
ls will output a long listing of the directory /etc.

### Paths
This is a means to access a particular file or directory in a system. 

#### Absolute and Relative Paths ####
There are 2 types of paths - **absolute and relative**
In the **linux system,** the filing system is **hierarchical** The **root directory** is at the very top and denoted by a single slash ( / ). Then there are subdirectories and files may reside in any of these directories. 

**Absolute paths** specify a location (file or directory) in relation to the root directory. It is easy to identify them since they usually begins with a forward slash ( / ). 

**Relative paths** specify a location (file or directory) in relation to where we currently are in the system. They will not begin with a slash.

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
Tab completion is simply a mechanism to help us complete the paths we are already typing. It's kind of an auto complete feature.  
















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
