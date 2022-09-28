---
title: "Exporting and Saving Data from OpenRefine"
teaching: 10
exercises: 5
questions:
- "How can we save and export our cleaned data from OpenRefine?"
objectives:
- "Save an OpenRefine project."
- "Export cleaned data from an OpenRefine project."
keypoints:
- "Cleaned data or entire projects can be exported from OpenRefine."
- "Projects can be shared with collaborators, enabling them to see, reproduce and check all data cleaning steps you performed."
---

## Saving and Exporting a Project

In OpenRefine you can save or export the project. This means you're saving the data and all the 
information about the cleaning and data transformation steps you've done. Once you've saved a project, you can
open it up again and be just where you stopped before.

### Saving

By default OpenRefine is saving your project continuously. If you close OpenRefine and open it up again,
you'll see a list of your projects. You can click on any one of them to open it up again.

### Exporting

You can also export a project. This is helpful, for instance, if you wanted to send your raw data and cleaning steps to a collaborator, 
or share this information as a supplement to a publication. 

1. Click the `Export` button in the top right and select `OpenRefine project archive to file`.
2. A `tar.gz` file will download to your default `Download` directory. Depending on your browser you may have to confirm that you want to save the file. The `tar.gz` extension tells you that this is a compressed file.
The downloaded `tar.gz` file is actually a folder of files which have been compressed. Linux and Mac machines will have software installed to automatically expand this type of file when you double-click on it. For Windows based machines you may have to install a utility like '7-zip' in order to expand the file and see the files in the folder. 
3. After you have expanded the file look at the files that appear in this folder. What files are here? What information do you think these files contain?

> ## Solution
> You should see:
> - a  `history` folder which contains a collection of  `zip` files. Each of these files itself contains a `change.txt` file. 
> These `change.txt` files are the records of each individual transformation that you did to your data. 
> - a `data.zip` file. When expanded, this `zip` file includes a file called `data.txt` which is a copy of your raw data.
> You may also see other files.
{: .solution}

You can import an existing project into OpenRefine by clicking `Open...` in the upper right > `Import Project` and selecting the `tar.gz` 
project file. This project will include all of the raw data and cleaning steps that were part of the original project.

## Exporting Cleaned Data 

You can also export just your cleaned data, rather than the entire project.

1. Click `Export` in the top right and select the file type you want to export the data in. `Tab-separated values` (`tsv`) or `Comma-separated values` (`csv`) would be good choices.
2. That file will be exported to your default `Download` directory. That file can then be opened in a spreadsheet program or imported
into programs like R or Python, which we'll be discussing later in our workshop.

Remember from our lesson on Spreadsheets that using widely-supported, non-proprietary file formats like `tsv` or `csv` improves the ability of yourself and others to use your data. 

{% include links.md %}
