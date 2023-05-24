---
title: Introduction
teaching: 10
exercises: 0
---

::::::::::::::::::::::::::::::::::::::: objectives

- Describe OpenRefine’s uses and applications.
- Differentiate data cleaning from data organization.
- Experiment with OpenRefine’s user interface.
- Locate helpful resources to learn more about OpenRefine.

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- What is OpenRefine useful for?

::::::::::::::::::::::::::::::::::::::::::::::::::

::::: instructor

## Please help improve this page

There are several issues related to this section of the lesson:

- [the goals of the (whole) lesson should be stated (#38)][issue-38]
- [it does not explain the difference between data cleaning and data organisation (#56)][issue-56]
- [the contents do not match the objectives (#86)][issue-86]
- [it does not explain when (not) to use OpenRefine (#103)][issue-103]
- [the Getting Help section should move to the end or an Extras page (#122)][issue-122]

[issue-38]: https://github.com/datacarpentry/openrefine-socialsci/issues/38
[issue-56]: https://github.com/datacarpentry/openrefine-socialsci/issues/56
[issue-86]: https://github.com/datacarpentry/openrefine-socialsci/issues/86
[issue-103]: https://github.com/datacarpentry/openrefine-socialsci/issues/103
[issue-122]: https://github.com/datacarpentry/openrefine-socialsci/issues/122

Your input on these issues would be much appreciated!

::::::::::::::::

## Motivations for the OpenRefine Lesson

- Data is often very messy. OpenRefine provides a set of tools to allow you to
  identify and amend the messy data.
- It is important to know what you did to your data. Additionally, journals,
  granting agencies, and other institutions are requiring documentation of the
  steps you took when working with your data. With OpenRefine, you can capture
  all actions applied to your raw data and share them with your publication as
  supplemental material.
- All actions are easily reversed in OpenRefine.
- If you save your work it will be to a new file. OpenRefine always uses a copy
  of your data and *does not* modify your original dataset.
- Data cleaning steps often need repeating with multiple files. OpenRefine
  keeps track of all of your actions and allows them to be applied to different datasets.
- Some concepts such as clustering algorithms are quite complex, but OpenRefine
  makes it easy to introduce them, use them, and show their power.

## Features

- Open source ([source on GitHub](https://github.com/OpenRefine/OpenRefine)).
- A large growing community, from novice to expert, ready to help. See Getting
  Help section below.
- Works with large-ish datasets (100,000 rows). Can adjust memory allocation to
  accommodate larger datasets.
- OpenRefine always keeps your data private on your own computer until you
  choose to share it. It works by running a small server on your computer and
  using your web browser to interact with it, but your private data never
  leaves your computer unless you want it to.


::: instructor

### Data privacy when using APIs or reconciliation

Most functionality does not require an Internet connection and keeps your data
within the computer.
Some functions, however, like looking up data from URLs or reconciling values
in your dataset with online services, necessarily require that data is sent to
the online services.
While this lesson does not cover these functions, it may be important to know
how data could be shared with outside parties, especially if you work with
sensitive or confidential data.

::::::::::::::

## Before we get started

Note: this is a Java program that runs on your machine (not in the cloud). It
runs inside your browser, but no web connection is needed.

Follow the [Setup](../learners/setup.md) instructions to install OpenRefine.

If after installation and running OpenRefine, it does not automatically open
for you, point your browser at [http://127.0.0.1:3333/](https://127.0.0.1:3333/)
or [http://localhost:3333](https://localhost:3333) to launch the program.

## Getting help for OpenRefine

You can find out a lot more about OpenRefine at [http://openrefine.org](https://openrefine.org)
and check out some great introductory videos.

These videos and others on OpenRefine can also be found on YouTube by searching under
'OpenRefine'.  There is an [official forum](https://forum.openrefine.org/) that
can answer a lot of beginner questions and problems. Information can also be found on
[StackOverflow](https://stackoverflow.com/questions/tagged/openrefine) where
you can find a lot of help. As with other programs of this type, OpenRefine
libraries are available too, where you can find a script you need and copy it
into your OpenRefine instance to run it on your dataset.



:::::::::::::::::::::::::::::::::::::::: keypoints

- OpenRefine is a powerful, free, and open source tool that can be used for data cleaning.
- OpenRefine will automatically track any steps allowing you to backtrack as needed and providing a record of all work done.

::::::::::::::::::::::::::::::::::::::::::::::::::


