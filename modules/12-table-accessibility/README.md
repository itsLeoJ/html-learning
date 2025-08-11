# HTML Table Accessibility ♿

## Introduction
- This article focuses on making HTML tables accessible, especially for visually impaired users.
- It covers captions, structuring with `<thead>`, `<tbody>`, and `<tfoot>`, and using `scope`, `id`, and `headers` attributes.
- **Prerequisites:** Basic HTML knowledge.
- **Learning outcomes:** Understanding table accessibility issues, adding captions, improving structure, and creating associations between headers and cells.

---

## Recap: Tables for Visually Impaired Users 👁️‍🗨️
- Tables are useful for quick data access and lookups.
- Sighted users make visual associations between data and headers.
- Visually impaired users use screen readers, which can struggle with tables.
- Proper markup can create programmatic associations to help screen readers.
- **Fact:** Around 253 million people live with visual impairment (WHO 2017 data).

### Using Column and Row Headers 🗣️
- Screen readers identify `<th>` headers to programmatically associate them with related cells.
- This allows screen reader users to interpret the table similarly to sighted users.

---

## Adding a Caption with `<caption>` 📝
- The `<caption>` element provides a descriptive caption for the table.
- Place it directly after the opening `<table>` tag.
- Useful for all readers to quickly understand the table's purpose without reading all cells.
- **Note:** The `summary` attribute is deprecated; `<caption>` is recommended as it's visible on the page.

---

## Adding Structure with `<thead>`, `<tbody>`, and `<tfoot>` 🧱
- These elements define the header, body, and footer sections of a table.
- They don't inherently improve accessibility for screen readers but are crucial for applying CSS styling.
- Styling can enhance accessibility by improving layout and readability.
- **Order:** `<thead>` (header rows), `<tbody>` (main content), `<tfoot>` (footer rows).
- `<tbody>` is implicitly added by browsers if not specified, but explicit use provides more control.

---

## The `scope` Attribute 🎯
- Added to `<th>` elements to explicitly define what cells the header relates to.
- **Values:**
  - `scope="col"`: Header for a column.
  - `scope="row"`: Header for a row.
  - `scope="colgroup"`: Header for a group of columns (e.g., "Clothes" over "Trousers," "Skirts," and "Dresses").
  - `scope="rowgroup"`: Header for a group of rows (e.g., "The Netherlands" over "Amsterdam" and "Utrecht").
- Allows screen readers to read entire columns or rows at once.

---

## The `id` and `headers` Attributes 🆔
- An alternative method for creating precise associations between headers and data cells.
- Use `id` on each `<th>` element to give it a unique identifier.
- Use `headers` on `<td>` and subheading `<th>` elements to link them to the corresponding `<th>` `id`(s).
- Takes a space-separated list of `id`s.
- This method is very explicit but requires more markup. The `scope` attribute is often sufficient for most tables.

---

## Summary ✅
- This article covered essential features for making HTML tables accessible.
- Topics included captions (`<caption>`), structural elements (`<thead>`, `<tbody>`, `<tfoot>`), and header-cell associations (`scope`, `id`, and `headers`).
- You are now ready to take on the HTML tables challenge.