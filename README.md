# Isabelle Athena Qian — Personal Website & Portfolio

A clean, fast, mobile-friendly, accessible one-page personal website tailored for **Frontier Lab Policy and Safety Teams** (Anthropic, Google DeepMind, OpenAI, etc.).

---

## 📁 Files Included

* **`index.html`**: Semantic, accessible HTML5 structure with OpenGraph meta tags, smooth scrolling anchors, dark/light theme persistence, and WCAG compliance.
* **`style.css`**: Mobile-first responsive CSS stylesheet featuring an elegant academic/frontier lab aesthetic, dark/light mode CSS variables, and high-contrast typography.
* **`README.md`**: Step-by-step instructions for hosting on GitHub Pages for free.

---

## ⚡ How to Preview Locally

You can preview the site immediately on your Mac:

### Method 1: Double-Click
Simply double-click `index.html` in your Finder to open it in Chrome, Safari, or your default browser.

### Method 2: Python Local Server
Open Terminal, navigate to the folder, and run:
```bash
python3 -m http.server 8000
```
Then visit `http://localhost:8000` in your browser.

---

## 🚀 Step-by-Step: Host for Free on GitHub Pages

GitHub Pages gives you free, secure (HTTPS), zero-maintenance hosting directly from a GitHub repository.

### Step 1: Create a GitHub Repository
1. Log into your GitHub account at [github.com](https://github.com).
2. Click the **`+`** icon in the top-right corner and select **New repository**.
3. For your primary personal website URL, name the repository exactly:
   ```text
   <your-github-username>.github.io
   ```
   *(For example, if your GitHub handle is `isabelleqian`, name it `isabelleqian.github.io`).*
4. Set the visibility to **Public**.
5. Leave "Initialize with README" **unchecked** (we already have our files).
6. Click **Create repository**.

---

### Step 2: Upload Your Website Files

#### Method A: Using Git in Terminal (Recommended)
Open Terminal and run the following commands (replace `isabelleqian` with your actual GitHub username):

```bash
cd "personal-website"

# Initialize git repository
git init -b main

# Add all files (index.html, style.css, README.md, and your resume PDF)
git add .

# Commit files
git commit -m "Initial launch of AI governance & safety portfolio"

# Connect to your GitHub repository
git remote add origin https://github.com/isabelleqian/isabelleqian.github.io.git

# Push to GitHub
git push -u origin main
```

#### Method B: Using GitHub Web UI (No Terminal Needed)
1. In your newly created GitHub repository page, click the link that says **"uploading an existing file"**.
2. Drag and drop `index.html`, `style.css`, and your resume PDF file into the browser window.
3. Type a commit message (e.g., `Initial commit`) and click **Commit changes**.

---

### Step 3: Enable GitHub Pages & Verify Deployment

1. On your repository page on GitHub, click **Settings** (tab on the top right).
2. In the left sidebar, click **Pages** (under the "Code and automation" section).
3. Under **Build and deployment**:
   * **Source**: Select `Deploy from a branch`.
   * **Branch**: Select `main` (or `master`) and folder `/ (root)`.
   * Click **Save**.
4. GitHub Pages will take about 1 to 2 minutes to build. Refresh the page until you see a green box:
   > *"Your site is live at `https://<your-username>.github.io/`"*
5. Click the link to view your live portfolio!

---

### Step 4: Adding Your Resume PDF
In `index.html`, the resume button references:
```html
<a href="Isabelle_Qian_Resume.pdf" class="btn btn-primary" download="Isabelle_Qian_Resume.pdf">
```
To enable one-click resume downloads:
1. Export your master resume as a PDF named `Isabelle_Qian_Resume.pdf`.
2. Place `Isabelle_Qian_Resume.pdf` in the same directory alongside `index.html`.
3. Commit and push the file to your repository (`git add Isabelle_Qian_Resume.pdf && git commit -m "Add PDF resume" && git push`).

---

## 🎨 Customizing & Updating
* **Accent Colors & Theming**: All colors, fonts, and dark/light mode palettes are defined as clean CSS variables at the top of `style.css` (`:root` and `[data-theme="light"]`).
* **Paper Updates**: The arXiv link is set to `https://arxiv.org/html/2512.15584v2` and can be adjusted anytime in `index.html`.
