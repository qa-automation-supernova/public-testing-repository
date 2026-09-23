# MD Comprehensive Test Fixture

This file is a broad **Markdown** test fixture. It intentionally stays within ordinary Markdown/CommonMark/GFM-style syntax and does **not** contain JSX, React components, or executable JavaScript.

## 1. Headings

# Heading 1

EDITED again

## Heading 2

### Heading 3

#### Heading 4

##### Heading 5

###### Heading 6

Setext Heading 1
=================

Setext Heading 2
-----------------

## 2. Paragraphs and inline formatting

This is a normal paragraph with **bold text**, *italic text*, ***bold italic text***, ~~strikethrough~~, `inline code`, and an [inline link](https://example.com).

Here is a [link with a title](https://example.com "Example title").

You can also write an autolink: <https://example.com> and an email autolink: <mailto:test@example.com>.

Escaped punctuation: \*asterisk\* \_underscore\_ \[brackets\] \#hash \`backtick\`.

Hard line break here  
and the next line continues the same paragraph.

## 3. Links

### Inline links

- [Example](https://example.com)
- [Example with title](https://example.com "Example title")
- [Relative link](./relative/path.md)
- [Anchor link](#headings)

### Reference-style links

This uses a [reference link][docs].

This uses a [collapsed reference][] link.

This uses a [shortcut reference].

[docs]: https://example.com/docs "Documentation"
[collapsed reference]: https://example.com/collapsed
[shortcut reference]: https://example.com/shortcut

## 4. Images

![Markdown logo](https://upload.wikimedia.org/wikipedia/commons/4/48/Markdown-mark.svg "Markdown")

Reference-style image:

![A reference image][md-image]

[md-image]: https://upload.wikimedia.org/wikipedia/commons/4/48/Markdown-mark.svg "Reference image"

## 5. Unordered lists

- First item
- Second item
  - Nested item
  - Another nested item
    - Third-level item
- Final item

Using asterisks:

* Alpha
* Beta
  * Nested beta

Using plus signs:

+ One
+ Two
  + Nested two

## 6. Ordered lists

1. First
2. Second
3. Third

Nested ordered list:

1. Outer one
   1. Inner one
   2. Inner two
2. Outer two

Non-sequential source numbering:

1. First
4. Second
9. Third

## 7. Task lists / checkboxes

- [x] Completed task
- [ ] Open task
- [X] Completed with uppercase X

Nested tasks:

- [x] Parent task
  - [ ] Child task
  - [x] Another child task

## 8. Blockquotes

> This is a blockquote.

Nested blockquote:

> Outer quote
>
> > Nested quote
> >
> > With a second paragraph.

Blockquote with formatting:

> **Bold**, *italic*, and `code` inside a quote.

## 9. Code

### Inline code

Use `npm install` to install dependencies.

### Fenced code block: plain

```
plain text
line two
line three
```

### Fenced code block: JavaScript

```js
function greet(name) {
  return `Hello, ${name}!`;
}

console.log(greet('Markdown'));
```

### Fenced code block: JSON

```json
{
  "name": "markdown-fixture",
  "enabled": true,
  "items": [1, 2, 3]
}
```

### Fenced code block: HTML

```html
<section class="example">
  <h2>Hello</h2>
  <p>Markdown code fixture.</p>
</section>
```

### Indented code block

    function indentedExample() {
      return 'four spaces';
    }

## 10. Horizontal rules

---

***

___

## 11. Tables

### Basic table

| Name | Type | Enabled |
| --- | --- | --- |
| Alpha | A | Yes |
| Beta | B | No |
| Gamma | C | Yes |

### Aligned table

| Left | Center | Right |
| :--- | :---: | ---: |
| A | B | C |
| 1 | 2 | 3 |
| 4 | 5 | 6 |

### Table with formatting

| Feature | Example | Notes |
| :--- | :--- | :--- |
| **Bold** | **text** | Strong emphasis |
| *Italic* | *text* | Emphasis |
| `Code` | `value` | Inline code |
| [Link](https://example.com) | Link | Destination |

## 12. HTML blocks and inline HTML

<div class="markdown-html-example">
  <strong>Inline HTML content</strong>
  <p>This is an HTML block embedded in Markdown.</p>
</div>

Line with <span data-example="true">inline HTML</span> content.

<details>
<summary>Expandable HTML details</summary>

This is hidden until expanded.

</details>

## 13. Escaping and special characters

Escaped characters:

\# Not a heading

\* Not emphasis\*

\_ Not emphasis\_

\> Not a blockquote

\- Not a list item

\[Not a link\]

\`Not inline code\`

## 14. Entities and symbols

HTML entities: &copy; &amp; &lt; &gt; &quot;

Symbols: © ™ ® € £ ¥ § ± × ÷ → ← ↑ ↓

## 15. Whitespace and blank lines

Paragraph one.


Paragraph two after extra blank lines.

## 16. Nested formatting

***Bold italic***

**Bold with _nested italic_**

*Italic with **nested bold***

~~Strikethrough with **bold** and *italic*~~

## 17. Long paragraph

Markdown is often used for documentation, notes, README files, changelogs, knowledge bases, and content pipelines. This paragraph is intentionally longer so that renderers can be tested with ordinary prose wrapping, punctuation, repeated inline formatting, and a mixture of short and long words. It should remain a single paragraph while still exercising realistic text layout and line-wrapping behavior across different viewports.

## 18. Definition-like content

Term
: Definition text associated with the term.

Another term
: A second definition.

## 19. Escaped and literal Markdown patterns

The following text should remain literal:

\# heading-like text

\- list-like text

\[link-like text\](https://example.com)

\*emphasis-like text\*

## 20. URLs and protocol examples

- https://example.com
- http://example.com/path?q=1&sort=asc
- mailto:test@example.com
- tel:+1-555-0100

## 21. Unicode and multilingual text

English — Français — Deutsch — Español — Português — 日本語 — 한국어 — 中文 — العربية — हिन्दी

Emoji: 😀 🚀 ✅ ⚠️ 🔥 🧪

## 22. Special characters inside code

`<component />`

`{ "key": "value" }`

`const x = a && b ? c : d;`

## 23. Code fence edge cases

~~~python
def square(value):
    return value * value
~~~

```text
A fenced block using a text language identifier.
```

## 24. Mixed content

> ## Mixed blockquote
>
> 1. Ordered item
> 2. Another item
>
> ```js
> const quoted = true;
> ```
>
> And a [quoted link](https://example.com).

- List item with a quote:
  > Nested quote inside a list.

- List item with code:

  ```bash
  echo "nested code"
  ```

## 25. Empty-ish and minimal structures

A minimal paragraph.

---

Another paragraph after a rule.

## 26. Footnote-style syntax (where supported)

A sentence with a footnote reference.[^1]

Another reference.[^long-note]

[^1]: This is the first footnote.
[^long-note]: This is a longer footnote definition that can contain **formatting** and a [link](https://example.com).

## 27. Final coverage sample

# Final Heading

This final section combines **bold**, *italic*, `inline code`, a [link](https://example.com), a task item, and a small table.

- [x] Markdown syntax parsed
- [ ] Rendering verified

| Key | Value |
| --- | --- |
| format | md |
| jsx | unsupported |
| react | unsupported |
| interactivity | external implementation required |

> Markdown itself is declarative text. Interactivity typically comes from the renderer, surrounding application, JavaScript, or embedded HTML rather than from Markdown syntax alone.
