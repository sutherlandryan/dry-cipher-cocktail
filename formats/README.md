# Dry Cipher — Formats Folder

This folder contains **machine-readable versions** of the Dry Cipher cocktail recipe for use in point-of-sale (POS) systems, automated bartender machines, and cocktail databases.

---

## 📂 Files

### **dry-cipher.json**
- **Use for:** Modern APIs, cocktail databases, and systems that can import structured JSON.
- **Why:** Includes all metadata (name, author, license, creation date, full ingredient list, and method).
- **Import tip:** Many bar inventory and cocktail apps (e.g., Mixology Tech, custom API scripts) can consume JSON directly.

---

### **dry-cipher.csv**
- **Use for:** Simple or legacy POS systems, spreadsheet management, and auto-bar pump mapping.
- **Why:** CSV is the most widely compatible format. Can be opened in Excel, Google Sheets, or imported into POS software.
- **Import tip:** Each row = one ingredient with its amount, unit, and notes.  
- **Header columns:** `Drink Name`, `Ingredient`, `Amount`, `Unit`, `Notes`

---

### **dry-cipher.xml**
- **Use for:** Automated bartender machines or systems with XML-based recipe import.
- **Why:** XML is still used in certain closed or proprietary bar systems (e.g., Barsys, Drinkworks, Bartesian).
- **Import tip:** The `<cocktail>` root element contains `<ingredients>` with `<ingredient>` child elements for each component.

---

## 📜 License
All formats are licensed under **CC BY-NC 4.0 (Creative Commons Attribution-NonCommercial 4.0 International)**.  
- **Non-commercial use allowed** with credit to **Ryan Sutherland**.  
- **Commercial use requires permission** from the author.  
[Full License Text](https://creativecommons.org/licenses/by-nc/4.0/)

---

## 🛠 Integration Notes
- **Grams-first measurement system**: All ingredients are listed in grams for quick use with pour-over scales.  
- **Volume equivalents** are included in the main README for ml/oz conversion.
- Keep ingredient names **exact** for best compatibility with inventory-mapped POS systems.

---

**Recipe Origin Date:** 2025-08-09  
**Author:** Ryan Sutherland  
