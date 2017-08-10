---
title: "Using regular expressions "
teaching: 0
exercises: 0
questions:
- "How can we use patterns in strings to subset the data?"
objectives:
- "Use GREL to create simple regular expressions to filter data"
keypoints:
- "Using regular expressions allow you to create more complex and precise filter conditions."
---

## Using regular expressions to filter data

A regular expression is a sequence of characters that define a search pattern. When you use the Text filter and start to type a few letters, those letters represent a pattern to search for.

> ## Exercise
> 
> 1. In the `C01_responent_roof` column find a row which has  a value of **green**. Edit the cell and change the value to **green-grass**
> 2. Click the down arrow on the column and select Text filter.
> 3. Type the letters **gr**
> 4. How many rows are returned by this filter?
> 5. Now change the filter to **-gr**
> 6. How many rows are returned now?
> 
> > ## Solution
> >
> > The first filter should return 73 rows, including the green-grass row.
> > The second filter only returns the green-grass row.
> > The pattern **gr** occurs in all of the rows with **grass** but the pattern **-gr** only occurs in the one **green-grass** row. It doesn't matter that it is not at the start of text string
> > 
> {: .solution}
{: .challenge}


Because we were just interested in the pattern **gr** and didn't where it occurred we could use a simple Text filter.

Suppose now that from the `A01_interview date` column we wanted to know which dates were _not_ in **Nov**

In this case we will need to use a regular expression. We need to construct a pattern which says: there are 2 digits followed by a hypthen and then the next character is _not_ allowed to be an 'N' after that we don't care. 


> ## Exercise
> 
> 1. Create a Text filter for the `A01_interview_date` column.
> 2. check the `regular expression box`
> 3. In text box type **[0-9]{2}-[N]**. 
> 4. There should be 88 matching rows. But this is telling us which rows are in Nov. We could have done this more easily by simply typing **-Nov-** into the normal Text fileter.
> 5. Now change the expression to **[0-9]{2}-[^N]**
> 6. the **^** acts like a **NOT**, so now instead of looking for 2 digits ([0-9]{2}) followed by '-' followed by capital N ([N]), we are now looking for 2 digits followed by '-' followed by anything but 'N'
> 7. We should end up with the 43 rows where the interview date was not in November.
{: .challenge}

With regular expressions it is possible to construct any arbitary complex search pattern. More details of the regular exresssion construcs that you can use with OpenRefine are available in the OpenRefine Wiki site on github. The link is [here](https://github.com/OpenRefine/OpenRefine/wiki/Understanding-Regular-Expressions).




