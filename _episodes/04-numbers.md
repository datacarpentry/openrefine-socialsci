---
title: "Examining Numbers in OpenRefine"
teaching: 10
exercises: 10
questions:
- "How can we convert a column from one data type to another?"
- "How can we find non-numeric values in a column that should contain numbers?"
objectives:
- "Transform a text column into a number column."
- "Identify and modify non-numeric values in a numeric column using facets."
keypoints:
- "OpenRefine also provides ways to to examine and clean numerical data."
---

## Numbers

When a table is imported into OpenRefine, all columns are treated as containing text values. We saw earlier how we can sort column values as numbers, but this does not change the cells in a column from text to numbers. Rather, this interprets the values as numbers for the purposes of sorting but keeps the underlying data type as is. We can, however, transform columns from text to other data types (e.g. number or date) using the `Edit cells` > `Common transforms` feature. Here we will experiment changing columns to numbers and see what additional capabilities that grants us.

Be sure to remove any `Text filter` facets you have enabled from the left panel so that we can examine our whole dataset. You can remove an existing facet by clicking the `x` in the upper left of that facet window.

To transform cells in the `years_farm` column to numbers, click the down arrow for that column, then `Edit cells` > `Common transforms…` > `To number`. You will notice the `years_farm` values change from left-justified to right-justified, and black to green in color.

> ## Exercise
>
> Transform three more columns, `no_membrs`, `years_liv`, and `buildings_in_compound`, from text to numbers. Can all columns be transformed to numbers? - Try it with `village` for example.
>
> > ## Solution
> >
> > Only observations that include only numerals (0-9) can be transformed to numbers. If you apply a number transformation to
> > a column that doesn't meet this criteria, and then click the `Undo / Redo` tab, you will see a step that starts with
> > `Text transform on 0 cells`. This means that the data in that column was not transformed.
> {: .solution}
{: .challenge}

### Numeric facet
Sometimes non-numeric values or blanks occur in a column where numbers are expected. Such values may represent errors in data entry, and we want to find them.
We can do that with a `Numeric facet`.

> ## Exercise
> 1. For a column you transformed to numbers, edit one or two cells, replacing the numbers with text (such as `abc`) or blank (no number or text). You will need to change the `Data type` to `text` using the drop-down menu.
> 2. Use the column pulldown menu to apply a numeric facet to the column you edited. The facet will appear in the left panel.
> 3. Notice that there are several checkboxes in this facet: `Numeric`, `Non-numeric`, `Blank`, and `Error`. Below these checkboxes are counts of the number of cells in each category. You should see checks for `Non-numeric` and `Blank` if you changed some values.
> 4. Experiment with checking or unchecking these boxes to select subsets of your data.
{: .challenge}

When done examining the numeric data, remove this facet by clicking the `x` in the upper left corner of its panel. Note that this does not undo the edits you made to the cells in this column. Use the `Undo / Redo` function to reverse these changes.

{% include links.md %}
