# 📚 Study Notes Hub

A beautiful, organized collection of study notes with collapsible subjects and chapter navigation. Perfect for students who want quick access to their notes from anywhere!

## ✨ Features

- **📁 Organized by Subject** - Each subject has its own section
- **📖 Chapter Navigation** - Break down subjects into individual chapters
- **🔍 Smart Search** - Search across subjects and chapters instantly
- **📱 Mobile Friendly** - Perfect on phones, tablets, and computers
- **🖨️ Print Ready** - Optimized for printing
- **⚡ Fast & Simple** - No frameworks, just pure HTML/CSS/JS
- **🎯 Collapsible Sections** - Click headers to expand/collapse subjects

## 📁 Folder Structure

```
study-notes/
│
├── index.html                          # Main page with all subjects
│
├── notes/                              # All note files go here
│   ├── government-accounting.html      # Example complete note
│   ├── physics-chapter1.html           # Example chapter note
│   ├── physics-chapter2.html
│   ├── chemistry-chapter1.html
│   └── ...                             # Add more here
│
├── assets/                             # Optional: images, PDFs
│   ├── images/
│   └── pdfs/
│
└── README.md                           # This file
```

## 🚀 Quick Start

### 1. Create GitHub Repository

1. Go to [GitHub](https://github.com) and login/signup
2. Click **+** → **New repository**
3. Name it: `study-notes`
4. Make it **Public**
5. ✅ Check "Add a README file"
6. Click **Create repository**

### 2. Upload Files

**Option A: GitHub Web Interface (Easiest)**

1. Click **Add file** → **Create new file**
2. Name it: `index.html`
3. Copy and paste the index.html content
4. Click **Commit new file**
5. Repeat for creating `notes/` folder:
   - Create file: `notes/government-accounting.html`
   - Paste content and commit

**Option B: Git Command Line**

```bash
# Clone your repo
git clone https://github.com/yourusername/study-notes.git
cd study-notes

# Create folders
mkdir notes assets

# Add your files (copy index.html and notes here)

# Commit and push
git add .
git commit -m "Added study notes with chapter navigation"
git push origin main
```

### 3. Enable GitHub Pages

1. Go to repository **Settings**
2. Click **Pages** (left sidebar)
3. Under **Source**: Select **main** branch and **/ (root)** folder
4. Click **Save**
5. Wait 1-2 minutes ⏳

### 4. Access Your Website

Your site will be live at:
```
https://yourusername.github.io/study-notes/
```
Replace `yourusername` with your GitHub username.

## 📝 How to Add Content

### Adding a Complete Subject (Single Page)

If your subject has all content in one page (like Government Accounting):

```html
<div class="subject-section">
    <div class="subject-header" onclick="toggleSection(this)">
        <span class="subject-icon">🏛️</span>
        <div class="subject-title">
            <h2>Subject Name</h2>
            <p>Subject description</p>
        </div>
        <span class="toggle-icon">▼</span>
    </div>
    
    <div class="chapters-grid">
        <a href="notes/subject-complete.html" class="chapter-card">
            <div class="chapter-number">COMPLETE NOTES</div>
            <h3>Full Course Material</h3>
            <p>All topics in one document.</p>
        </a>
    </div>
</div>
```

### Adding a Subject with Multiple Chapters

For subjects broken into chapters (like Physics):

```html
<div class="subject-section">
    <div class="subject-header" onclick="toggleSection(this)">
        <span class="subject-icon">⚛️</span>
        <div class="subject-title">
            <h2>Physics</h2>
            <p>Classical and modern physics</p>
        </div>
        <span class="toggle-icon">▼</span>
    </div>
    
    <div class="chapters-grid">
        
        <a href="notes/physics-chapter1.html" class="chapter-card">
            <div class="chapter-number">CHAPTER 1</div>
            <h3>Motion and Kinematics</h3>
            <p>Velocity, acceleration, equations of motion.</p>
        </a>
        
        <a href="notes/physics-chapter2.html" class="chapter-card">
            <div class="chapter-number">CHAPTER 2</div>
            <h3>Newton's Laws</h3>
            <p>Forces, momentum, and laws of motion.</p>
        </a>
        
        <a href="notes/physics-chapter3.html" class="chapter-card">
            <div class="chapter-number">CHAPTER 3</div>
            <h3>Work, Energy & Power</h3>
            <p>Energy conservation and power calculations.</p>
        </a>
        
    </div>
</div>
```

### 📝 Quick Add Template

Copy this entire block to add a new subject:

```html
<div class="subject-section">
    <div class="subject-header" onclick="toggleSection(this)">
        <span class="subject-icon">📖</span>
        <div class="subject-title">
            <h2>Subject Name</h2>
            <p>Brief description</p>
        </div>
        <span class="toggle-icon">▼</span>
    </div>
    
    <div class="chapters-grid">
        
        <a href="notes/subject-chapter1.html" class="chapter-card">
            <div class="chapter-number">CHAPTER 1</div>
            <h3>Chapter Title</h3>
            <p>Chapter description.</p>
        </a>
        
        <a href="notes/subject-chapter2.html" class="chapter-card">
            <div class="chapter-number">CHAPTER 2</div>
            <h3>Chapter Title</h3>
            <p>Chapter description.</p>
        </a>
        
    </div>
</div>
```

## 🎨 Customization

### Subject Icons

Choose from these emojis or use your own:

| Subject | Icon |
|---------|------|
| Physics | ⚛️ |
| Chemistry | 🧪 |
| Mathematics | 📐 |
| Biology | 🧬 |
| Computer Science | 💻 |
| History | 🏛️ |
| Geography | 🌍 |
| Literature | 📖 |
| Business | 💼 |
| Economics | 📈 |
| Law | ⚖️ |
| Medicine | ⚕️ |
| Engineering | ⚙️ |
| Arts | 🎨 |

### Change Colors

Edit the CSS in `index.html`:

```css
/* Main colors */
background: linear-gradient(135deg, #F5F1E8, #E8DCC4);  /* Page background */
background: linear-gradient(135deg, #7B92A8, #8B9D83);  /* Header */
border-left: 5px solid #D4917B;                         /* Card accent */
```

### File Naming Convention

Keep it organized and consistent:

**Format:** `subject-chapterX.html` or `subject-topic.html`

**Examples:**
```
physics-chapter1.html
physics-chapter2.html
chemistry-chapter1.html
chemistry-chapter2.html
math-algebra.html
math-calculus.html
biology-cell-structure.html
history-world-war2.html
```

## 🔍 Search Function

The search works on:
- ✅ Subject names
- ✅ Subject descriptions
- ✅ Chapter numbers
- ✅ Chapter titles
- ✅ Chapter descriptions

**Examples:**
- Search "chapter 1" → Shows all Chapter 1s
- Search "physics" → Shows Physics subject and all its chapters
- Search "motion" → Shows chapters with "motion" in title/description

## 📱 Mobile Usage

### Add to Home Screen

**iPhone/iPad:**
1. Open your site in Safari
2. Tap the Share button
3. Tap "Add to Home Screen"
4. Name it and tap "Add"

**Android:**
1. Open your site in Chrome
2. Tap the menu (⋮)
3. Tap "Add to Home Screen"
4. Name it and tap "Add"

Now you have an app icon to access your notes instantly!

## 🖨️ Printing Notes

1. Open any note page
2. Press `Ctrl + P` (Windows) or `Cmd + P` (Mac)
3. Choose your printer or "Save as PDF"
4. Print!

All pages are optimized for printing with:
- Clean backgrounds
- Readable fonts
- Proper page breaks

## 🎯 Real-World Examples

### Example 1: Chemistry Course

```html
<div class="subject-section">
    <div class="subject-header" onclick="toggleSection(this)">
        <span class="subject-icon">🧪</span>
        <div class="subject-title">
            <h2>Chemistry</h2>
            <p>Organic, inorganic, and physical chemistry</p>
        </div>
        <span class="toggle-icon">▼</span>
    </div>
    
    <div class="chapters-grid">
        
        <a href="notes/chemistry-chapter1.html" class="chapter-card">
            <div class="chapter-number">CHAPTER 1</div>
            <h3>Atomic Structure</h3>
            <p>Atoms, electrons, protons, neutrons, and the periodic table.</p>
        </a>
        
        <a href="notes/chemistry-chapter2.html" class="chapter-card">
            <div class="chapter-number">CHAPTER 2</div>
            <h3>Chemical Bonding</h3>
            <p>Ionic, covalent, and metallic bonds explained.</p>
        </a>
        
        <a href="notes/chemistry-chapter3.html" class="chapter-card">
            <div class="chapter-number">CHAPTER 3</div>
            <h3>Stoichiometry</h3>
            <p>Moles, molecular mass, and balanced equations.</p>
        </a>
        
        <a href="notes/chemistry-chapter4.html" class="chapter-card">
            <div class="chapter-number">CHAPTER 4</div>
            <h3>Thermodynamics</h3>
            <p>Enthalpy, entropy, and Gibbs free energy.</p>
        </a>
        
    </div>
</div>
```

### Example 2: Computer Science Course

```html
<div class="subject-section">
    <div class="subject-header" onclick="toggleSection(this)">
        <span class="subject-icon">💻</span>
        <div class="subject-title">
            <h2>Computer Science</h2>
            <p>Programming, algorithms, and data structures</p>
        </div>
        <span class="toggle-icon">▼</span>
    </div>
    
    <div class="chapters-grid">
        
        <a href="notes/cs-python-basics.html" class="chapter-card">
            <div class="chapter-number">MODULE 1</div>
            <h3>Python Basics</h3>
            <p>Variables, data types, and control structures.</p>
        </a>
        
        <a href="notes/cs-data-structures.html" class="chapter-card">
            <div class="chapter-number">MODULE 2</div>
            <h3>Data Structures</h3>
            <p>Arrays, linked lists, stacks, and queues.</p>
        </a>
        
        <a href="notes/cs-algorithms.html" class="chapter-card">
            <div class="chapter-number">MODULE 3</div>
            <h3>Algorithms</h3>
            <p>Sorting, searching, and algorithm complexity.</p>
        </a>
        
    </div>
</div>
```

## 🔧 Troubleshooting

### Notes not loading

**Problem:** Clicking a chapter shows "404 Not Found"

**Solution:**
- Check file name spelling (case-sensitive!)
- Verify file is in `notes/` folder
- Make sure path is correct: `notes/filename.html`

### Search not working

**Problem:** Search doesn't show results

**Solution:**
- Make sure JavaScript is enabled in browser
- Check browser console for errors (F12)
- Clear browser cache and refresh

### Changes not appearing

**Problem:** Updated files but changes don't show

**Solution:**
- Wait 1-5 minutes for GitHub to rebuild
- Hard refresh: `Ctrl + Shift + R` (Windows) or `Cmd + Shift + R` (Mac)
- Check GitHub Actions tab for build errors

### Sections won't collapse

**Problem:** Clicking subject headers doesn't work

**Solution:**
- Ensure `onclick="toggleSection(this)"` is present in subject-header div
- Check JavaScript is not blocked
- Verify you copied the complete code

## 📊 Features Breakdown

| Feature | Description |
|---------|-------------|
| **Collapsible Subjects** | Click any subject header to expand/collapse chapters |
| **Smart Search** | Real-time search across all content |
| **Auto-Expand** | Matching sections auto-expand when searching |
| **Responsive Grid** | Adapts to screen size (mobile, tablet, desktop) |
| **Print Optimized** | Clean printing without unnecessary elements |
| **Fast Loading** | No external dependencies, pure HTML/CSS/JS |
| **Easy Updates** | Simple HTML structure, no build process needed |

## 💡 Pro Tips

1. **Keep names consistent:** Use lowercase with hyphens (e.g., `physics-chapter1.html`)
2. **Organize by subject:** Group related files with same prefix
3. **Use descriptive titles:** Help search function work better
4. **Test locally first:** Open index.html in browser before uploading
5. **Commit regularly:** Save your work often on GitHub
6. **Use meaningful commits:** Write clear commit messages

## 🎓 Study Tips

- ✅ Add notes immediately after class while fresh
- ✅ Use search to quickly review specific topics
- ✅ Print important chapters for offline study
- ✅ Share link with study group
- ✅ Update regularly with new insights
- ✅ Create cross-references between related chapters

## 📞 Support

### Need Help?

- **GitHub Issues:** Report bugs or ask questions
- **Email:** your-email@example.com (optional)

### Useful Links

- [GitHub Pages Documentation](https://docs.github.com/pages)
- [Markdown Guide](https://www.markdownguide.org/)
- [HTML Reference](https://developer.mozilla.org/en-US/docs/Web/HTML)

## 📄 License

Free to use for educational purposes. Modify and share as needed!

## 🗺️ Roadmap

- [ ] Add more subjects and chapters
- [ ] Include practice questions
- [ ] Add bookmark functionality
- [ ] Create dark mode toggle
- [ ] Add download PDF option
- [ ] Include flashcards feature

## 🌟 Showcase

Share your study notes hub! If you create something cool with this template, let me know!

---

**⭐ Star this repo if you find it helpful!**

**Made with 📚 for students everywhere**

*Last updated: November 2025*
