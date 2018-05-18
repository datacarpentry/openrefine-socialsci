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

1. Click the down arrow next to `respondent_roof_type` > `Text filter`. A `respondent_roof_type` facet will appear on the left margin.
2. Type in `mabat` and press return. There are 58 matching rows of the original 131 rows (and these rows are selected for the subsequent steps).
3. At the top, change the view to `Show` 50 `rows`. This way you will see most of the matching rows.

> ## Exercise
>
> 1. What roof types are selected by this procedure?  
> 2. How would you restrict this to only one of the roof types?  
>
> > ## Solution
> > 1. Do `Facet` > `Text facet` on the `respondent_roof_type` column after filtering. This will show that
> > two names match your filter criteria. They are `mabatipitched` and `mabatisloping`.   
> > 2. To restrict to only one of these two roof types, you could include more letters in your filter.
> >
> {: .solution}
{: .challenge}

### Excluding entries


In addition to the simple text filtering we used above, another way to narrow our filter is to `include` and/or `exclude` entries in a facet. You will see the `include` or `exclude` options if you hover over the name in the facet window.

If you still have your facet for `respondent_roof_type`, you can use it, or use drop-down menu > `Facet` > `Text facet` to create a new facet. Only the entries with names that agree with your `Text filter` will be included in this facet.

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
> > 2. Click `include`. This will explicitly include this roof type, and exclude others that are not explicitly included. Notice that the
> option now changes to `exclude`.
> > 3. Click `include` and `exclude` on the other roof type and notice how the two entries appear and disappear
> >  from the table.
> >
> {: .solution}
{: .challenge}

Remove the filter before moving on so that you again have the full dataset of 131 records.

## Sort

You can sort the data by a column by using the drop-down menu in that column.
There you can sort by `text`, `numbers`, `dates` or `booleans` (`TRUE` or `FALSE` values). You can also specify what order to put `Blanks` and `Errors` in the sorted results.

If this is your first time sorting this table, then the drop-down menu for the selected column shows `Sort...`. Select what you would like to sort by (such as `numbers`). Additional options will then appear for you to fine-tune your sorting.

> ## Exercise
>
> Sort the data by `gps_Altitude`. Do you think the first few entries may have incorrect altitudes?.
>
> > ## Solution
> > In the `gps:Altitude` column, select `Sort...` > `numbers` and select `smallest first`. The first few values are all 0. The altitudes are more likely 'missing' than incorrect. The survey is delivered by Smartphone with the gps information added automatically by the app. The lack of an altitude value suggests that the smartphone was unable to provide it and it defaulted to 0.
> {: .solution}
{: .challenge}


If you try to re-sort a column that you have already used, the drop-down menu changes slightly, to > `Sort` without the `...`, to remind you that you have already used this column. It will give you additional options:

* `Sort` > `Sort...` - This option enables you to modify your original sort.
* `Sort` > `Reverse` - This option allows you to reverse the order of the sort.
* `Sort` > `Remove sort` - This option allows you to undo your sort.

### Sorting by multiple columns.

You can sort by multiple columns by performing sort on additional columns. The sort will depend on the order in which you select columns to sort. To restart the sorting process with a particular column, check the `sort by this column alone` box in the `Sort` pop-up menu.

If you go back to one of the already sorted columns and select > `Sort` > `Remove sort`, that column is removed from your multiple sort. If it is the only column sorted, then data reverts to its original order.

> ## Exercise
>
> We discovered in an earlier lesson that the value for one of the `village` entries was given as 49. This is clearly wrong. By looking at the GPS coordinates for the entries of the other villages can we decide what village the data in that column was collected from?   
> 1. Sort on `gps_Longitude` as a number with the largest first.   
> 2. Add a sort on `gps_Lattitude` as a number with the largest first. 
> 3. Using the drop down arrow on the `village` column, select `Edit column` > `Move column to end`. This will allow you to compare village names with GPS coordinates. 
> 4. Scroll through the entries until you find village `49`. Can you tell from it's GPS coordinates which village it belong to?
> 5. Now sort only by `interview_date` as date. Move the `village` column to the start of the table. Does the row where village is `49` group with one particular village? Is it the same village as when comparing GPS coordinates?
>
> > ## Solution
> >
> > The interview data for that row is in a small cluster of Chirodzo interviews when sorting by GPS coordinates. When sorting by interview date, it is also with Chirodzo interviews. In fact, only Chirodzo had interviews conducted on that date. 
> {: .solution}  
{: .challenge}

Perform a text facet on the `village` column and change `49` to the village name that was determined in the previous exercise. You should now have only three village names. 

{% include links.md %}
