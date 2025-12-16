![Decks screen – last 30 days bar graph](screenshots/screenshot-1.png)

---

# Anki Bar Graph
*(Last 30 Days Review Bar Graph for Decks screen)*

🔗 **AnkiWeb**  
https://ankiweb.net/shared/info/1487842475

---

## What this add-on does

**Anki Bar Graph** displays your **recent review activity as a bar graph directly on the Decks screen**.

- No Statistics window
- Always visible
- Immediate feedback when you open Anki

By default, it shows your **recent review history**, helping you keep track of study momentum at a glance.

---

## Core Features

- 📊 Bar graph shown **directly on the Decks screen**
- 📅 Displays review counts for a configurable recent period
- 🔄 Automatically updates after review sessions
- 🎯 Optional **daily goal line**
- 🖱 Hover to see exact review counts per day
- 🪶 Lightweight and fast (cached DB access)

---

## 🆕 Recent Updates (Latest Features)

### 📆 Configurable date range

You can now choose how many days to display:

- 7 days  
- 30 days  
- 90 days  
- 180 days  
- 365 days  

This supports both **short-term habit tracking** and **long-term trend analysis**.

---

### 🎨 Full color customization (GUI color picker)

All colors can be configured via a **color picker UI** (no manual RGBA editing).

Customizable elements include:

- Past days bars  
- Today’s bar  
- Goal-achieved bars  
- Goal line  
- Background / border colors  

---

### 🧩 Unified color setting components

All color options use a shared internal **RGBA picker row**, providing:

- Consistent UI behavior
- Easier maintenance
- Predictable previews across settings

---

### 🖱 Improved scroll behavior (UX fix)

Mouse wheel / trackpad scrolling is **disabled on numeric and combo inputs** to prevent:

- Accidental value changes while scrolling
- Unintended edits in the settings dialog

Applies to:
- Spin boxes
- Combo boxes

---

### ⚡ Safer configuration handling

- Invalid values (e.g. unsupported range days) are auto-corrected
- Unknown config keys are preserved during updates
- **Reset to defaults** reliably restores the original state

---

## Configuration

Open:

**Tools → Add-ons → Bar Graph → Config**

Available options include:

- Enable / disable graph
- Display range (7–365 days)
- Daily review goal
- Bar width and spacing
- Chart height
- Full RGBA color customization (GUI)

For detailed descriptions, see `config.md`.

---

## Installation

### From AnkiWeb (recommended)

1. Open Anki  
2. Tools → Add-ons → Get Add-ons  
3. Enter the code from AnkiWeb  
4. Restart Anki  

👉 https://ankiweb.net/shared/info/1487842475

---

### Manual (GitHub)

1. Download or clone this repository  
2. Place it in:

   `Anki2/<profile>/addons21/anki-bar-graph/`

3. Restart Anki

---

## Performance Notes

- Queries only the selected recent range (max 365 days)
- Results are cached
- No background timers or polling
- Negligible impact even on large collections

---

## Compatibility

- Anki 24.x
- Anki 25.x
- Windows / macOS / Linux

---

## License

MIT License

---

## Author

Created by **@yuwayanagitani**

---

## Notes

- This add-on **does not modify cards, decks, or scheduling**
- The graph is shown **only on the Decks screen**
- Deleting `config.json` will recreate it with default values
