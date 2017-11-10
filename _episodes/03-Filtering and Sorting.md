---
title: "Filtering and Sorting with OpenRefine"
teaching: 10
exercises: 10
questions:
- "How can we select only a subset of our data to work with?"
- "How can we sort our data?"
objectives:
- "Filter to a subset of rows by text filter or include/exclude."
- "Sort table by a column."
- "Sort by multiple columns."
keypoints:
- "OpenRefine provides a way to sort and filter data without affecting the raw data."
---

# Lesson

## Filtering

There are many entries in our data table. We can filter it to work on a subset of the data in the list for the next set of operations. Please ensure you perform this step to save time during the class.

1. Click the down arrow next to `C01_responent_roof_type` > `Text filter`. A `C01_responent_roof_type` facet will appear on the left margin.
2. Type in `mabat` and press return. There are 58 matching rows of the original 131 rows (and these rows are selected for the subsequent steps).
3. At the top, change the view to `Show` 50 `rows`. This way you will see most of the matching rows.

> ## Exercise
>
> 1. What roof types are selected by this procedure?  
> 2. How would you restrict this to only one of the roof types?  
> 
> > ## Solution
> > 1. Do `Facet` > `Text facet` on the `C01_responent_roof_type` column after filtering. This will show that
> > two names match your filter criteria. They are `mabatipitched` and `mabatisloping`.   
> > 2. To restrict to only one of these two roof types, you could make include more letters in your filter.
> > 
> {: .solution}
{: .challenge}

### Excluding entries


In addition to the simple text filtering we used above, another way to narrow our filter is to `include` and/or `exclude` entries in a facet. You will see the `include` or `exclude` options if you hover over the name in the facet window.

If you still have your facet for `C01_responent_roof_type`, you can use it, or use drop-down menu > `Facet` > `Text facet` to create a new facet. Only the entries with names that agree with your `Text filter` will be included in this facet.

Faceting and filtering look very similar. A good distinction is that faceting gives you an overview description of all of the data that 
is currently selected, while filtering allows you to select a subset of your data for analysis. 


> ## Exercise
>
> Use `include / exclude` to select only entries from one of these two roof types.
>
> > ## Solution
> > 
> > 1. In the facet (left margin), click on one of the names, such as `mabatisloping`. Notice that when you click on the name, or hover
> > over it, there are entries to the right for `edit` and `include`. 
> > 2. Click `include`. This will explicitly include this roof type, and exclude others that are not expicitly included. Notice that the
> option now changes to `exclude`.
> > 3. Click `include` and `exclude` on the other roof type and notice how the two entries appear and disappear
> >  from the table.
> > 
> {: .solution}
{: .challenge}

Remove the facet and the filter before moving on so that you again have the full dataset of 131 records.

## Sort

You can sort the data by a column by using the drop-down menu in that column.
There you can sort by `text`, `numbers`, `dates` or `booleans` (`TRUE` or `FALSE` values). You can also specify what order to put `Blanks` and `Errors` in the sorted results.

If this is your first time sorting this table, then the drop-down menu for the selected column shows `Sort...`. Select what you would like to sort by (such as `numbers`). Additional options will then appear for you to fine-tune your sorting.

If you try to re-sort a column that you have already used, the drop-down menu changes slightly, to > `Sort` without the `...`, to remind you that you have already used this column. It will give you additional options:

* > `Sort` > `Sort...` - This option enables you to modify your original sort. 
* > `Sort` > `Reverse` - This option allows you to reverse the order of the sort.
* > `Sort` > `Remove sort` - This option allows you to undo your sort.

> ## Exercise
> 
> Sort the data by `gps:Altitude`. Do you think the first 4 entries may have incorrect altitudes?. 
> 
> > ## Solution
> > In the `plot` column, select `Sort...` > `numbers` and select `smallest first`. The years represented are 1990 and 1995.
> > 
> {: .solution}
{: .challenge}


### Sorting by multiple columns.

You can sort by multiple columns by performing sort on additional columns. The sort will depend on the order in which you select columns to sort. To restart the sorting process with a particular column, check the `sort by this column alone` box in the `Sort` pop-up menu.

> ## Exercise
>
> We discovered in an earlier lesson that the value for one of the `A09_village` entries was given as 49. Something that is clearly wrong. By looking at the altitudes for the entries of the other villages can we decide what the 49 value should be?     
> 1. Sort on `A09_village` as text.   
> 2. Sort on `gps:Altitude` as a number with the largest first.
> 3. Scan down the sorted `gps:Altitude` and see if you can decide wher the village changes based on the altitudes.
> 4. Lookup the altitude value for village '49' and decide which is the most likely village for it to belong in.
> 
> > ## Solution
> > 
> > 1. For the `A09_village` column, click on `Sort...` and then `text`. This will group all of the villages in name order. village '49' will appear at the top. 
> > 2. For the `gps:Altitude` column, click on `Sort` > `Sort...` > `numbers` and select `largest first`. 
> > 3. make a note of the altitude for village '49' and see where you think it fits in.
> >
> > Given the accuracy of the gps reading this is hardly a foolproof approach. A asimple one would be to;
> > 
> > 4.  For the `A04_start` column, click on `Sort` > `Sort...` > `dates` and select `earliest first` and `sort by this column alone`. This will remove all of your previous sorts.
> > 5. Now find where village '49' fits in with this order list of `A04_start` values.
> {: .solution}  
{: .challenge}

If you go back to one of the already sorted colunms and select > `Sort` > `Remove sort`, that column is removed from your multiple sort. If it is the only column sorted, then data reverts to its original order.

