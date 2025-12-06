# UST Bannu ID Card Generator & PSD Exporter

**Developed by [@muhibkhan123](https://github.com/muhibkhan123)**

![Project Status](https://img.shields.io/badge/Status-Stable-success)
![License](https://img.shields.io/badge/License-MIT-blue)
![Version](https://img.shields.io/badge/Version-1.0.0-orange)

A comprehensive, client-side web application designed to generate professional Student ID Cards for the **University of Science & Technology Bannu (USTB)**. 

Unlike standard generators that only produce flat images, this tool features a **Layered PSD (Photoshop) Export** engine, allowing administrators to download fully editable files directly from the browser.

---

## 📋 Table of Contents

- [Key Features](#-key-features)
- [Tech Stack](#-tech-stack)
- [Installation & Setup](#-installation--setup)
- [Usage Guide](#-usage-guide)
- [Troubleshooting (Common Issues)](#-troubleshooting-common-issues)
- [Customization](#-customization-for-developers)
- [Disclaimer](#-disclaimer)

---

## ✨ Key Features

### 1. Advanced Export Options
* **Layered PSD Export:** Uses the `ag-psd` library to generate Photoshop files where text, background patterns, and images remain on separate layers. This allows for post-processing adjustments.
* **High-Res PNG:** Uses `html2canvas` to capture a pixel-perfect render of the card for quick printing.

### 2. Security & Design
* **Pattern Randomizer:** Includes a "Pick Random Pattern" button that generates complex vector background patterns (Waves, Geometric, Isometric, etc.) to simulate security watermarks.
* **Dynamic Barcodes:** Automatically converts the Student ID into a scannable Code 39 barcode.

### 3. Dynamic Inputs
* **Dual-Side Generation:** Updates Front and Back cards simultaneously in real-time.
* **Image Handling:** Supports drag-and-drop or file selection for:
    * Student Photo
    * Registrar Signature
    * University Logos (Front & Back)

---

## 🛠 Tech Stack

This project is built entirely on the **Client-Side**, meaning it requires no backend server (Node.js/PHP) to run.

* **Structure:** HTML5
* **Styling:** [Tailwind CSS](https://tailwindcss.com/) (via CDN)
* **Icons:** FontAwesome
* **Fonts:** Google Fonts (Roboto Condensed, Libre Barcode 39)
* **Core Libraries:**
    * `html2canvas.js` (Screen capture)
    * `ag-psd.js` (PSD construction)

---

## 🚀 Installation & Setup

Since this is a standalone HTML file, installation is instant.

### Option 1: Git Clone
1.  Open your terminal/command prompt.
2.  Run the following command:
    ```bash
    git clone [https://github.com/muhibkhan123/ust-id-card-generator.git](https://github.com/muhibkhan123/ust-id-card-generator.git)
    ```
3.  Navigate to the folder:
    ```bash
    cd ust-id-card-generator
    ```
4.  Open `index.html` in your browser (Chrome, Edge, or Firefox recommended).

### Option 2: Direct Download
1.  Download the ZIP file from this repository.
2.  Extract it to your desktop.
3.  Double-click `index.html`.

> **⚠️ Important:** You must have an active internet connection when opening the file, as it loads Tailwind CSS and Fonts from online servers (CDNs).

---

## 📖 Usage Guide

1.  **Enter Student Data:** Fill in the form on the left side (Name, FName, Discipline, etc.). The card preview updates instantly.
2.  **Upload Photos:**
    * Click **"Student Photo"** to upload the student's picture.
    * Click **"Signature"** to upload the Registrar's signature (transparent PNG recommended).
3.  **Security Pattern:** If the background looks too plain, click the **"Pick Random Pattern"** button until you find a design you like.
4.  **Adjust Back Layout:** If the address or details on the back are overlapping, use the **"Back Bottom Spacing"** slider to adjust the padding.
5.  **Download:**
    * **Download PNG:** For immediate printing.
    * **Layered PSD:** If you need to edit the text later in Photoshop.

---

## 🔧 Troubleshooting (Common Issues)

If you face any problems, check this list first.

### 1. "The styling/design looks broken."
* **Cause:** You are likely offline.
* **Solution:** This tool uses Tailwind CSS via a CDN link. Connect to the internet and refresh the page to load the styles.

### 2. "The exported image is blank" or "Security Error".
* **Cause:** Browser security (CORS) restricts saving images if they are loaded from external URLs without permission.
* **Solution:** * Ensure you are uploading images using the "Choose File" buttons rather than trying to modify the HTML `src` code directly.
    * If you are a developer, try running the file on a local server (e.g., Live Server in VS Code) instead of just double-clicking the HTML file.

### 3. "The Barcode isn't showing in the downloaded image."
* **Cause:** The font file hasn't finished loading before the download started.
* **Solution:** Wait 2-3 seconds after opening the page before clicking download.

---

## 💻 Customization (For Developers)

If you want to change the default values (so you don't have to type them every time):

1.  Open `index.html` in a code editor (like VS Code or Notepad++).
2.  Search for `value=` inside the input tags.
    * *Example:* To change the default session from "Fall-2022" to "Spring-2025":
    * **Find:** `<input type="text" id="inSession" value="Fall-2022" ...>`
    * **Replace with:** `<input type="text" id="inSession" value="Spring-2025" ...>`
3.  Save the file and refresh your browser.

---

## ⚠️ Disclaimer

This tool is created for **educational purposes** and to assist authorized administrative staff.
* Do not use this tool to generate fraudulent identification.
* The developer (@muhibkhan123) is not responsible for misuse of this code.

---

*Star this repository if you found it useful! ⭐*
