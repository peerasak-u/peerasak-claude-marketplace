# Send to Kindle - Commands Reference

## Command Syntax

```bash
bunx @peerasak-u/send-to-kindle [options]
```

## Options

| Option | Required | Description | Default |
|--------|----------|-------------|---------|
| `--to` <email> | Yes | Recipient email address (your Kindle email) | - |
| `--from` <email> | Yes | Sender email address (must be approved in Amazon account) | - |
| `--file` <path> | Yes | Path to the file to attach (EPUB, PDF, etc.) | - |
| `--subject` <text> | No | Subject prefix for the email | "Daily News" |
| `--message` <text> | No | Body message for the email | - |
| `--help` | No | Show help message | - |
| `--version` | No | Show version number | - |

## Usage Examples

### Basic Usage

Send an EPUB file to Kindle:

```bash
bunx @peerasak-u/send-to-kindle \
  --to=your-kindle@kindle.com \
  --from=your-email@gmail.com \
  --file=/path/to/book.epub
```

### Send with Custom Subject

```bash
bunx @peerasak-u/send-to-kindle \
  --to=your-kindle@kindle.com \
  --from=your-email@gmail.com \
  --file=/path/to/document.pdf \
  --subject="Monthly Report"
```

### Send with Message Body

```bash
bunx @peerasak-u/send-to-kindle \
  --to=your-kindle@kindle.com \
  --from=your-email@gmail.com \
  --file=/path/to/book.epub \
  --message="Here's the book I mentioned. Enjoy reading!"
```

### Send PDF to Kindle

```bash
bunx @peerasak-u/send-to-kindle \
  --to=your-kindle@kindle.com \
  --from=your-email@gmail.com \
  --file=/Users/username/Documents/article.pdf \
  --subject="Article to Read"
```

## Getting Help

Display help message:

```bash
bunx @peerasak-u/send-to-kindle --help
```

Show version:

```bash
bunx @peerasak-u/send-to-kindle --version
```

## Notes

- The `--to` email must be your Kindle email address (found in your Amazon account settings)
- The `--from` email must be approved in your Amazon account's "Approved Personal Document E-mail List"
- Supported file formats include EPUB, PDF, and other formats supported by Kindle
- Apple Mail.app must be configured and working on your Mac
