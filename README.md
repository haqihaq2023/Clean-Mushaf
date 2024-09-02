# Clean-Mushaf

Bismillah. This is a high-resolution (vectorised) and minimalistic PDF of the Medina mushaf, with an outline containing all english surah names and numbers. It is a compiled version of the SVG files [here](https://github.com/batoulapps/quran-svg/tree/main). Put it on your phone, so you can always have available a copy of the mushaf that you can annotate and refer to. If you are using iPhone, I highly recommend the `PDF Viewer` application, which is fast and has a ad-free and versatile free tier.

Please open a github issue if you can think of any improvements to the PDF!

## How to Use this Repository
#### Option 1: Simply download the mushaf

Download Link [(Google Drive)](https://drive.google.com/file/d/15eOohukjSJD95aqnxm9RgbeqeNRvYsgw/view?usp=sharing)

**Notes**
- The file size is almost 200 Mb; I could not find a way to further reduce the size while keeping the high resolution.

#### Option 2: Compile the mushaf yourself using Python
This is tested for Ubuntu.

Step 1: Clone [this](https://github.com/batoulapps/quran-svg/tree/main) repository, which contains SVG files of each individual page of the Quran.
Step 2: Copy the *svg* folder into this repository, renaming it as *quran_svg*.
Step 3: Install inkscape, which gives you a command-line tool to convert from svg to pdf's.
```
sudo add-apt-repository universe
sudo add-apt-repository ppa:inkscape.dev/stable
sudo apt-get update
sudo apt install inkscape
```

Step 4: Install pypdf
```
pip install pypdf
```

Step 5: Walk through `svg_to_pdf.ipynb`, which 
1. Converts each svg page into a pdf
2. Merges all of the pages together 
3. Writes a table of contents with the surah names
