---
title: "RNAseq Data Processing & Analysing Course"
author: "Alex Gibbs"
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

# Day 1

---
---

We will cover:

- Introduction to course.
- Basic Unix.
- Introduction to HAWK.
- Basic Unix Continued.
- Fetch data with nf-core/fetchngs pipeline.

---

#### Course Introduction

---

You should have one of three questions:

- Have you found a nice bulk-RNAseq dataset from a paper and want to download and use it for your research?
- Have you recently generated bulk-RNAseq data and need to process and analyse it?
- You are planning a bulk-RNAseq experiment and would like to know how to process the data when the time comes?

---

#### What you will learn on this course:

- How to find and download sequencing data from online data repositories.
- How to process the sequencing data.
- How to analyse the sequencing data.
- How to interpret the analysed data.

---

#### What you won't learn on this course:

- How RNAseq technology/process works. Please see this [video](https://www.youtube.com/watch?v=tlf6wYJrwKY) for an overview.
- How to hack the mainframe and take over the world.

---

#### Basic Unix: Learning Objectives

- Learn the concept of using the command line.
- Learn how to navigate and manipulate files and data.
- Learn how to run and manage programs.

---

#### Basic Unix: Brief History

- UNIX is a suite of programs that make up an operating system (like Windows and Mac).
- First developed in 1960's and has been in constant development ever since.
- It's a stable, multi-use, multi-tasking system for servers, desktops, and laptops.
- UNIX systems also have a grahpical user interface (GUI), providing an easy to use Windows-like icon-based environment.
- Linux is a clone of UNIX (they're the same thing). UNIX is a commercial product, whereas Linux is open-source (you can download, install, and use it).
- We will be using Linux on this course.

---

#### Basic Unix: Graphical User Interface (GUI) & Command Line/Shell

- All Windows/Mac/Linux PC's use a GUI to allow users to easily navigate and use the PC.
- The GUI is what allows us to point and click on things, which in turn opens the respective programs etc.
- These operations can also be performed using the command line through the use of a shell.

![Shell](/assets/img/figure-1.png) This is a shell. We can use this to type commands etc.

---

#### Basic Unix: Setup & Installation

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

#### Basic Unix: Setup & Installation: Mac

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

![FileZilla Log-in](/assets/img/figure-2.png)

---

#### Basic Unix: Setup & Installation: Windows

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

#### Introduction to HAWK

- HAWK is Cardiff and Bangor universities High Performance Compute (HPC) system.
- Swansea and Aberystwyth universities use SunBird - both systems are the run by Supercomputing Wales (SCW).
- Both HPC's are the same, but are set-up slightly different - we will be working with HAWK.
- If we need to run analyses/softwares/code that requires a lot of computing power, we need to use HPC's.
- The way we interact with HAWK is through the command line via Bash.
- Think of HAWK as a computer that's located in the cloud. We can connect to it via out Unix shells - Terminal, MobaXterm, and FileZilla.

---

#### Introduction to HAWK: HAWK Filesystem

- Like our own PC's, HAWK has its own files and folder structure.
- From here, we will now refer to folders as **directories**.
- The basic structure of HAWK:

![Basic HAWK Structure](/assets/img/figure-3.png)

- We have two main directories: *home* and *scratch*.

- **home directory (green)**
  - This is where we are located when we log into HAWK.
  - Has limited long-term storage.
  - **DO NOT WORK HERE!**  
  <br>
- **scratch directory (red)**
  - This is where we perform our compute-heavy analyses.
  - Not for long-term storage! Files are deleted after 60-days.
  - Do your work, then move your files back to home directory or to another storage location such as the Research Data Store (RDS).

---

#### Basic Unix Continued: Common Commands

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
#### Basic Unix Continued: Command line Syntax

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

---

**Options**
- The `-lah` options will print a list in long format which will be human readable and show hidden files.

---

**Argument**
- The argument gives the system the required input, these are usually files or directories
- The `.` argument means 'here' or where I currently am. We will cover this shortly.

---

- Not all commands have options, and most commands have optional options - you don't have to use them!

---

#### Basic Unix Continued: Exploring Using Unix
- Lets cover the three most basic (and used) commands:
  - `pwd` = Where am I?
  - `ls` = List
  - `cd` = Change directory
    
---

##### pwd Command
- When we first open a Unix shell, we are taken to the default directory.
- If you have downloaded a shell (such as iTerm2, MobaXterm, FileZilla), this location can change depending on where you installed the software.
- To find out where we are currently located, we can use the `pwd` command:

---

**Input**
```
pwd
```

---

**Output**
```
/Users/alexgibbs/Desktop`
```

---






#### Exercise: 




```
this should be a chunk of code
```
![Text](/assets/img/figure-.png) This is a shell. We can use this to type commands etc.

