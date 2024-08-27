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
### AM Session - 2-3 hours followed by a troubleshooting session

- Basic Unix
- Introduction to HAWK
- Basic Unix continued
- Fetching data with nf-core/fetchngs pipeline

## Day 2
---
### AM Session - 1-2 hours followed by a troubleshooting session

- Process RNAseq data with nf-core/rnaseq pipeline

## Day 3
---
### AM Session - 1-2 hours followed by a troubleshooting session

- Analyse processed RNAseq data with nf-core/differentialabundance pipeline

## Day 4
---
### AM Session - 2-3 hours followed by a troubleshooting session

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

### Course Introduction

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

Connecting to the VPN

- The VPN runs automatically after installation.
- Enter the portal address as *ras.cf.ac.uk*
- Enter your university username and password.
- Click *OK* when prompted to allow GlobalProtect access to your Desktop, Documents, and Downloads folders (three prompts).

---









```
this should be a chunk of code
```

