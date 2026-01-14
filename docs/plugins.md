# Plugin Catalog

## macOS Automation

| Plugin | Description | Install |
|--------|-------------|---------|
| [apple-notes](#apple-notes) | Interact with Apple Notes via JXA | `/plugin install apple-notes` |
| [send-to-kindle](#send-to-kindle) | Send EPUB/PDF to Kindle via Mail.app | `/plugin install send-to-kindle` |

## Financial Tools

| Plugin | Description | Install |
|--------|-------------|---------|
| [pacioli](#pacioli) | Generate financial documents | `/plugin install pacioli` |

---

## apple-notes

Interact with Apple Notes on macOS via JXA (JavaScript for Automation).

```bash
# Search notes
bunx @peerasak-u/apple-notes list "budget"
bunx @peerasak-u/apple-notes read-index "budget" 2

# Create note
bunx @peerasak-u/apple-notes create "Meeting Notes" "# Agenda\n- Item 1" "Work"

# Recent notes
bunx @peerasak-u/apple-notes recent 10
```

[View commands](../plugins/apple-notes-skills/skills/apple-notes/references/COMMANDS.md)

---

## send-to-kindle

Send EPUB and PDF files to Kindle via email using Apple Mail.app.

```bash
bunx @peerasak-u/send-to-kindle \
  --to=your-kindle@kindle.com \
  --from=your-email@gmail.com \
  --file=/path/to/book.epub
```

[View commands](../plugins/send-to-kindle-skills/skills/send-to-kindle/references/COMMANDS.md)

---

## pacioli

Generates professional financial documents (invoices, quotations, receipts) for freelancers using HTML templates and Puppeteer.

```bash
# Generate an invoice
bunx pacioli generate invoice invoices/oct-service.json --customer customers/acme.json

# Generate a quotation
bunx pacioli generate quotation quotations/web-design.json --customer customers/acme.json
```

[View schemas](../plugins/pacioli-skills/skills/pacioli/references/SCHEMAS.md)

---

[← Back to README](../README.md)
