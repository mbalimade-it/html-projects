# Basic File Structure and Organization

- Keep everything in **one main project folder** for organization.

- Inside it, have your main file **`index.html`** (browser looks for this first).

- Create subfolders:

  - **`css/`** → stylesheets
  - **`js/`** → JavaScript files
  - **`images/`** → images

- A clean folder might look like: `index.html`, `about.html`, and folders for CSS, JS, and images.

- Inside `index.html`, include a basic HTML skeleton with `<head>` (for title, meta info, CSS) and `<body>` (for visible content and linking JS).

- Always use **relative paths** like `css/style.css` or `images/logo.png` to connect files.

- This keeps your site neat, easy to manage as it grows, and follows standard practices.

---

# Block vs Inline Elements

### 1. Block Elements

- Take up the **full width** available.
- Always start on a **new line**.
- Can contain **other block elements** and inline elements.
- Examples: `<div>`, `<p>`, `<h1>`-`<h6>`, `<section>`, `<article>`, `<header>`, `<footer>`, `<ul>`, `<ol>`, `<li>`.

**Visual idea:**

```
[Paragraph 1 takes full width]
[Paragraph 2 takes full width]
```

### 2. Inline Elements

- Take up **only as much width as needed**.
- Do **not** start on a new line; they sit inside block elements.
- Usually used for formatting text.
- Examples: `<span>`, `<a>`, `<strong>`, `<em>`, `<img>`, `<label>`, `<button>`.

**Visual idea:**

```
This is [bold] and [italic] inside one line.
```

**Rule of Thumb:**

- Use **block** elements to structure the page.
- Use **inline** elements to style or highlight parts of content inside blocks.

---

# HTML Entities and Special Characters

- HTML entities let you show **reserved characters** (like `<` or `>`) or special symbols (©, €, ♥).
- They are **codes that the browser displays as characters**.

### How They Work

- Start with `&` and end with `;`.
- Examples:

  - `&lt;` → `<`
  - `&gt;` → `>`
  - `&amp;` → `&`

**Tip:** To show `<p>` as text on a page, write `&lt;p&gt;`.

### Common HTML Entities

| Character | Entity Code | Output |
| --------- | ----------- | ------ |
| `<`       | `&lt;`      | <      |
| `>`       | `&gt;`      | >      |
| `&`       | `&amp;`     | &      |
| `"`       | `&quot;`    | "      |
| `'`       | `&apos;`    | '      |
| ©         | `&copy;`    | ©      |
| €         | `&euro;`    | €      |
| ®         | `&reg;`     | ®      |
| ♥         | `&hearts;`  | ♥      |

**Example Usage:**

- `Use &lt;h1&gt; for main headings.` → Displays `<h1>`
- `Price: 50 &euro;` → Displays `Price: 50 €`
- `Made with &hearts; in Belgium` → Displays `Made with ♥ in Belgium`

**Rule of Thumb:**

- Use entities to display HTML code as text or special symbols.

---

# Basic Text Content Elements

### `<span>`

- Inline container for small pieces of text.
- Often used for styling.
  Example: `This is <span style="color:red;">important</span> text.`

### `<code>`

- Inline element for **computer code**.
- Monospace font by default.
  Example: `Use the <code>&lt;h1&gt;</code> tag for headings.`

### `<pre>`

- Preformatted text.
- Preserves spaces, line breaks, and formatting.
  Example:

```
Line 1
    Line 2 (indented)
Line 3
```

### `<blockquote>`

- Used for **long quotes** from another source.
- Usually indented.
  Example: `"The only limit to our realization of tomorrow is our doubts of today."`

### `<cite>`

- Marks the **title of a work** (book, movie, article).
- Usually italicized.
  Example: `<cite>The Great Gatsby</cite> was written by F. Scott Fitzgerald.`

### `<q>`

- For **short, inline quotes**.
- Browsers add quotation marks automatically.
  Example: `She said, <q>Always do your best.</q>`

**Quick Recap Table**

| Tag            | Purpose                    |
| -------------- | -------------------------- |
| `<span>`       | Inline container (styling) |
| `<code>`       | Inline code snippet        |
| `<pre>`        | Preformatted text block    |
| `<blockquote>` | Long external quote        |
| `<cite>`       | Title of a work            |
| `<q>`          | Short inline quote         |

**Rule of Thumb:**

- `<span>` → style small text
- `<code>` / `<pre>` → coding examples
- `<blockquote>` / `<cite>` / `<q>` → quotations
