# Images (`<img>` tag)

The `<img>` tag is used to **embed images into a webpage**. Unlike most tags, it is **self-closing** (doesn’t need `</img>`).

- **`src` (Source)** → Defines the **path or URL** of the image.

  - Can be **relative** (same folder/subfolder) or **absolute** (full URL).

- **`alt` (Alternative text)** → Text description of the image if it can’t be displayed.

  - Helps with **accessibility** (screen readers for visually impaired users).
  - Important for **SEO**.

- **`title` (Tooltip)** → Shows extra info when hovering over the image.
- **`width` / `height`** → Set the **size of the image** (in pixels or percentages).

---

# Lists

### Unordered List (`<ul>`)

- Displays items with **bullets**.

```html
<ul>
  <li>Apples</li>
  <li>Oranges</li>
</ul>
```

### Ordered List (`<ol>`)

- Displays items with **numbers** (or letters/roman numerals).

```html
<ol>
  <li>Step one</li>
  <li>Step two</li>
</ol>
```

### Description List (`<dl>`)

- Used for **terms and definitions** (like a glossary).

  - `<dt>` → Definition Term
  - `<dd>` → Definition Description

```html
<dl>
  <dt>HTML</dt>
  <dd>HyperText Markup Language</dd>
</dl>
```

---

# Basic Form Elements

A group of html tags related to gathering data from a user. This will be a combination of input, textarea, and select tags. You can then use this form element to send that data to your server. A form tag itself doesn't show anything; it's a just a container for the other tags.

### `<form>`

- Container for all form elements.
- Where **users enter data** to be sent somewhere (like a server).
- Important attributes:

  - **`action`** → where the data goes (URL/server).
  - **`method`** → how data is sent (`GET` or `POST`).

---

### `<input>`

Gather information from the users

- Element for user input (type changes behavior).
- Common attributes:

  - **`type`** → text, password, email, checkbox, radio, file, etc.
  - **`name`** → key used to send the data.
  - **`placeholder`** → hint text inside the field.
  - **`value`** → default value or button text.

**different types of inputs ....**

- `<input type="color" />`
- `<input type="file" />`
- `<input type="number" />`
- `<input type="datetime-local" />`
- `<input type="radio" />`
- `<input type="checkbox" />`
  can use radio buttons or select .. more prefered is radio ...

---

### `<textarea>`

Comment area and long form texts. So for example on reddit.

- For **long text inputs** (comments, messages).
- Attributes:

  - **`rows`** → height in lines.
  - **`cols`** → width in characters.

Example:

```html
<form>
  <label for="message">Message:</label>
  <textarea
    id="message"
    name="message"
    rows="5"
    cols="30"
    placeholder="Write your message..."
  ></textarea>
</form>
```

---

### `<button>`

- More flexible than `<input type="submit">`.
- Types:

  - **`type="submit"`** → sends the form.
  - **`type="reset"`** → clears the form.
  - **`type="button"`** → just a clickable button (no default action).

---

### `<label>`

- Makes forms **accessible and clickable**.
- Always connect with the `for` attribute → must match the input’s `id`.
- Clicking the label focuses the input (good UX).
- Diff between id and name. Name is associated with the processing script - normally not a front-end job.

Example:

```html
<label for="email">Email:</label> <input type="email" id="email" name="email" />
```

---

# HTML Attributes and Syntax

- Attributes provide **extra information** about an element.
- They are written **inside the opening tag**.
- Example:

```html
<img src="logo.png" alt="Website Logo" width="100" />
```

---

# Comments in HTML

- Comments are **notes in your code that the browser ignores**.
- Useful for:

  - Explaining code
  - Temporarily hiding code
  - Leaving reminders

Example:

```html
<!-- This is a comment -->
```
