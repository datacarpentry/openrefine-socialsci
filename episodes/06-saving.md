---
title: Exporting and Saving Data from OpenRefine
teaching: 10
exercises: 5
---

::::::::::::::::::::::::::::::::::::::: objectives

- Export cleaned data from an OpenRefine project.
- Save an OpenRefine project as a shareable file.

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- How can we get our cleaned data out of OpenRefine?
- How can we save the whole project with all history as a file?

::::::::::::::::::::::::::::::::::::::::::::::::::

## Exporting Cleaned Data

When you completed the cleaning steps, you probably want to save the cleaned
dataset as a new file, so that you can further analyse the data using other
applications.
OpenRefine allows you to do so by *exporting* the data in various file formats.

1. Click `Export` in the top right and select the file type you want to export
   the data in. `Tab-separated values` (`tsv`) or `Comma-separated values`
   (`csv`) would be good choices.
2. OpenRefine creates a file whose name is based on the project name and asks
   the browser to download it.
   Depending on your browser settings, this file is automatically saved in the
   default location for downloaded files, or you see a dialog window to choose
   where you want to save the file.

The downloaded file can then be opened in a spreadsheet program or imported into
programs written in R or Python, for example.

Remember from our lesson on Spreadsheets that using widely-supported,
non-proprietary file formats like `tsv` or `csv` improves the ability of
yourself and others to use your data.

::::::::::::::::::::::::::: callout

### Only matching rows are exported

OpenRefine only operates on rows that match all enabled filters.
This is also true for exporting data.
So if you want to export a selection from a larger dataset, you can use filters
and facets to select what data you want to export.

However, if you wanted to export all data and forget to reset all facets and filters,
the exported dataset may appear to be incomplete.
OpenRefine does not provide a warning about enabled filters when you export data.

:::::::::::::::::::::::::::::::::::


## Saving a Project as a File

Next to exporting the data, you can export the project as well.
When you export the project, OpenRefine creates a single file that includes the
data and all the information about the cleaning and data transformation steps
that you have taken.

You can use this file as a project backup, transfer it to another computer to
continue working on the data or share it with a collaborator who can open it
to see what you did and continue the work.

::::::::::::::::::::::::::: callout

### Saving happens automatically

By default OpenRefine is saving your project continuously while you work on it.
If you close OpenRefine and open it up again, you can see a list of your
projects when you select "Open Project" on the start screen.
You can open an existing project by clicking on its title.

:::::::::::::::::::::::::::::::::::


::::::::::::::::::::::::: challenge

### Exporting and examining the project

In this exercise, we will export the project and examine the contents of the
exported file.

1. Click the `Export` button in the top right and select `OpenRefine project archive to file`.
2. OpenRefine then presents a `tar.gz` file for download.
   Depending on your browser you may have to specify where you want to save the
   file, or it may be downloaded to your default directory for downloaded files.
   The `tar.gz` extension tells you that this is a compressed file. The
   downloaded `tar.gz` file is actually a folder of files which have been
   compressed. Linux and Mac machines will have software installed to
   automatically expand this type of file when you double-click on it. For
   Windows based machines you may have to install a utility like '7-zip' in
   order to expand the file and see the files in the folder.
3. After you have expanded the file, look at the files that appear in this
   folder. What files are here? What information do you think these files
   contain?

:::::::::::::::  solution

### Solution

You should see:

- a `history` folder which contains a collection of  `zip` files. Each of
  these files itself contains a `change.txt` file. These `change.txt` files
  are the records of each individual transformation that you did to your
  data.
- a `data.zip` file. When expanded, this `zip` file includes a file called
  `data.txt` which is a copy of your raw data. You may also see other files.
  

:::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::

### Importing a Project

You can import an existing project into OpenRefine by clicking `Open...` in the
upper right, then opening the `Import Project` tab and selecting the `tar.gz`
project file.


:::::::::::::::::::::::::::::::::::::::: keypoints

- Cleaned data, or selected data, can be exported from OpenRefine
  for use in other applications.
- Projects can be exported to files that contain the original data
  and all data cleaning steps you performed.

::::::::::::::::::::::::::::::::::::::::::::::::::
