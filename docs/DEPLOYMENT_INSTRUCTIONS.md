# Skeletal System Educational Resource - Deployment Instructions

## Package Contents

This package contains:
- **skeletal_system_guide.md** - Complete educational guide in Markdown format
- **images/** - 26 high-quality educational illustrations
- **DEPLOYMENT_INSTRUCTIONS.md** - This file

---

## Option 1: View as Markdown (Simplest)

### Using VS Code (Recommended)
1. Install [Visual Studio Code](https://code.visualstudio.com/)
2. Extract this zip file to a folder on your computer
3. Open VS Code
4. Go to **File → Open Folder** and select the extracted folder
5. Click on `skeletal_system_guide.md` in the sidebar
6. Press `Ctrl+Shift+V` (Windows/Linux) or `Cmd+Shift+V` (Mac) to open the Markdown preview
7. All images will display inline with the content

### Using Obsidian (Great for Students)
1. Download [Obsidian](https://obsidian.md/) (free)
2. Extract this zip file to a folder
3. Open Obsidian and create a new vault pointing to the extracted folder
4. Open `skeletal_system_guide.md`
5. Click the "Reading view" button (book icon) to see formatted content with images

### Using Typora
1. Download [Typora](https://typora.io/) (paid, but excellent)
2. Extract the zip file
3. Open `skeletal_system_guide.md` with Typora
4. All content will display beautifully formatted

---

## Option 2: Convert to PDF

### Using Pandoc (Free)
1. Install [Pandoc](https://pandoc.org/installing.html)
2. Extract the zip file to a folder (e.g., `skeletal-system`)
3. Open Terminal/Command Prompt
4. Navigate to the folder:
   ```bash
   cd path/to/skeletal-system
   ```
5. Run:
   ```bash
   pandoc skeletal_system_guide.md -o skeletal_system_guide.pdf --pdf-engine=xelatex
   ```
6. Open the generated PDF file

### Using VS Code + Markdown PDF Extension
1. Install VS Code and the "Markdown PDF" extension
2. Open `skeletal_system_guide.md` in VS Code
3. Press `Ctrl+Shift+P` (Windows/Linux) or `Cmd+Shift+P` (Mac)
4. Type "Markdown PDF: Export (pdf)" and press Enter
5. The PDF will be created in the same folder

---

## Option 3: Create a Simple Website

### Using Python (Built-in on Mac/Linux)

1. Extract the zip file to a folder
2. Create a simple HTML file in the same folder called `index.html`:

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Human Skeletal System Guide</title>
    <script src="https://cdn.jsdelivr.net/npm/marked/marked.min.js"></script>
    <style>
        body {
            max-width: 900px;
            margin: 0 auto;
            padding: 20px;
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Arial, sans-serif;
            line-height: 1.6;
            color: #333;
        }
        img {
            max-width: 100%;
            height: auto;
            border-radius: 8px;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
            margin: 20px 0;
        }
        h1, h2, h3 {
            color: #2c3e50;
            margin-top: 30px;
        }
        h1 {
            border-bottom: 3px solid #3498db;
            padding-bottom: 10px;
        }
        h2 {
            border-bottom: 2px solid #95a5a6;
            padding-bottom: 8px;
        }
        table {
            border-collapse: collapse;
            width: 100%;
            margin: 20px 0;
        }
        th, td {
            border: 1px solid #ddd;
            padding: 12px;
            text-align: left;
        }
        th {
            background-color: #3498db;
            color: white;
        }
        tr:nth-child(even) {
            background-color: #f2f2f2;
        }
        code {
            background-color: #f4f4f4;
            padding: 2px 6px;
            border-radius: 3px;
        }
        blockquote {
            border-left: 4px solid #3498db;
            margin: 20px 0;
            padding-left: 20px;
            color: #555;
        }
    </style>
</head>
<body>
    <div id="content"></div>
    <script>
        fetch('skeletal_system_guide.md')
            .then(response => response.text())
            .then(text => {
                document.getElementById('content').innerHTML = marked.parse(text);
            });
    </script>
</body>
</html>
```

3. Open Terminal/Command Prompt in the folder
4. Run a simple web server:
   
   **On Mac/Linux:**
   ```bash
   python3 -m http.server 8000
   ```
   
   **On Windows:**
   ```bash
   python -m http.server 8000
   ```

5. Open your web browser and go to: `http://localhost:8000`
6. Click on `index.html`

---

## Option 4: Host Online (Free)

### Using GitHub Pages
1. Create a free [GitHub](https://github.com) account
2. Create a new repository called `skeletal-system-guide`
3. Upload all files from this package
4. Go to **Settings → Pages**
5. Select **main** branch and click **Save**
6. Your site will be live at: `https://yourusername.github.io/skeletal-system-guide/`

### Using Netlify Drop
1. Go to [Netlify Drop](https://app.netlify.com/drop)
2. Drag and drop the entire extracted folder
3. Your site will be live instantly with a free URL

---

## Tips for Students

- **Print the guide:** Export to PDF and print for offline study
- **Interactive learning:** Use the HTML version to click through topics
- **Flashcards:** Screenshot individual bone diagrams for study cards
- **Presentations:** Use images in PowerPoint or Google Slides
- **Quizzes:** Cover labels on diagrams and test yourself

---

## Technical Support

If you encounter any issues:
1. Make sure all files are in the same folder
2. Image paths in the Markdown file are relative (e.g., `images/bone.png`)
3. For web viewing, you need a local server (not just opening the HTML file)
4. Most Markdown viewers will display images automatically

---

## System Requirements

- **Minimum:** Any computer with a web browser or Markdown viewer
- **Recommended:** 
  - Modern web browser (Chrome, Firefox, Safari, Edge)
  - 100 MB free disk space
  - Screen resolution: 1280x720 or higher for best viewing

---

Enjoy learning about the human skeletal system! 🦴

