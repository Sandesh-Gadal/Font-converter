# Himalaya TT Font → Nepali Unicode Converter

A lightweight, offline web-based tool to convert legacy **Himalaya TT / Himali-style font encoded text** into standard **Nepali Unicode**.  
This helps convert old documents created in MS Word, PageMaker, Photoshop, and other legacy tools into modern Unicode text usable on web, mobile, and social platforms.

---

## 🌟 Features

- 🔄 Converts Himalaya TT / legacy Nepali font encoding to Unicode
- ⚡ Real-time auto conversion while typing
- 📋 Copy converted text to clipboard
- 💾 Download output as `.txt` file
- 🔢 Option to use English digits (0–9) or Nepali digits (०–९)
- 📴 Fully offline (no internet required)
- 📱 Responsive UI for mobile and desktop

---

## 🖥️ Demo

Open the `index.html` file in any browser.

---

## 🚀 How to Use

1. Download or clone this repository
2. Open `index.html` in a browser (Chrome, Firefox, Edge)
3. Paste your Himalaya TT / legacy encoded text into the left panel
4. The converted Unicode text appears on the right panel automatically

### Buttons:

- **Convert to Unicode** → Manually trigger conversion
- **Copy Unicode** → Copy converted text to clipboard
- **Download .txt** → Save output as a text file
- **Clear** → Reset both input and output fields

---

## ⚙️ Options

### Auto Convert
- Automatically converts text while typing
- Enabled by default

### Use English Digits
- Converts numbers to 0–9 instead of Nepali digits (०–९)

---

## 🧠 How It Works

The converter uses a two-step conversion process:

### 1. Character Mapping
Each character from the Himalaya TT encoding is mapped to its Unicode equivalent using a JavaScript lookup table (`HIMALAYA_MAP`).

### 2. Unicode Cleanup
After mapping, the script fixes common Nepali script issues such as:

- Incorrect vowel positioning (ि, ी, ो, ौ)
- Reordering consonant clusters
- Handling “reph” (र्) placement
- Removing duplicate vowel signs
- Normalizing Unicode output (NFC)

---

## 📁 Project Structure

```plaintext
index.html   → Complete standalone application (HTML + CSS + JavaScript)
