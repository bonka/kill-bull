# Slashes Bullets and Formatting

Exterminate bullet points and structural markdown with razor precision.

## Features

- **Bullet Point Assassination**: Eliminates bullet points (•, -, *, +, ‣, ◦, ▪, ▫, ⁃) while preserving content
- **Numbered List Termination**: Removes numbered lists (1. 2. 3. or 1) 2) 3) or (1) (2) (3))
- **Alphabetic List Elimination**: Destroys alphabetic lists (a. b. c. or a) b) c) or (a) (b) (c))
- **Structural Element Obliteration**: Optionally targets markdown headers, blockquotes, code blocks, and horizontal rules
- **Indentation Destruction**: Removes hierarchical tabulation when enabled
- **Mode Shortcuts**: Quick access to common killing patterns

## Usage

### Basic Operation
- Select text or have text in clipboard
- Run the extension
- Cleaned text replaces selection or gets copied to clipboard

### Mode Shortcuts
Use the mode argument for quick presets:

- `a` or `all` - Kill everything (nuclear option)
- `l` or `lists` - Target only list elements (bullets, numbers, letters)
- `s` or `structure` - Eliminate structural elements, spare lists
- `h` or `headers` - Silent strike: headers only
- `q` or `quotes` - Silent strike: blockquotes only
- `c` or `code` - Silent strike: code blocks only
- `r` or `rules` - Silent strike: horizontal rules only
- `i` or `indentation` - Silent strike: indentation only

### Preferences
Configure what gets spared or targeted:

**Have mercy on…**
- Bullets: Spare bullet points (•, -, *)
- Numbers: Grant passage to numeric order (1. 2. 3.)
- Letters: Show clemency to alphabetic procession (a, b, c)

**Also target…**
- Headers: Slice markdown headers (#, ##, ###) with prejudice
- Blockquotes: Target blockquotes (>) for termination
- Code: Obliterate code blocks (```)
- Rules: Chop horizontal rules (---, ***) into pieces
- Indentation: Destroy hierarchical tabulation

## Examples

**Before:**
```
• First bullet point
  - Nested bullet
    1. Numbered item
    2. Another number
# Header
> Blockquote
```

**After (default settings):**
```
First bullet point
  Nested bullet
    1. Numbered item
    2. Another number
# Header
> Blockquote
```

**After (mode: "a"):**
```
First bullet point
Nested bullet
Numbered item
Another number
Header
Blockquote
```

## Installation

Install from the Raycast Store or build from source.

## Development

```bash
npm install
npm run dev
```

## License

MIT
