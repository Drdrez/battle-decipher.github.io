Here is a professional, Markdown-formatted `README.md` for your GitHub repository. You can copy this directly into your repo.

---

# 🔐 Battle Decipher v2.0

**A lightweight, single-file browser tool designed for Capture The Flag (CTF) competitions and encryption battles.**

## ⚡ Overview

**Battle Decipher v2.0** is a standalone utility built with standard HTML, CSS, and JavaScript. It requires **no server, no installation, and no internet connection** to run. It is optimized for speed, allowing competitors to quickly brute-force, analyze, and decrypt classic ciphers entirely in the browser.

## 🚀 Getting Started

1. **Download:** Clone this repo or download the `decoder.html` file.
2. **Run:** Double-click the file to open it in any modern web browser (Chrome, Edge, Firefox).
3. **Decrypt:** Paste your ciphertext into the appropriate tab and strike!

## 🛠 Features

### 1. Caesar / Shift Cipher Breaker

* **Brute Force Engine:** Instantly generates all 25 possible shifts.
* **Real-time Frequency Analysis:** Visual bar chart identifies the most common letters (likely 'E' or 'A') to help you spot the key without reading every line.

### 2. XOR / One-Time Pad Solver

* **Dual Input Modes:** Handles both **Text** strings and **Hex** values (e.g., `1A 2B 3C`).
* **Bitwise Logic:** Performs standard XOR operations against a provided key.

### 3. Columnar Transposition

* **Keyword-Based Decryption:** Reconstructs the grid based on the alphabetical order of a keyword.
* **Smart Grid Logic:** Automatically handles irregular column lengths.

### 4. Rail Fence (Zig-Zag) Cipher

* **Multi-Rail Support:** Decodes zigzag patterns for 2 to 10 rails.

### 5. Quick Tools Suite (Sidebar)

* **Trim & Remove Spaces:** Critical for cleaning input before transposition attacks.
* **Reverse Text:** Flips strings instantly.
* **Uppercase:** Standardizes input for better readability.
* **Base64 Decode:** One-click decoding for standard Base64 strings.

## ⚔️ Battle Tactics (How to Win)

* **Spotting Caesar:** Look for single letters standing alone. If you see `X` as a single word, it is likely `A` or `I`. Use the **Frequency Chart**—the tallest bar is usually `E`.
* **Spotting XOR:** If the clue is a string of numbers or hex codes (e.g., `4F 12...`), go straight to the **XOR** tab. Ensure "Is input Hex?" is checked.
* **Spotting Transposition:** If the letter frequency looks normal (lots of E's and T's) but the words are jumbled, it is a transposition. **Remove spaces** before decrypting.
* **Spotting Base64:** If the string ends with `==`, click **Base64 Decode** in the sidebar immediately.

## 📝 Modification

Since this is a single HTML file, you can add new features easily:

1. Open `decoder.html` in any text editor (VS Code, Notepad++, etc.).
2. Add a new `<div class="tab">` for your navigation.
3. Add a new `<div class="panel">` for your logic.
4. Write your JavaScript function in the `<script>` section.
