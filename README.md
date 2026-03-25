# MD Stripper

A single-file HTML tool that converts Markdown into a clean, formatted preview — then copies it with real formatting (bold, italic, links) so you can paste directly into Google Docs or Word without any `**asterisks**` or `#` symbols.

## The Problem

Markdown is great for writing, but when you paste it into Google Docs, Notion, or an email, you get this:

```
## My Heading
**Bold text** and *italic text* and a [link](https://example.com)
```

Instead of the formatted version you actually wanted.

## The Solution

MD Stripper renders your markdown live and copies it as **rich HTML** — so paste into Docs and it just looks right.

## Features

- **Live preview** — renders as you type, side by side with your input
- **Rich copy** — copies formatted HTML so bold, italic, headings, and links survive the paste into Google Docs / Word
- **File upload** — drag & drop or click to upload a `.md` file
- **No dependencies** — single `.html` file, no install, no server, works offline
- **Word / line / char counts** on both input and output

## What Renders

| Markdown | Renders As |
|---|---|
| `**bold**` | **bold** |
| `*italic*` | *italic* |
| `[text](url)` | clickable link |
| `# Heading` | styled heading |
| `- list item` | bullet list |
| `> blockquote` | indented quote |
| `` `code` `` | inline code block |
| `---` | horizontal rule |
| `~~strike~~` | ~~strikethrough~~ |
| Tables | rendered table |

## Usage

1. Download `md-cleaner.html`
2. Open it in any browser
3. Paste your markdown or drag in a `.md` file
4. Click **Copy All** (or `Ctrl/Cmd + Shift + C`)
5. Paste into Google Docs, Word, Notion, email — formatted and clean

## No Install Required

This is a single self-contained `.html` file. No npm, no build step, no backend.

```bash
# Just open it
open md-cleaner.html
```

## Browser Support

Works in any modern browser (Chrome, Firefox, Safari, Edge). Rich copy uses the `ClipboardItem` API with a `document.execCommand` fallback for older browsers.

## License

MIT
