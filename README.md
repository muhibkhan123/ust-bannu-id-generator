UST Bannu ID Card Generator

A powerful, web-based tool designed to generate professional Student ID Cards for the University of Science & Technology, Bannu (USTB). This application provides a real-time preview and allows users to export high-resolution cards in both PNG format for immediate printing and Layered PSD format for advanced editing in Adobe Photoshop.

🌟 Features

1. Real-Time Visualization

Instant Preview: See changes immediately on both the Front and Back cards as you type or upload images.

Responsive Design: The interface adapts to various screen sizes, making it usable on desktops, tablets, and mobile devices.

2. Deep Customization

University Details: Manually edit the University Name and Address header to suit different campuses or departments.

Student Information: Comprehensive fields for S/ID, Session, Discipline, Name, Father's Name, Contact No, CNIC, and Address.

Smart Barcode: Automatically generates a scannable Code 39 barcode based on the Student ID.

3. Visual & Security Elements

Security Patterns: Includes a "Pick Random Pattern" feature that applies intricate, vector-based security background textures (e.g., Waves, Geometric, Leaves, Micro-grid) to prevent counterfeiting.

Layout Control: A "Back Bottom Spacing" slider allows you to adjust the vertical alignment of the back card content to ensure it fits perfectly with pre-printed card stock or specific printer margins.

4. Media Support

Photo Upload: Supports standard image formats (JPG, PNG) for student photos, automatically fitting them into the designated frame.

Custom Logos: Upload distinct logos for the Front and Back of the card.

Digital Signature: Upload a digital signature image for the issuing authority on the back.

5. Advanced Export Options

Download PNG: Generates a high-resolution, flattened image (3x scale) optimized for direct printing on CR80 PVC cards.

Download Layered PSD: Uses the ag-psd library to generate a true Photoshop file. Every element (Text, Logo, Photo, Background) is placed on its own separate layer, allowing for post-production edits in Adobe Photoshop.

🚀 Getting Started

Prerequisites

A modern web browser (Google Chrome, Mozilla Firefox, Microsoft Edge, or Safari).

No internet connection is required to run the tool once downloaded (it works offline), but an internet connection is needed to load the initial external libraries (Tailwind, FontAwesome, etc.) unless you save them locally.

Installation

Clone the repository:

git clone [https://github.com/muhibkhan123/ust-bannu-id-generator.git](https://github.com/muhibkhan123/ust-bannu-id-generator.git)


Download ZIP: Alternatively, click the "Code" button and select "Download ZIP". Extract the files to a folder on your computer.

Running the App

Navigate to the project folder.

Double-click the idm.html file.

The application will open in your default web browser.

📖 Usage Guide

University Settings:

At the top of the form, verify or edit the University Name and Address. These changes reflect on both the front header and the back header.

Student Data Entry:

Fill in the Student Details form. The S/ID field automatically updates the barcode on the back card.

Uploading Assets:

Front Logo / Back Logo: Click "Choose File" to upload the university crest or department logo.

Student Photo: Upload a passport-sized photograph.

Signature: Upload a transparent PNG of the Registrar's signature for the back.

Styling:

Click "Pick Random Pattern" until you find a background security design you like.

Use the Slider to adjust the spacing on the back card if the text overlaps with the footer.

Exporting:

For Printing: Click the Download PNG button for the respective side.

For Editing: Click the Layered PSD button to get a file compatible with Photoshop.

🛠️ Technical Stack

Core: HTML5, CSS3, Vanilla JavaScript.

Styling Framework: Tailwind CSS (via CDN) for utility-first styling.

Typography: Google Fonts ('Roboto Condensed' for text, 'Libre Barcode 39 Text' for barcodes).

Icons: FontAwesome 6.

Libraries:

html2canvas: Captures the DOM element and renders it as a canvas for PNG export.

ag-psd: A pure JavaScript library used to construct binary PSD files with layers, text, and images directly in the browser.

⚠️ Troubleshooting

Images not appearing in download: Ensure you are using local image files. If you are developing and using online placeholder images, browser security policies (CORS) might block the download.

Barcode not scanning: Ensure the Student ID is numeric. The tool automatically adds the required start/stop characters (*) for Code 39 barcodes.

Layout looks wrong on mobile: While the tool is responsive, it is best used on a Desktop or Tablet screen to accurately visualize the physical card dimensions.

📂 Project Structure

/
├── idm.html       # The complete application (HTML structure, CSS styles, JS logic)
└── README.md      # Detailed documentation


🤝 Contributing

Contributions are welcome! If you have ideas for new features (like QR code support or bulk generation), feel free to fork the repository and submit a pull request.

Fork the Project

Create your Feature Branch (git checkout -b feature/AmazingFeature)

Commit your Changes (git commit -m 'Add some AmazingFeature')

Push to the Branch (git push origin feature/AmazingFeature)

Open a Pull Request

📄 License

This project is open-source and available for educational and personal use.
