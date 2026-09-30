# Day-1
Introduction of HTML
**What HTML is**
HTML (HyperText Markup Language) is not a programming language — it's a markup language. It describes structure and content: what's a heading, what's a paragraph, what's a container. Browsers read this and render it visually. It has no logic, no calculations — just structure.

**Tags — the basic building block**
A tag is a keyword in angle brackets. Most come in pairs: an opening tag and a closing tag, wrapping content.

```html
<p>This is a paragraph.</p>
```

Some tags don't wrap anything and don't need a closing tag — void/self-closing tags:

```html
<img src="photo.jpg" alt="A photo">
<br>
<hr>
```

**Tag vs Element**

- Tag = the keyword itself, e.g. `<p>`
- Element = the whole unit — opening tag + content + closing tag, e.g. `<p>Hello</p>`

Used interchangeably in casual talk, but technically different.

**Attributes**
Extra info inside the opening tag, written as `name="value"`.

```html
<img src="cat.jpg" alt="A cat">
```

`src` and `alt` here are attributes.

**Basic HTML document structure**

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My First Page</title>
  </head>
  <body>
    <h1>Hello World</h1>
    <p>This is my first webpage.</p>
  </body>
</html>
```

- `<!DOCTYPE html>` — declares this is HTML5. Always the first line, not a tag itself.
- `<html>` — root element, everything lives inside it.
- `<head>` — metadata, not visible on the page (title, later: CSS links, meta tags).
- `<title>` — text shown on the browser tab.
- `<body>` — everything visible goes here.

**Tags to introduce today (structure only — not their full usage)**
Just enough vocabulary so structure makes sense:

| Tag | Purpose |
| --- | --- |
| `<html>` | Root of the page |
| `<head>` | Metadata container |
| `<title>` | Browser tab text |
| `<body>` | Visible content container |
| `<h1>` | A heading (just to show *some* tag in action) |
| `<p>` | A paragraph |
| `<div>` | Generic block container — no meaning on its own |

Don't go into lists, links, images, tables today — that's the rest of the week.

**Nesting rule**
Tags can go inside other tags, but must close in reverse order — like brackets.

```html
<!-- correct -->
<div>
  <p>Text</p>
</div>

<!-- wrong -->
<div>
  <p>Text</div>
</p>
```

**Comments**

```html
<!-- This won't show on the page, only in the code -->
```

**Common mistakes on day one**

- Forgetting `<!DOCTYPE html>` at the top
- Mixing up `<head>` and `<body>` — putting visible text in `<head>`
- Not closing tags properly, especially nested ones
- Writing tags in uppercase inconsistently — HTML isn't case-sensitive but lowercase is the convention everyone follows

**Small practice task**
Create a basic `.html` file with:

- Correct doctype
- A `<title>` of their choice
- One `<h1>` and one `<p>` inside `<body>`
- Open it in the browser and see it render
