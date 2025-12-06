# UST Bannu ID Card Generator

A powerful, client-side web application designed to generate professional Student ID Cards for the **University of Science & Technology Bannu (USTB)**. This tool allows for real-time data entry, security pattern generation, and exporting to both **PNG** and **Layered PSD** formats.

![Project Status](https://img.shields.io/badge/Status-Active-success)
![Tech Stack](https://img.shields.io/badge/Built%20With-HTML5%20%7C%20Tailwind%20%7C%20JS-blue)

## 📸 Screenshots

![App Interface](https://via.placeholder.com/800x400?text=App+Interface+Screenshot)

## ✨ Features

* **Real-Time Preview:** Instantly see changes on the ID card as you type student details.
* **Dual-Side Generation:** Generates both Front and Back sides of the ID card simultaneously.
* **Security Pattern Randomizer:** Includes a built-in engine that generates random vector background patterns (Geometric, Waves, Grid, etc.) to simulate security watermarks.
* **Layered PSD Export:** Unlike most web generators that only save images, this tool uses `ag-psd` to export fully editable **Layered Photoshop (PSD)** files.
* **PNG Export:** High-quality PNG download using `html2canvas`.
* **Custom Assets:**
    * Upload Student Photos.
    * Upload Digital Signatures.
    * Upload Custom University Logos (Front and Back).
* **Barcode Generation:** Automatically converts the Student ID into a visual Barcode.
* **Responsive UI:** Built with Tailwind CSS for a clean, modern interface.

## 🛠️ Tech Stack

* **Core:** HTML5, JavaScript (ES6+).
* **Styling:** [Tailwind CSS](https://tailwindcss.com/) (via CDN).
* **Icons:** FontAwesome.
* **Fonts:** Google Fonts (Roboto Condensed & Libre Barcode 39).
* **Libraries:**
    * `html2canvas` - For capturing the DOM as a flat PNG image.
    * `ag-psd` - For constructing and writing layered PSD files directly in the browser.

## 🚀 How to Run

Since this is a client-side application using CDNs, no server setup is required.

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/ust-id-card-generator.git](https://github.com/your-username/ust-id-card-generator.git)
    ```
2.  **Open the file:**
    Navigate to the folder and open `index.html` in any modern web browser (Chrome, Edge, Firefox).
3.  **Internet Connection:**
    Ensure you are connected to the internet, as the application loads styles and libraries via CDN.

## 📖 Usage Guide

1.  **University Details:** Modify the university name or address if needed (defaults to UST Bannu).
2.  **Student Details:** Enter the Name, Father's Name, CNIC, and Session.
3.  **Photos & Logos:** Click the "Choose File" buttons to upload the student's photo and the Registrar's signature.
4.  **Pattern:** Click **"Pick Random Pattern"** to change the background security design.
5.  **Adjust Back Spacing:** Use the slider to adjust the text spacing on the back of the card if the content overlaps.
6.  **Download:**
    * Click **Download PNG** for a quick image file.
    * Click **Layered PSD** to edit text and layers later in Photoshop.

## 📂 Project Structure

```text
/
├── index.html       # The main application file containing HTML, CSS, and JS
├── README.md        # Project documentation
└── (assets)         # (Optional) If you decide to host images locally later
