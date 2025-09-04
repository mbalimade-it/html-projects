# Basic Table Structure

Tables let you display data in rows and columns - like in Excel or Google Sheets. They are perfect to display: schedules, prices, reports etc.

Tables are built using these key elements:

1. `<table>` → The table container
1. `<tr>` → Table row
1. `<td>` → Table data
1. `<th>` → Table header

---

# Table Sections

Table sections help your tables become more structured and professional. They do not change how the table looks, but they organize the table semantically.

How we organize tables:

- `<thead>` (table head) - groups the header rows and usually contain th and tr.
- `<tbody>` (table body) - groups the main data rows and usually contains tr and td.
- `<tfoot>` (table footer) - groups the footer rows and often used for totals, summaries or notes.
- `<caption>` (table title) - short description/title of the table.

---

# Column and Row Spanning

Column and row spanning allows you to stretch tables across multiple columns or rows.
This is useful as you might want a title cell that stretches across the whole table or a cell that covers multiple rows.

That’s where `colspan` and `rowspan` attributes come in.

1. **`colspan="number"`**

   - Makes a cell span across multiple **columns**.
   - Example: One cell covering 3 columns in the same row.

2. **`rowspan="number"`**

   - Makes a cell span across multiple **rows**.
   - Example: One cell covering 2 or more rows downwards.

---

# Table accessibility (scope, headers attributes)

Table accessibility is all about **making your tables understandable for everyone** - especially people who use screen readers. The program needs extra clues to properly align which heading belongs to which data etc.

That’s where `scope` and `headers` come in.

---

## 1. The `scope` attribute

- Used only inside `<th>`.
- Tells the browser/screen reader what the header applies to.

Values:

- `scope="col"` → says this is a **header column**
- `scope="row"` → says this is a **header row**

_The **example code** includes rows and columns as headers, then the data inside the table_

---

## 2. The `headers` attribute

- Used inside `<td>` (data cell).
- Explicitly **links** a data cell to one or more `<th>` elements.
- This is very helpful when you have **complex tables** with multiple levels of headers.

_On the example code you can see that each `<th>` has an `id` and each `<td>` points to its related header(s) using `headers="..."`._

## When to use what?

- Use **`scope`** for **simple tables** (1 header row + 1 header column).
- Use **`headers`** (with `id`) for **complex tables** (multi-level headers, spanning cells).

## Resources

## [H63: Using the scope attribute to associate header cells and data cells in data tables](https://www.w3.org/TR/WCAG20-TECHS/H63.html#:~:text=The%20scope%20attribute%20may%20be,identify%20these%20possible%20scopes%20respectively)

# Column Grouping

Column grouping is best for when you want to style a table with many rows and columns. So instead of styling every cell individually, you can target the table column and it will style it entirely. It is useful for setting widths, background colours or hiding columns.

The elements

1. **`<colgroup>`**

   - A container for one or more `<col>` elements.
   - Placed between **`<caption>` (if any)** and `<thead>`.

2. **`<col>`**

   - Defines properties for a single column.
   - Can use `span="n"` to cover multiple columns at once.

_the example code shows 3 different tables that style the background of different columns, styling and spanning over columns and setting up the width of each column_

---

# Responsive Table Consideration

There's a big problem with creating tables - they don't respond well on small screens (like cellphones). Tables are naturally wide and have many columns with tons of data. When viewed on smaller screens, this can create text squishing, table extending outside of the screen, and too much info at once can make everything confusing.

The easiest html approach is usually called:

**Scrollable tables or horizontal scrolling tables**

It is the simplest responsive table solution as it allows the user to scroll left/right(sideways) if the screen is too small.

Steps:

1. Wrap table in a `<div>` - a div acts as a container
2. Use `style="overflow-x:auto;"`

Explanation:

- `overflow-x` means → what happens if the content is too wide **horizontally (x-axis)**.
- `auto` means → if the table fits, nothing happens. If it **doesn’t fit**, then the browser will **add a scroll bar** automatically.

And that is it, the rest is left untouched.

---
