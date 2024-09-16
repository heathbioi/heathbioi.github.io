---
title: "RNAseq Data Processing & Analysing Course"
author: "Alex Gibbs"
full-width: true
---


# THIS PAGE IS UNDER CONSTRUCTION




---
# <span style="color:black;">Course Structure  
---

<br>

## <span style="color:black;">Day 1  
---
##### <span style="color:black;">AM Session - 2-3 hours followed by a troubleshooting session

- Basic Unix
- Introduction to HAWK
- Basic Unix continued
- Fetching data with nf-core/fetchngs pipeline

---

<br>

## <span style="color:black;">Day 2
---
##### <span style="color:black;">AM Session - 1-2 hours followed by a troubleshooting session

- Process RNAseq data with nf-core/rnaseq pipeline

---

<br>

## <span style="color:black;">Day 3
---
##### <span style="color:black;">AM Session - 1-2 hours followed by a troubleshooting session

- Analyse processed RNAseq data with nf-core/differentialabundance pipeline

---

<br>

## <span style="color:black;">Day 4
---
##### <span style="color:black;">AM Session - 2-3 hours followed by a troubleshooting session

- Explore outputs and perform further analyses
  
---

<br>
<br>

# <span style="color:black;">Day 1

---
---

We will cover:

- Introduction to course.
- Basic Unix.
- Introduction to HAWK.
- Basic Unix Continued.
- Fetch data with nf-core/fetchngs pipeline.

---

<br>

---
## <span style="color:black;">Course Introduction

You should have one of three questions:

- Have you found a nice bulk-RNAseq dataset from a paper and want to download and use it for your research?
- Have you recently generated bulk-RNAseq data and need to process and analyse it?
- You are planning a bulk-RNAseq experiment and would like to know how to process the data when the time comes?

---

<br>

---

## <span style="color:black;">What you will learn on this course:

- How to find and download sequencing data from online data repositories.
- How to process the sequencing data.
- How to analyse the sequencing data.
- How to interpret the analysed data.

---

<br>

---

## <span style="color:black;">What you won't learn on this course:

- How RNAseq technology/process works. Please see this [video](https://www.youtube.com/watch?v=tlf6wYJrwKY) for an overview.
- How to hack the mainframe and take over the world.

---

<br>

---

## <span style="color:black;">Basic Unix: Learning Objectives

- Learn the concept of using the command line.
- Learn how to navigate and manipulate files and data.
- Learn how to run and manage programs.

---

<br>

---

## <span style="color:black;">Basic Unix: Brief History

- UNIX is a suite of programs that make up an operating system (like Windows and Mac).
- First developed in 1960's and has been in constant development ever since.
- It's a stable, multi-use, multi-tasking system for servers, desktops, and laptops.
- UNIX systems also have a grahpical user interface (GUI), providing an easy to use Windows-like icon-based environment.
- Linux is a clone of UNIX (they're the same thing). UNIX is a commercial product, whereas Linux is open-source (you can download, install, and use it).
- We will be using Linux on this course.

---

<br>

---

## <span style="color:black;">Basic Unix: Graphical User Interface (GUI) & Command Line/Shell

- All Windows/Mac/Linux PC's use a GUI to allow users to easily navigate and use the PC.
- The GUI is what allows us to point and click on things, which in turn opens the respective programs etc.
- These operations can also be performed using the command line through the use of a shell.

<img src="/assets/img/figure-1.png" alt="Shell" width="1200"/> 
This is a shell. We can use this to type commands etc.

---

<br>

---

## <span style="color:black;">Basic Unix: Setup & Installation

- Before we cover installation of Unix on your PC's, we first need to install the universities VPN.
- We will need to have the Global Protect VPN installed on our PC's in order to connect to HAWK off campus.

--- 
For **MAC:**

  - Use this [link](https://software.cardiff.ac.uk) and log in to the Software Downloads website with your university log in.
  - Then click on *Global Protect*, then click the *MAC OS* link, then click on the *GlobalProtect-6.2.4.pkg* download button to initiate the download to your PC.
  - Once the file has downloaded, navigate to it and double-click on it to initiate installation onto your PC.
  - Navigate through the installer by clicking *Continue*.
  - Check boxes for *GlobalProtect* and *GlobalProtect System Extensions* and click *Continue*.
  - Click *Install*.
  - Enter your admin password when prompted and click *Install Software*.
  - Click *Close* once the installation has completed.
  - When prompted, choose to *Allow* the system extension in Security and Privacy preferences.
  - Click on the system notification to Allow notifications from GlobalProtect.


---
For **Windows:**
  
  - Use this [link](https://software.cardiff.ac.uk) and log in to the Software Downloads website with your university log in.
  - Then click on *Global Protect*, then click the *Windows* link, then click on the 32- or 64-bit client link. To find out what bit your system is, go to Control Panel > System and Security > System. In the System area, the System Type shows if the system is 32 bit or 64 bit.
  - Now click on the *GlobalProtect64-6.2.4.msi* download button to initiate the download to your PC.
  - Click *Run* to start installation. Accept any browser security messages if they pop up.
  - Click *Next* in the setup wizard and accept the default installation folder on your PC.
  - Click *Next* to install the Agent in the default location in *Program Files*.
  - Click *Next* to continue with the installation.
  - You will be notified once installation has completed, click *Close* to finish.
    
---

**Connecting to the VPN:**

- The VPN runs automatically after installation.
- Enter the portal address as *ras.cf.ac.uk*
- Enter your university username and password.
- Click *OK* when prompted to allow GlobalProtect access to your Desktop, Documents, and Downloads folders (three prompts).

---

<br>

---

## <span style="color:black;">Basic Unix: Setup & Installation: Mac

- Mac users have a built-in Unix shell called bash. To open this, open the *Terminal* application/program.
- To transfer files to- and from the HAWK servers that we will be using, we can either use code in Terminal (advanced use), or use a file transfer program (FTP) called FileZilla.

**FileZilla Installation**

- Search for *FileZilla* on Google, or follow this [link](https://filezilla-project.org/download.php?type=client).
- Click on the *Download FileZilla Client* button to initiate the download.
- Once downloaded, double-clicking on the downloaded file will initiate installation.
- Once installed, open the software.

**To connect to HAWK:**

- Host: **hawklogin.cf.ac.uk**
- Username: **c.c123456**  (Your HAWK account username)
- Password: **XXXXXXX**  (Your HAWK account password)
- Once connected, you will see that you have two connections.
- Your PC files and folders are on the left box.
- Your HAWK files and folders are on the right box.
- **To transfer files, simply drag and drop from one side to the other.**
- You can also double-click on the respective folders to navigate to wherever you want to be.

<img src="/assets/img/figure-2.png" alt="FileZilla Log-in" width="1200"/>

---

<br>

---

## <span style="color:black;">Basic Unix: Setup & Installation: Windows

- Windows users don't have an integrated Unix shell, so you will need to download and install one. We will use **MobaXterm**.
- MobaXterm is an integrated shell, which combines command line with FTP all in one window/application.
- 
- Mac users have a built-in Unix shell called bash. To open this, open the *Terminal* application/program.
- To transfer files to- and from the HAWK servers that we will be using, we can either use code in Terminal (advanced use), or use a file transfer program (FTP) called FileZilla.

**MobaXterm Installation**

- Search for *MobaXterm* on Google, or follow this [link](https://mobaxterm.mobatek.net/download.html).
- Click on the *Download Now* button on the Home Edition version to initiate the download.
- Once downloaded, click *Run* to initiate installation.
- Once installed, open the software.

# THIS BIT NEEDS COMPLETING

---

<br>

---

## <span style="color:black;">Introduction to HAWK

- HAWK is Cardiff and Bangor universities High Performance Compute (HPC) system.
- Swansea and Aberystwyth universities use SunBird - both systems are the run by Supercomputing Wales (SCW).
- Both HPC's are the same, but are set-up slightly different - we will be working with HAWK.
- If we need to run analyses/softwares/code that requires a lot of computing power, we need to use HPC's.
- The way we interact with HAWK is through the command line via Bash.
- Think of HAWK as a computer that's located in the cloud. We can connect to it via out Unix shells - Terminal, MobaXterm, and FileZilla.

---

<br>

---

## <span style="color:black;">Introduction to HAWK: HAWK Filesystem

- Like our own PC's, HAWK has its own files and folder structure.
- From here, we will now refer to folders as **directories**.
- The basic structure of HAWK:

<img src="/assets/img/figure-3.png" alt="Basic HAWK Structure" width="1200"/>

- We have two main directories: <span style="color: green;">*home*</span> and <span style="color: red;">*scratch*.

- <span style="color: green;">**home directory**
  - This is where we are located when we log into HAWK.
  - Has limited long-term storage.
  - **DO NOT WORK HERE!**  
  <br>
- <span style="color: red;">**scratch directory**
  - This is where we perform our compute-heavy analyses.
  - Not for long-term storage! Files are deleted after 60-days.
  - Do your work, then move your files back to home directory or to another storage location such as the Research Data Store (RDS).

---

<br>

---

## <span style="color:black;">Basic Unix Continued: Common Commands
 
- Now that we have covered basic Unix and introduced HAWK, we can now learn how to use the command line.

- Here is a list of commonly used Unix commands that we will be using:
  

Command|Description|Common Options|Option Description
|:----:|:----------|:-----------|:--------------|
`ls`|print directory contents|`ls -lah`|list that is long, shows hidden files, and is human-readable
`mv`|rename/move a file|`mv -r/*`|moves recursively (moves a directory and everything inside)/moves everything
`cp`|copy a file|`cp -r/*`|copies recursively (copies a directory and everything inside)/copies everything
`cd`|change directory||
`pwd`|where am I?||
`history`|what have I typed?||
`rm`|remove a file|`rm -r/*`|removes recursively (removes a directory and everything inside)/removes everything
`mkdir`|make a directory||
`touch`|make an empty file||
`nano`|open and edit a file||
`more/less`|reads a file||
`head`|read the top of a file||
`tail`|read the bottom of a file||
`wc`|count the number of lines in a file||
`grep`|word search in a file||
`chmod`|change permission of a file|`chmod +x`|makes file executable

---

<br>

---

## <span style="color:black;">Basic Unix Continued: Command line Syntax

Syntax = Structure of statements in a computing language.

"I like computers" - pronoun, verb, noun

`ls -lah .` - command, options, arguments

- `ls` = list command
- `-lah` = options for the list command
- `.` = argument for the list command

**All commands are case sensitive!**

---

**Command**
- The `ls` command will list/print the files and directories in your current directory.

<br>

**Options**
- The `-lah` options will print a list in long format which will be human readable and show hidden files.

<br>

**Argument**
- The argument gives the system the required input, these are usually files or directories
- The `.` argument means 'here' or where I currently am. We will cover this shortly.

---

Not all commands have options, and most commands have optional options - you don't have to use them!

---

<br>

## <span style="color:black;">Basic Unix Continued: Exploring Using Unix

- Lets cover the three most basic (and used) commands:
  - `pwd` = Where am I?
  - `ls` = List
  - `cd` = Change directory
    
---

<br>

---

## <span style="color:black;">Basic Unix Continued: pwd Command

- When we first open a Unix shell, we are taken to the default directory.
- If you have downloaded a shell (such as iTerm2, MobaXterm, FileZilla), this location can change depending on where you installed the software.
- To find out where we are currently located, we can use the `pwd` command.
- In the example below, the pwd output tells me that I am in my Desktop directory.

**Input**
```
pwd
```

**Output**
```
/Users/alexgibbs/Desktop
```

<img src="/assets/img/pwd.gif" alt="pwd" width="1000"/>

---

<br>

---

## <span style="color:black;">Basic Unix Continued: ls Command

- To explore the directory, we can use the `ls` command to list the contents of the Desktop directory:

**Input**
```
ls
```

**Output**
```
IGV_2.8.10.app  plan-to-take-over-the-world  Why is multiple t-testing a problem?.pdf
```

<img src="/assets/img/ls.gif" alt="ls" width="1000"/>

- To see this list in a long format, we can use the `-l` option.
- To see hidden contents, we can use the `-a` option.
- To see the contents in a human-readable format, we can use the `-h` option.
- In the example below, we combine both options to return a long, hidden, and human-readable list of contents:

**Input**
```
ls -lah
```

**Output**

<img src="/assets/img/figure-4.png" alt="ls" width="1000"/>

- We will cover permission shortly

<br>

<img src="/assets/img/ls-lah.gif" alt="ls" width="1000"/>

- Any file or directory with a dot (.) in front makes it hidden.
- Hidden files are usually filesystem files and directories required by the system to correctly operate and function.
- These hidden files are not normally needed by the user. \
- In this course, we will potentially need to access a hidden file if things go wrong.

---

<br>

---

## <span style="color:black;">Basic Unix Continued: cd Command

- To move between different directories, we use the `cd` command.
- In the example below,  we move into the plan to take over the world directory.
- **Note:** we can use the `tab-key` to autofill. Start typing the name of the directory and then hit tab.
- Note: when we use the `cd` command, we don't get any feedback from the shell. Usually, we move into the directory, then use the `ls` command to show us the contents.

**Input**
```
cd plan-to-take-over-the-world
ls
```

**Output**
```
gantt-chart.pdf  top-secret-map.pdf
hit-list.docx  villain-cape-designs.ppt
how-to-attach-lasers-to-sharks.docx  world-takeover-ticklist.pdf
script-to-steal-all-the-money-in-the-UK.sh
```

<img src="/assets/img/cd-ls.gif" alt="ls" width="1000"/>

---

<br>

---

## <span style="color:black;">Basic Unix Continued: Other Notations

**Tab-key**
- As mentioned above, we can use the `tab-key` to autofill.
- This will save you time and lots of errors! The `tab-key` is your friend!

**Making Use Of The Dot(.)**
- As mentioned above, the dot(.) is used to tell the system where you currently are.
- This is best used for commands such as `ls` and `cd`.
- When we combine two dots(..), this tells the system to use the directory above where we currently are.

Input|Description
-----|-----------
.|Here/where I am now
..|Previous directory/up one directory

-For example, if I am currently in the Desktop directory and want to list contents of where I currently am, I can either use `ls` or `ls .`

**Input**
```
ls
ls .
```

**Output**

<img src="/assets/img/ls-ls.dot.gif" alt="ls" width="1000"/>

- If I wanted to see what contents were above/outside of my Desktop, I would use `ls ..`

**Input**
```
ls ..
```

**Output**

<img src="/assets/img/ls.dot.dot.gif" alt="ls" width="1000"/>

**Wildcard (*)**
- The wildcard (*) can be used to select multiple things at once.
- It is used to match any character and is commonly used to select directories/files with common names.
- Example, if there are multiple directories (file-1 through file-10) and I wanted to move them all into one directory (dir-1), I could use the common name to all the files followed by the wildcard.
- `mv file* dir-1/`
- The wildcard can also be used to select the same file extensions. Example: If we wanted to move all the .fastq files to a new directory, we would use the wildcard followed by the extension.
- `mv *.fastq dir-1/`

**Input**
```
ls
mv file* dir-1/
ls dir-1/
mv *.fastq dir-1/
ls dir-1/
```

**Output**

<img src="/assets/img/wildcard.gif" alt="Wildcard" width="1000"/>

---

<br>

---

## <span style="color:black;">Basic Unix Continued: Working Example

- To give a visual explanation of what we have covered so far, let's use the HAWK directory structure that I made up:

- I have just logged into my HAWK account and am not sure where I am located. To find out, I used the `pwd` command. This tells me that I am in the home directory:

**Input**
```
pwd
```

**Output**
```
/home/steve
```

<img src="/assets/img/figure-5.png" alt="ls" width="1000"/>

- One of the SCW administrators told me that a few users had used my account for training purposes and stored some files etc. Lets first see if the users made a directory in the home directory:

**Input**
```
ls ..
```

- This command lists the contents in the directory above mine, i.e. lists the contents of the home directory

**Output**
```
karen  steve  terry
```

<img src="/assets/img/figure-6.png" alt="ls" width="1000"/>

- I decided to look at what Karen had been up to in the home directory.
- Theres two ways to do this, <span style="color:red;">either move into her directory and list the contents</span>, <span style="color:green;">or use the list command</span>.

**Input**
```
ls ../karen
```

**OR**

```
cd ../karen
ls
```
- **Note**: As I am still in my directory, I need to use the two dots (..) to move up/out and then into Karens directory.

**Output**

<img src="/assets/img/figure-7.png" alt="ls" width="1000"/>


# This Needs To Be Completed!

---

<br>

---

## <span style="color:black;">Basic Unix Continued: File Permissions & File Privacy

- File permissions determine who can and who can't access certain files and directories.
- On HAWK, each user has their own account which comes with their own home and scratch directory.
- These directories can only be accessed by the user (and the admins). Other users can see that you have a directory, but cannot access as they do not have permission to do so.
- To see the file and directory permissions, we must first understand how the permissions are ordered.
- Unix splits file permission into three sections:
  

Section|Description
-------|-----------
user|The file/directory owner
group|A group of individuals permitted to read the file
other|Everyone

<img src="/assets/img/figure-8.png" alt="File Permissions" width="1000"/>

Symbol|Meaning
------|-------
-/d|file/directory
u/g/o|user/group/other
+/-|enable/disable
r/w/x|read/write/execute

- The group section enables group access to files and directories.
- When we run scripts, we need to make sure they are executable (x), otherwise the system will not recognise it as an executable file.
- To check if a file is executable, we can use the `ls -l` command and check the permissions.

**Changing File Permissions**

- A good example for changing file permissions is to make a script executable.
- In the example below, I have made a shell script named file-permission.sh
- These types of files (.sh) are what we use to run a script on Unix. These scripts can range from a simple one liner task, to a list of tasks that will run sequentially.
- When we create a file using the `touch` or `nano` command, by default it is not executable, as denoted by `-rw-r--r--`. We will cover `nano` shortly.
- Subsequently, the system does not recognise it as an executable file and you wont be able to run it.
- To change the file permissions and make the file executable, we use the `chmod` command.
- If we wanted to change the permission for just the user (u), we would use `chmod u+x`.
- Using `chmod +x` on the file makes the file executable (x) for everyone (u/g/o).

**Input**
```
touch file-permission.sh
ls -l
chmod +x file-permission.sh
ls -l
```

<img src="/assets/img/permissions.gif" alt="File Permissions" width="1000"/>

---

<br>

---

## <span style="color:black;">Basic Unix Continued: Moving & Copying Files

- We sometimes will want to copy or move files from one directory to another.
- An example of this would be copying a reference genome from our home directory (long term storage) to our scratch directory for an analysis.

---

<br>

---

## <span style="color:black;">Basic Unix Continued: Copying a file using `cp` command

- The copy command does what it says on the tin... Copies a file/directory from one place to another.

**Input**
```
cp name-of-file.txt path/to/directory/
```

<img src="/assets/img/cp.gif" alt="Copying a File" width="1000"/>

- The command works by first inputting the name of the file/directory that you want to copy, followed by the location of where you want to copy it to.
- To copy a directory, we need to use the `-r` option:

**Input**
```
cp -r name-of-directory path/to/directory/
```

<img src="/assets/img/cp-r.gif" alt="Copying a Directory" width="1000"/>

- To state the obvious, this command makes a copy of the file at the destination that you have chosen.

---

<br>

---

## <span style="color:black;">Basic Unix Continued: Moving a file using `mv` command

- The move command does what it says on the tin... Moves a file/directory from one place to another.

**Input**
```
mv name-of-file.txt path/to/directory/
mv name-of-directory path/to/directory/
```

<img src="/assets/img/mv-file.gif" alt="Moving a File" width="1000"/>

<img src="/assets/img/mv-directory.gif" alt="Moving a Directory" width="1000"/>

- The command works by first inputting the name of the file/directory that you want to move, followed by the location of where you want to move it to.
- **Note**: This command physically moves the file/directory to the location you have chosen. Be aware of typos when using this command, as it is very easy to overwrite other files/directories!
- **I would reccomend sticking to using the cp command when you want to move files just in case you make typos**
- The `mv` command can also be used to rename a file/directory:

**Input**
```
mv name-of-file.txt new-name-of-file.txt
mv name-of-directory new-name-of-directory
```

<img src="/assets/img/renaming.gif" alt="Renaming a File/Directory" width="1000"/>

---

<br>

---

## <span style="color:black;">Basic Unix Continued: Making a file

- To make a file, we can use the `touch` command.
- We don't need to use this command for the course, but for completeness (and for the task ahead) we will cover it.

**Input**
```
touch name-of-file.extension.name
```
<img src="/assets/img/touch.gif" alt="Making an empty file" width="1000"/>

- The command works by calling the `touch` command followed by the name and extension of the file you want to create.
- To make a file named `myFile.txt`, we would use `touch myFile.txt`.

---

<br>

---

## <span style="color:black;">Basic Unix Continued: Editing a file

- To edit a file in Unix, we can use an editor called nano.
- The nano editor opens a new window within the Unix shell whilst in use, and then returns you to where you was once you have exited the editor.
- To use the editor, we simply use the `nano` command.
- The editor can be used to create new files and also edit existing files.
- If we wanted to create a new file, we would use `nano name-of-new-file.extension.name`.
- Likewise, if we wanted to edit an existing file, we would use `nano name-of-existing-file-extension.name`.
- **To exit the nano editor, use `ctrl + x`, then `y` to save, then `enter` to exit.**

**Input**
```
nano myFile.txt
this is some simple text that I want to put into the file.
this another simple line of text to include.
ctrl + x
y
enter
```

<img src="/assets/img/nano.gif" alt="Making and editing a file with nano" width="1000"/>

- Along the bottom of the editor, you can see the various options that you are able to use.
- Once we use `ctrl + x` you can see the bottom of the editor changes to `save modified buffer?`. Typing `Y` saves the file, `N` deletes it.
- Once you have hit `Y`, you get another prompt to check the file name. Here, you get the opportunity to rename the file if needed. Then hitting `enter` saves and exits the editor. 

---

<br>

---

## <span style="color:black;">Basic Unix Continued: Making a directory

- To make a directory, we can use the `mkdir` command.

**Input**
```
mkdir name-of-directory
```
- The command works by calling the `mkdir` command  followed by the name of the directory you want to make.
- We can use this command to make multiple directories within the current directory, too:

**Input**
```
mkdir directory1 directory2 directory3
```
- Each new directory is named after the other and is separated by a space whilst using the command.
- We can also create a new directory within an existing directory without moving into it:

**Input**
```
mkdir directory1/directory1.1
```
- The `touch` command can also be used in this manner.

<img src="/assets/img/mkdir.gif" alt="Making a directory" width="1000"/>

---

<br>

---

## <span style="color:black;">Exercise 1
- Open a shell on your PC



<details>
<summary>Answer</summary>
<br>

Find out where you are: `pwd`
List contents: `ls`
Change directory: `cd unix-practical`
```bash
pwd
ls
cd unix-practical
ls
```
</details>















<br>

---

##### <span style="color:black;">Example Title 

# Email out a directory with files etc in there and tell them do cd into it and then ls and make files etc etc
- Now that we have covered the basics


- The move command does what it says on the tin... Moves a file/directory from one place to another.

**Input**
```
mv name-of-file.txt path/to/directory/
mv name-of-directory path/to/directory/
```

---

<br>












