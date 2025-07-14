# Kill Bull

Remove bullet points and markdown elements from the beginning of lines in clipboard text or selected text. Perfect for cleaning up messy text copied from chatbots, webpages etc. 

## Overview

Kill Bull's **default behavior** is to slash list items such as bullet points, sequential numbers, and letters. It's can also be set to target **structural markdown** elements such as headers, blockquotes, code blocks, horizontal rules, and indentation.

The default behavior can be customized in two ways:
1. **Settings menu** - Configure persistent preferences for what elements to target
2. **Command arguments** - Use inline commands like `kill bull headers` for single-use

### Targeting Modes
- **Default mode** - Without arguments – follows modes set in preferences.
- **Full Assault** - Wider targeting that hits groups of elements.
- **Silent Strike** - Precise targeting of specific structural markdown elements only.

## Features

- **Smart text detection**: Automatically processes selected text or clipboard content.
- **Default behavior**: Removes all bullet points and list markers
- **Multiple bullet types**: Supports `•`, `-`, `*`, `+`, `‣`, `◦`, `▪`, `▫`, `⁃` bullet points
- **List markers**: Removes all variations of numbered and lettered lists (1., 1), (1), A., A), (A), a., a), (a))
- **Cross-platform text**: Normalizes line endings from different operating systems
- **Direct replacement**: When text is selected, it gets replaced immediately
- **Clipboard processing**: When no text is selected, processes clipboard content

## Quick Mode Arguments

Kill Bull accepts quick mode arguments with fuzzy matching - just type the first letter(s) of the mode:

**Note**: Kill Bull only removes structural block elements, not inline markdown formatting, like `**bold**` or `[links](url)`.

### Full Assault (Multiple targets)
- `a` / `all` - Destroys all structural block elements
- `l` / `lists` - Targets all list elements (bullets, numbers, letters)
- `s` / `structure` - Targets all structural elements (headers, quotes, code, rules)

### Silent Strike (Individual targeting)
- `h` / `headers` - Only headers (#, ##, ###)
- `q` / `quotes` - Only blockquotes (>)
- `c` / `code` - Only code blocks (```)
- `r` / `rules` - Only horizontal rules (---, ***)
- `i` / `indent` - Only indentation

Just type `kill bull a` or `kill bull all` - both work! Fuzzy matching means `h`, `he`, `headers` all work for headers mode.

**Default behavior can be customized in the extension settings** to target a wider or more narrow range of elements, without using mode arguments.

## Usage

1. **With selected text**: Select text containing bullet points → Run Kill Bull → Text is instantly replaced with cleaned version
2. **With clipboard**: Copy text with bullet points → Run Kill Bull → Cleaned text replaces clipboard content

### Before (default behavior)
    • First bullet point 
        * Nested bullet
    1. Numbered list

### After
    First bullet point
        Nested bullet
    Numbered list
        

## Opt-out Features

By default, Kill Bull removes all ordered and unordered list markers. You can customize its behavior in Raycast preferences to spare certain elements. Check these preferences to "ON" to spare:

- Spare **Bullet**: Keep bullet characters (•, -, *, +)
- Spare **Numbers**: Keep numbered list markers (1., 1), (1), A., A), (A))
- Spare **Letters**: Keep letter list markers (a., a), (a))

## Opt-in Features

Additional markdown elements can be removed either by inline shortcut, or as default, by opting in enabling these preferences:

- Kill **Headers**: Remove markdown headers (#, ##, ###)
- Kill **Quotes**: Remove markdown blockquotes (>)
- Kill **Code**: Remove code blocks (```, `)
- Kill **Rules**: Remove horizontal rules (---, ***)

When a checkbox is checked, the corresponding element will be removed every time Kill Bull is run without arguments. When unchecked, the element will be preserved.

---

*Kill Bull — The silent warrior’s path to spotless content..* 🗡️