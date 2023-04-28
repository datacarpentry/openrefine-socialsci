---
title: Setup
---

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


::::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::  prereq

## Software

For this lesson you will need **OpenRefine** (formerly Google Refine) and a
web browser. Basic installation steps are provided on this page.
The OpenRefine [installation manual](https://openrefine.org/docs/manual/installing)
provides more details about installation, upgrades and configuration.

Note: this is a Java program that runs on your machine (not in the cloud).
It runs inside your browser, but no web connection is needed for this lesson.

:::::::::::::::::::::::::::::::::::::::::  callout

You do not need administrative rights on the computer to *install* OpenRefine.
However, if anti-malware software blocks OpenRefine when you try to start it,
you may need administrative rights to allow OpenRefine to *run*.
OpenRefine is safe to run.


::::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::::::

### Windows

- Check that you have Firefox, Edge, Opera or Chrome browsers installed and set
  as your default browser. OpenRefine runs in your default browser. It will not
  run correctly in Internet Explorer.
- Download the software from [openrefine.org](https://openrefine.org).
- Unzip the downloaded file into a directory by right-clicking and
  selecting "Extract…". Name that directory something like OpenRefine.
  :::::::::::::::::::::::::::::::::::::::::  callout
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


