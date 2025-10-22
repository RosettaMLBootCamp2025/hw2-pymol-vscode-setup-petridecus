[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/026OgCAU)
# HW2: PyMOL and VS Code Setup

## Overview

This assignment ensures you have PyMOL and VS Code installed and configured for the bootcamp. You will:

1. Install PyMOL (a molecular visualization tool)
2. Install VS Code (a powerful code editor/IDE)
3. Verify your installations by completing hands-on tasks
4. Commit your work to GitHub

## Prerequisites

- HW1 completed

## Part 1: PyMOL Installation

PyMOL is a molecular visualization tool that is super useful for visualizing, manipulating, and analyzing molecular structures, especially proteins. We will use PyMOL to explore protein structures during bootcamp. We recognize that it's likely you are already quite familiar with PyMOL but if you have been using an alternative visualization software, this is a great opportunity to explore PyMOL. Please be ready to use this in the Bootcamp.

### Installation Options

**Option 1: Official PyMOL (Requires Educational License)**
1. Visit the PyMOL website: https://pymol.org/
2. Obtain a free educational license: https://pymol.org/edu/
3. Download and install PyMOL

**Option 2: Open-Source PyMOL via Homebrew (Mac users)**
If you have Homebrew installed:
```bash
brew install pymol
```

Verify installation by launching PyMOL (GUI) from your applications or by running:
```bash
pymol
```

### Optional PyMOL Learning Resources

Though a comprehensive understanding of the various features in PyMOL is not within the scope of this course, it may be a useful tool for your future work and presentations.

- [PyMOL Tutorial Video](https://www.youtube.com/watch?v=h5wKppcyzOw) - Complete this tutorial using a protein of interest
- [PyMOL Guide](https://docs.google.com/document/d/1ocdlrfUPerFWDb_QSMvAfxt_RVG4ArQkUeGh6q4Leys/edit#heading=h.4pohw9oi2g04) - Comprehensive written guide
- [PyMOL Wiki](https://pymolwiki.org/index.php/Main_Page) - Explore more PyMOL features and tools

### Customizing PyMOL (Optional)

If you would like to alter your visual defaults, you may do so by editing your `.pymolrc`, which is a script that gets read every time PyMOL opens. To do so, go to File > Edit pymolrc. [Here are the defaults that Rosetta member Joey Lubin uses](https://drive.google.com/file/d/1W5h-jVch1KVdripRdiu856kICsZRjO-0/view?usp=sharing), which can be pasted into the window that opens.

## Part 2: VS Code Installation

VS Code is a powerful IDE that is largely customizable and can incorporate many different extensions and features. If you do not have VS Code or an alternative IDE, please install it before the bootcamp.

### Installation Options

**Option 1: Download from Website**
Visit the VS Code website: https://code.visualstudio.com/

**Option 2: Install via Homebrew (Mac users)**
If you have Homebrew installed:
```bash
brew install --cask visual-studio-code
```

Verify installation by launching VS Code or running:
```bash
code --version
```

### Recommended VS Code Extensions

Once VS Code is installed, we recommend installing the following extensions:

1. **Python** (Microsoft) - Python language support
2. **Pylance** (Microsoft) - Fast Python language server
3. **Jupyter** (Microsoft) - Jupyter notebook support

To install extensions:
1. Open VS Code
2. Click the Extensions icon in the sidebar (or press Cmd+Shift+X / Ctrl+Shift+X)
3. Search for each extension and click "Install"

## Part 3: Verification Tasks

Now let's verify that everything is working correctly!

### Task 1: PyMOL Verification

1. **Fetch a protein structure:**
   - Open PyMOL
   - In the PyMOL command line, type: `fetch 1ubq`
   - This fetches ubiquitin (PDB ID: 1UBQ), a small regulatory protein

2. **Style your visualization:**
   - Try different representations (cartoon, sticks, surface, etc.)
   - Color the structure in a way you find visually appealing
   - Feel free to experiment!

3. **Save your work:**
   - Save the PyMOL session: `File > Save Session As...`
   - Name it `1ubq_session.pse` and save it in this assignment directory
   - Export an image: `File > Export Image As > PNG...`
   - Name it `1ubq_visualization.png` and save it in this assignment directory

### Task 2: VS Code Verification

1. **Open VS Code**

2. **Create a Python script:**
   - Open this assignment folder in VS Code: `File > Open Folder...`
   - Create a new file called `verify_setup.py`
   - Copy and paste the verification script (provided in this repository)
   - Run the script to verify your setup

3. **Run the verification script:**
   - Open the integrated terminal in VS Code: `Terminal > New Terminal`
   - Activate your conda environment from HW1: `conda activate bootcamp2025_HW1`
   - Run: `python verify_setup.py`
   - The script will check your installations and create a `verification_result.txt` file

## Part 4: Submission

Once you've completed both tasks, commit your work to your GitHub Classroom repository:

```bash
# Add all the files you created
git add 1ubq_session.pse 1ubq_visualization.png verification_result.txt

# Commit your work
git commit -m "Complete PyMOL and VS Code setup verification"

# Push to GitHub
git push
```

### Required Files for Submission

Make sure your repository contains:
- [ ] `1ubq_session.pse` - Your PyMOL session file
- [ ] `1ubq_visualization.png` - Your exported PyMOL visualization
- [ ] `verification_result.txt` - Output from the VS Code verification script

## Troubleshooting

### PyMOL Issues

**PyMOL won't launch:**
- Make sure you've completed the installation fully
- Mac users: Try the Homebrew installation method
- Make sure you're launching the GUI application, not just the Python package

**Can't fetch PDB structures:**
- Check your internet connection
- Try: `fetch 1ubq, type=pdb1` if the default doesn't work

### VS Code Issues

**`code` command not found:**
- On Mac: Open VS Code, press Cmd+Shift+P, type "shell command", and select "Install 'code' command in PATH"
- On Windows: VS Code should be in your PATH automatically after installation

**Python extension not working:**
- Make sure Python is installed (you should have this from HW1)
- Restart VS Code after installing extensions

## Questions?

If you run into any issues or have questions, contact Ian at: **icanderson@ucdavis.edu**
