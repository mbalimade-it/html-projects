# Document Outline and Heading Hierarchy

Think of your HTML document like a book:

- A **book** has chapters, sections, sub-sections, etc.
- Your **HTML page** also needs this structure so that people (and machines) can understand what’s important and how content is organized.

### Heading Hierarchy (H1 → H6)

HTML gives us six levels of headings:

- `<h1>` → Main title (the most important heading, used **once per page**)
- `<h2>` → Section titles (big divisions of your content)
- `<h3>` → Sub-sections under `<h2>`
- `<h4>` → Sub-sub-sections, and so on up to `<h6>`

The rule: **Headings are nested like a tree**. Don’t jump from `<h1>` to `<h4>` randomly. Always follow the hierarchy.

Why is This Important?

1. **Accessibility** → Screen readers use headings to let visually impaired users “jump” through sections.
2. **SEO (Google Search)** → Google loves clean hierarchy. It helps rank your page better.
3. **Readability** → Users scan pages quickly. Headings make it easier to digest.
4. **Maintainability** → Your code looks clean and logical.

_the example code shows the hierachy of headings using a recipe page_

---

# Semantic HTML5 Elements

What is “Semantic HTML”?

- **Semantic = Meaningful.**
- Semantic elements **describe their purpose** to both the browser and humans.

Before HTML5 (around early 2000s), developers mostly used `<div>` and `<span>` for everything.

`<div>` = a box or container (but has no meaning).

`<span>` = inline container (also meaningless by itself).

#### The problems it created:

- Search engines couldn’t easily understand which part was the main content vs. sidebar.
- Screen readers for visually impaired users struggled, since everything was just “div, div, div.”
- Developers had messy code, relying on IDs and classes just to explain structure.

Example:

- `<div>` → just a box, no meaning.
- `<header>` → clearly a page or section header.

Semantic HTML makes your code easier to read, improves **SEO**, and helps **screen readers** understand your page.

### The Key Semantic HTML5 Elements

1. `<header>`

   - The **top part** of a page or section.
   - Usually contains: logo, site title, navigation links.

2. `<nav>`

   - Used specifically for **navigation links**.
   - Can be inside `<header>` or stand alone.

3. `<main>`

   - The **main content** of your page.
   - Only **one `<main>`** per page!
   - Skips repeated things like headers, sidebars, footers.

4. `<section>`

   - Groups related content into **sections**.
   - Think of it like **chapters** in a book.

5. `<article>`

   - A **self-contained piece** of content that could stand alone (like a blog post, news article, or forum entry).

6. `<aside>`

   - Content **related but not main**: sidebars, ads, “did you know?” boxes.

7. `<footer>`

   - The **bottom section** of a page or section.
   - Usually has contact info, copyright, links.

### Why This is Better than Just `<div>`s?

More clear than just using divs.

---

# Figure and Figcaption Elements

- `<figure>` → a container that groups media (like an image, video, or illustration) with its caption.
- `<figcaption>` → the actual caption/description text that goes with the figure.

---

# Time Element with Datetime Attribute

The `<time>` element is used to **represent dates, times, or both** in your HTML.

It does two jobs at the same time:

1. Shows a **human-friendly version** of the date/time to users.
2. Stores a **machine-readable version** (using the `datetime` attribute) so browsers, search engines, and apps can understand it properly.

That way Google could show this in a calendar snippet and a calendar app could pick it up and add the event.

### Why it’s important:

1. **Accessibility** → Screen readers know it’s a date/time, not just text.
2. **SEO** → Search engines can parse events and schedules better.
3. **Future-proofing** → Browsers or apps can do smart things, like showing local time zones, reminders, or integrating with calendars.
4. **Clarity** → Other developers instantly see that this is a time-related value, not random text.

---

# Address Element

The `<address>` element is used to represent **contact details** for:

- A person,
- A business, or
- The author/owner of a web page or article.

It usually includes things like:

- Physical addresses,
- Email addresses,
- Phone numbers,
- Links to social profiles,
- Or any other relevant contact info.

Important to know:

1. **Not just physical addresses!**
   It can be email, phone, or even a Twitter handle.

2. **Not for random content**
   Don’t use `<address>` just for formatting.

---

# Div and Span for Layout Hook

- **`<div>`** = a block-level container.
  → It takes up the whole width of the page, stacking on top of other elements.
- **`<span>`** = an inline container.
  → It only takes up as much space as its content, sitting inside a line of text.

They don’t _mean_ anything (unlike `<header>` or `<footer>`). Their job is to **group elements** or **target them with CSS/JavaScript**.

---

# Progress and Meter Elements

## The `<progress>` Element

The `<progress>` element shows **how much of a task is completed**.
It’s usually used for **loading bars, file uploads, or task progress**.

## The `<meter>` Element

The `<meter>` element represents a **measurement within a known range** (a scalar value).
It’s great for **scores, ratings, capacity, or sensor readings**.

## Difference between `<progress>` and `<meter>`

- **`<progress>`** → "How far are we along in a process?"
  (loading, downloading, completing steps).
- **`<meter>`** → "What’s the current measurement in a range?"
  (score out of 10, battery percentage, disk space usage).

Easy way to remember:

- `<progress>` = **ongoing task**.
- `<meter>` = **status reading**.

---

# Details and Summary Elements

- **`<details>`** → a container that can expand/collapse to show extra content.
- **`<summary>`** → the visible heading or “label” you click to expand/collapse the `<details>`.

If no `<summary>` is provided, browsers just show a default “disclosure triangle” or “Details” text.
