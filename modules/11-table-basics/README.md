# HTML Table Basics 📊

This article provides an introduction to HTML tables, covering basic structure, headings, and cell spanning.

-----

## Prerequisites & Learning Outcomes 🎯

**Prerequisites:**

  - Basic HTML knowledge, specifically `Basic HTML Syntax`.

**Learning Outcomes:**

  - Understanding the purpose of tables: **structuring tabular data**.
  - Recognizing what tables are not for: **page layout**.
  - Basic table syntax: `<table>`, `<tr>` (table row), and `<td>` (table data/cell).
  - Defining headers with `<th>` (table header).
  - Spanning multiple columns and rows using the `colspan` and `rowspan` attributes.

-----

## What Is a Table? 📋

A table is a structured set of data organized into rows and columns. It allows for easy lookup and association of different data types, like a person's age or a timetable.

  - Tables are a rigid and effective way to present data, making information easy to interpret through visual associations with row and column headers.
  - **Accessibility:** When implemented correctly, HTML tables are handled well by screen readers, enhancing the experience for visually impaired users.
  - **Styling:** For tables to be effective and readable on the web, they require styling with CSS, which is covered in a separate lesson.

-----

## When to Avoid HTML Tables 🚫

HTML tables are designed exclusively for **tabular data**. They should not be used for page layout, a practice that was common in the past due to limited CSS support.

**Reasons to avoid table-based layouts:**

  - **Reduced accessibility:** Screen readers can get confused by the complex markup of layout tables.
  - **"Tag soup":** Layout tables often have more complex markup, making the code harder to write, maintain, and debug.
  - **Not automatically responsive:** Tables are sized by their content by default, requiring extra effort to adapt to different screen sizes.

-----

## Creating Your First Table 🔨

1.  Start with the `<table></table>` tags to enclose all table content.
2.  Each table row is created with a `<tr>` element.
3.  Each cell within a row is created with a `<td>` element.
4.  Cells automatically align on the same row until a new `<tr>` is started.

**Example:**

```html
<table>
  <tr>
    <td>First row, first cell.</td>
    <td>First row, second cell.</td>
  </tr>
  <tr>
    <td>Second row, first cell.</td>
    <td>Second row, second cell.</td>
  </tr>
</table>
```

-----

## Adding Headers with `<th>` Elements 🏷️

Table headers are special cells that define the type of data for a row or column. They are created using the `<th>` element instead of `<td>`.

  - **Visual and semantic recognition:** `<th>` elements are bold and centered by default, making them stand out.
  - **Accessibility benefit:** Headers, along with the `scope` attribute, help screen readers associate data with the correct header, allowing them to read out a whole row or column at once.

-----

## Allowing Cells to Span Rows and Columns ↔️↕️

Use the `colspan` and `rowspan` attributes to make a cell span across multiple columns or rows.

  - Both attributes accept a unitless number as a value, specifying how many columns or rows the cell should span.
  - `colspan="2"`: Makes a cell span two columns.
  - `rowspan="2"`: Makes a cell span two rows.

**Example:**

```html
<table>
  <tr>
    <th colspan="2">Animals</th>
  </tr>
  <tr>
    <th rowspan="2">Horse</th>
    <td>Mare</td>
  </tr>
  <tr>
    <td>Stallion</td>
  </tr>
</table>
```