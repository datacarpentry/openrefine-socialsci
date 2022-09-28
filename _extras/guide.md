---
layout: page
title: "Instructor Notes"
---

## Lesson

This time allotted for the teaching and exercises in lessons one through eight in this episode totals 135 minutes. This does not include time for installing OpenRefine, which could take an extra 10-30 minutes depending on how many different platforms and how many computers need OpenRefine installed.

## Setup

- There is a separate page with [setup instructions for installing OpenRefine]({{ page.root }}{% link setup.md %}).
- If Internet Explorer is the default browser for participants, OpenRefine may have trouble opening. The URL can be copied and pasted into a Google Chrome or Firefox browser. Or, participants can be encouraged in advance of the workshop to set one of these two browsers as their default.

## The datasets used

- The dataset used in this lesson can be downloaded from Figshare through
 the link on the [setup page]({{ page.root }}{% link setup.md %}).
- It will need to be downloaded to the local machine before it can be loaded into OpenRefine.
- A general description of the dataset used in the Social Sciences lessons can be found [in the workshop data home page](http://www.datacarpentry.org/socialsci-workshop/data/)

## The Lessons

[Introduction]({{ page.root }}{% link _episodes/01-introduction.md %})

- Explains what OpenRefine is, what it is used for and where to get help.

[Working with OpenRefine]({{ page.root }}{% link _episodes/02-working-with-openrefine.md %})

- Covers the creation of an OpenRefine project using our dataset.
- The file has a single header row and is csv.
- Facets and clustering are introduced and there is a discussion on the different clustering algorithms and how they may produce different results.
- Splitting columns is covered as is undo/redo.

[Filtering and Sorting]({{ page.root }}{% link _episodes/03-filter-sort.md %})

- Using Include and Exclude from a facet is covered and the difference between faceting and filtering is explained.
- The various sort options for single or multiple columns is covered.

[Examining Numbers in OpenRefine]({{ page.root }}{% link _episodes/04-numbers.md %})

- Explains that everything is a string until you change it.
- Explains how to change the data type and the additional faceting ability it provides.

[Using scripts]({{ page.root }}{% link _episodes/05-scripts.md %})

- Explains how actions within a project can be copied to an external file and re-applied. The same file is used to re-apply the changes.

[Saving results]({{ page.root }}{% link _episodes/06-saving.md %})

- Covers the overall format of a project 'file' and how the components can be viewed.
- This may require installing additional software on Windows machine (e.g. 7-zip) as the built-in un-zipping facility does not work with tar.gz files.

[Other resources in OpenRefine]({{ page.root }}{% link _episodes/07-resources.md %})

- Just a list of various OpenRefine resources available on-line (taken from the Ecology lessons)
