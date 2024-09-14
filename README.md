# Clean-Mushaf

**Bismillah.** This project provides a high-resolution, vectorized, and minimalistic PDF of the Medina Mushaf, complete with an outline containing all English Surah names and numbers. This PDF is compiled from the SVG files available [here](https://github.com/batoulapps/quran-svg/tree/main). Download it to your phone to have a beautiful, annotatable copy of the Mushaf always available for reference. For iPhone users, I highly recommend using the `PDF Viewer` app, which is fast, ad-free, and offers a versatile free tier.

If you have suggestions or improvements for the PDF, please feel free to open an issue on GitHub!

## How to Use This Repository

### Option 1: Simply Download the Mushaf

**[Download Link (Google Drive)](https://drive.google.com/file/d/1WGePc8kzeT3_rq0kjE-nxAMu6DUL1S2O/view?usp=sharing)**

**Notes:**
- The file size is approximately 200 MB. The high resolution of the pages necessitates this size, and further compression would compromise quality.

### Option 2: Compile the Mushaf Yourself Using Python

This method is tested on Ubuntu.

**Steps:**

1. **Clone the SVG Repository:**
   Clone the repository containing the SVG files of each page of the Quran:
   ```
   git clone https://github.com/batoulapps/quran-svg
   ```
2. **Copy the SVG Files:**
   Copy the `svg` folder into this repository and rename it to `quran_svg`.

3. **Install Inkscape:**
   Inkscape provides a command-line tool to convert SVG files into PDFs. Install it using the following commands:
   ```bash
   sudo add-apt-repository universe
   sudo add-apt-repository ppa:inkscape.dev/stable
   sudo apt-get update
   sudo apt install inkscape
   ```

4. **Install PyPDF:**
   Install PyPDF to handle the merging of PDF pages and creating a table of contents:
   ```bash
   pip install pypdf
   ```

5. **Run the `svg_to_pdf.ipynb` Notebook:**
   This notebook will:
   - Convert each SVG page into a PDF.
   - Merge all the pages into a single document.
   - Write a table of contents with Surah names.

**If you find this project useful, please consider [*buying me a coffee*](https://ko-fi.com/haqihaq)!** 
