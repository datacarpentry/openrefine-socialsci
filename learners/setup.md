---
title: Setup
---

::: instructor

## Install and run before workshop

Participants should install and run before the workshop, so that any problems
may reveal themselves early.

::::::::::::::

::::::::::::::::::::::::::::::::::::::::::  prereq

## Data

The data for this lesson is a part of the Data Carpentry Social Sciences
workshop. It is a teaching version of the Studying African Farmer-Led
Irrigation (SAFI) database. The SAFI dataset represents interviews of farmers
in two countries in eastern sub-Saharan Africa (Mozambique and Tanzania).
These interviews were conducted between November 2016 and June 2017 and probed
household features (e.g. construction materials used, number of household
members), agricultural practices (e.g. water usage), and assets (e.g. number
and types of livestock).

The data used in this lesson
is a subset of the teaching version that has been intentionally 'messed up'
for this lesson.

[**Download** the data file](https://ndownloader.figshare.com/files/11502815)
to your computer.

::: instructor

### About the data

A general description of the dataset used in the Social Sciences lessons can
be found [in the workshop data home page](https://www.datacarpentry.org/socialsci-workshop/data/).

::::::::::::::


::: instructor

### Import from URL

Instead of downloading the data to the computer, you could import the data from
the URL directly when you start the project.
When learners have trouble finding the file on their computer, this may be a
workaround to not have to wait.

::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::  prereq

## Software

For this lesson you will need **OpenRefine** (formerly Google Refine) and a
web browser. Basic installation steps are provided on this page.
The OpenRefine [installation manual](https://openrefine.org/docs/manual/installing)
provides more details about installation, upgrades and configuration.

Note: this is a Java program that runs on your machine (not in the cloud).
It runs inside your browser, but no web connection is needed for this lesson.

::::::::::::::::::::::::::::::::::::::  callout

### Administrator rights

You do not need administrative rights on the computer to *install* OpenRefine.
However, if anti-malware software blocks OpenRefine when you try to start it,
you may need administrative rights to allow OpenRefine to *run*.
OpenRefine is safe to run.

:::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::::::

::: instructor

### Long startup duration

Starting OpenRefine may take minutes, even on some modern computers.
Learners may be wondering if it is actually working; if there are no error messages,
it is probably still starting up and you should wait a little longer.

::::::::::::::

### Windows

 - Check that you have Firefox, Edge, Opera or Chrome browsers installed and set
   as your default browser. OpenRefine runs in your default browser. It will not
   run correctly in Internet Explorer.
 - Download the software from [openrefine.org](https://openrefine.org).
 - Unzip the downloaded file into a directory by right-clicking and
   selecting "Extract…". Name that directory something like OpenRefine.
   
   :::::::::::::::::::::::::::::::::::::::::  callout

   #### Long paths

   The path to the directory you extract the application files into should be
   short, because some of OpenRefine's files have very long names. If the path is
   too long, OpenRefine cannot start.
   
   ::::::::::::::::::::::::::::::::::::::::::::::::::
   
 - Go to your newly created OpenRefine directory.
 - Launch OpenRefine by opening `openrefine.exe`. This will launch a command prompt window,
   but you can ignore that and wait for the browser to launch.
 - If you see Internet Explorer start, or OpenRefine does not automatically
   open for you, point one of the supported browsers at [http://127.0.0.1:3333/](https://127.0.0.1:3333/) or
   [http://localhost:3333](https://localhost:3333) to launch the program.

### Mac

 - Check that you have Firefox, Edge, Opera or Chrome browsers installed and set as your
   default browser. OpenRefine runs in your default browser. It will not run
   correctly in Internet Explorer.
 - Download the software from [openrefine.org](https://openrefine.org).
 - Unzip the downloaded file into a directory by double-clicking it. Name
   that directory something like OpenRefine.
 - Go to your newly created OpenRefine directory.
 - Drag the OpenRefine app into the Applications folder.
 - Launch OpenRefine: Control-click the app icon, then
   choose "Open" from the shortcut menu. For Troubleshooting help, see
   [the Apple support page](https://support.apple.com/guide/mac-help/open-a-mac-app-from-an-unidentified-developer-mh40616/mac).
 - If you are using a different browser than listed above, or if OpenRefine does not automatically
   open for you, point your browser at [http://127.0.0.1:3333/](https://127.0.0.1:3333/) or
   [http://localhost:3333](https://localhost:3333) to launch the program.

### Linux

 - Check that you have Firefox or Chrome browsers installed and set as your
   default browser. OpenRefine runs in your default browser.
 - Download the software from [openrefine.org](https://openrefine.org).
 - Unzip the downloaded file into a directory. Name that directory something like OpenRefine.
 - Go to your newly created OpenRefine directory.
 - Launch OpenRefine by typing `./refine` into the terminal within the OpenRefine directory.
 - If you are using a different browser than listed above, or if OpenRefine does not automatically
   open for you, point your browser at [http://127.0.0.1:3333/](https://127.0.0.1:3333/) or
   [http://localhost:3333](https://localhost:3333) to launch the program.

### Exiting OpenRefine

To exit OpenRefine, close all the browser tabs or windows, then navigate to the command line window. 
To close this window and ensure OpenRefine exits properly, hold down [control] and press [c] on your keyboard. 
This will save all changes to your projects.  

Remember, it's important to close the browser window or tab first to ensure you're not actively using OpenRefine 
before stopping the server. This prevents any unsaved changes from being lost. After stopping the server, you can 
safely exit the terminal or command prompt window.
