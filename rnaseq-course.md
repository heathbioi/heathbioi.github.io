---
title: "RNAseq Data Processing & Analysing Course"
author: "Alex Gibbs"
full-width: true
---


# THIS PAGE IS UNDER CONSTRUCTION




---
# Course Structure  
---

## Day 1  
---
##### AM Session - 2-3 hours followed by a troubleshooting session

- Basic Unix
- Introduction to HAWK
- Basic Unix continued
- Fetching data with nf-core/fetchngs pipeline

## Day 2
---
##### AM Session - 1-2 hours followed by a troubleshooting session

- Process RNAseq data with nf-core/rnaseq pipeline

## Day 3
---
##### AM Session - 1-2 hours followed by a troubleshooting session

- Analyse processed RNAseq data with nf-core/differentialabundance pipeline

## Day 4
---
##### AM Session - 2-3 hours followed by a troubleshooting session

- Explore outputs and perform further analyses

  
---





---
---

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

#### <span style="color:black;">Course Introduction

---

You should have one of three questions:

- Have you found a nice bulk-RNAseq dataset from a paper and want to download and use it for your research?
- Have you recently generated bulk-RNAseq data and need to process and analyse it?
- You are planning a bulk-RNAseq experiment and would like to know how to process the data when the time comes?

---

#### <span style="color:black;">What you will learn on this course:

- How to find and download sequencing data from online data repositories.
- How to process the sequencing data.
- How to analyse the sequencing data.
- How to interpret the analysed data.

---

#### <span style="color:black;">What you won't learn on this course:

- How RNAseq technology/process works. Please see this [video](https://www.youtube.com/watch?v=tlf6wYJrwKY) for an overview.
- How to hack the mainframe and take over the world.

---

#### <span style="color:black;">Basic Unix: Learning Objectives

- Learn the concept of using the command line.
- Learn how to navigate and manipulate files and data.
- Learn how to run and manage programs.

---

#### <span style="color:black;">Basic Unix: Brief History

- UNIX is a suite of programs that make up an operating system (like Windows and Mac).
- First developed in 1960's and has been in constant development ever since.
- It's a stable, multi-use, multi-tasking system for servers, desktops, and laptops.
- UNIX systems also have a grahpical user interface (GUI), providing an easy to use Windows-like icon-based environment.
- Linux is a clone of UNIX (they're the same thing). UNIX is a commercial product, whereas Linux is open-source (you can download, install, and use it).
- We will be using Linux on this course.

---

#### <span style="color:black;">Basic Unix: Graphical User Interface (GUI) & Command Line/Shell

- All Windows/Mac/Linux PC's use a GUI to allow users to easily navigate and use the PC.
- The GUI is what allows us to point and click on things, which in turn opens the respective programs etc.
- These operations can also be performed using the command line through the use of a shell.

<img src="/assets/img/figure-1.png" alt="Shell" width="1200"/> This is a shell. We can use this to type commands etc.

---

#### <span style="color:black;">Basic Unix: Setup & Installation

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

#### <span style="color:black;">Basic Unix: Setup & Installation: Mac

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

#### <span style="color:black;">Basic Unix: Setup & Installation: Windows

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

#### <span style="color:black;">Introduction to HAWK

- HAWK is Cardiff and Bangor universities High Performance Compute (HPC) system.
- Swansea and Aberystwyth universities use SunBird - both systems are the run by Supercomputing Wales (SCW).
- Both HPC's are the same, but are set-up slightly different - we will be working with HAWK.
- If we need to run analyses/softwares/code that requires a lot of computing power, we need to use HPC's.
- The way we interact with HAWK is through the command line via Bash.
- Think of HAWK as a computer that's located in the cloud. We can connect to it via out Unix shells - Terminal, MobaXterm, and FileZilla.

---

#### <span style="color:black;">Introduction to HAWK: HAWK Filesystem

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

#### <span style="color:black;">Basic Unix Continued: Common Commands

  
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
#### <span style="color:black;">Basic Unix Continued: Command line Syntax

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

#### <span style="color:black;">Basic Unix Continued: Exploring Using Unix
- Lets cover the three most basic (and used) commands:
  - `pwd` = Where am I?
  - `ls` = List
  - `cd` = Change directory
    
---

##### <span style="color:black;">Basic Unix Continued: pwd Command
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

##### <span style="color:black;">Basic Unix Continued: ls Command
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

##### <span style="color:black;">Basic Unix Continued: cd Command
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

##### <span style="color:black;">Basic Unix Continued: Other Notations
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

-For example, if I am currently in the Desktop directory and want to list contents of where I currently am, I can either use `ls` or `ls .`:

**Input**
```
ls
ls .
```

**Output**
<img src="/assets/img/ls-ls.dot.gif" alt="ls" width="1000"/>









 To move between different directories, we use the `cd` command.
- In the example below,  we move into the plan to take over the world directory.
- **Note:** we can use the tab-key to autofill. Start typing the name of the directory and then hit tab.
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




























#### <span style="color:black;">Header Title 




```
this should be a chunk of code
```
![Text](/assets/img/figure-.png) This is a shell. We can use this to type commands etc.

