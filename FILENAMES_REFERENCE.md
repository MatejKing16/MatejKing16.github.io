# Filenames & Text Reference

## 🔴 CRITICAL: Replace These Text Placeholders in index.html

Find & replace in the code (case-sensitive):

```
YOUR-USERNAME  
→ Replace with: your actual GitHub username (e.g., matejkral1603)
   Appears in TWO places:
   - Hero section GitHub button
   - Contact section GitHub card
```

```
YOUR-GITHUB-USERNAME.github.io
→ Replace with: your GitHub Pages URL (e.g., matejkral1603.github.io)
   Appears in: meta tag <og:url>
```

Also update in projects-template.html:
```
YOUR-USERNAME
→ Replace with: your actual GitHub username (in footer link)
```

---

## 📷 Gallery Photos for Main Portfolio

These go in the **root folder** (same level as index.html):

| Section | Filenames | How Many |
|---------|-----------|----------|
| Hero portrait | `photo.jpg` | 1 |
| Featured EOAT | `eoat-assembly.jpg`, `solidworks-model.jpg`, `technical-drawing.jpg`, `robot-cell.jpg` | 4 |
| CzechSkills | `czechskills-podium.jpg`, `czechskills-programming.jpg`, `czechskills-diploma-photo.jpg` | 3 |
| CNC Milling | `machine-overview.jpg`, `cnc-in-action.jpg`, `solidworks-cad.jpg` | 3 |
| AI CNC Operator | `web-interface.jpg`, `cncjs-screenshot.jpg`, `wiring.jpg` | 3 |
| Squat Rack | `rack-render.jpg`, `solidworks-drawing.jpg`, `fabricated.jpg` | 3 |
| ATG Internship | `fanuc-robot.jpg`, `eoat-adapter.jpg`, `bin-picking.jpg` | 3 |
| Reverse Engineering | `cmm-measurement.jpg`, `solidworks-reconstruction.jpg`, `iso-drawing.jpg` | 3 |

**Format**: JPG or PNG, named exactly as above (case-sensitive!)

---

## 📹 Video Files for Main Portfolio

| Project | Filename | Format | Where |
|---------|----------|--------|-------|
| AI CNC Operator | `cnc-ai-demo.mp4` | MP4 video | root folder |

---

## 📄 PDF Files for Main Portfolio

These go in the **root folder**:

| Document | Filename | Size Estimate |
|----------|----------|----------------|
| CV | `cv.pdf` | ~0.5 MB |
| Thesis | `thesis.pdf` | ~8 MB |
| CzechSkills Diploma | `czechskills-diploma.pdf` | ~2 MB |
| CSWP Certificate | `cswp-certificate.pdf` | ~1 MB |
| Cambridge Certificate | `cambridge-certificate.pdf` | ~1 MB |
| Thesis Drawings | `thesis-drawings.pdf` | ~5 MB |

---

## 📂 Project Detail Pages (Optional)

If you want to create project detail pages, folder structure is:

```
projects/
├── eoat-tooling/
│   ├── index.html              (copy from projects-template.html)
│   ├── photo-1.jpg             (any names, just match HTML)
│   ├── photo-2.jpg
│   └── photo-3.jpg
│
├── cnc-ai-operator/
│   ├── index.html
│   ├── photo-1.jpg
│   └── demo.mp4
│
├── cnc-milling/
│   ├── index.html
│   └── photos...
│
└── (more projects...)
```

**Inside each project folder:**
- Name photos however you want
- Just make sure the HTML references the correct names
- Example in HTML: `<img src="photo-1.jpg" alt="...">`

---

## ✅ Checklist: What You Have

- ✅ `index.html` — main portfolio (updated)
- ✅ `projects-template.html` — copy for each project page
- ✅ `PROJECT_PAGES_SETUP.md` — detailed folder instructions
- ✅ `WHAT_WAS_ADDED.md` — summary of changes
- ✅ `FILENAMES_REFERENCE.md` — this file

---

## 🚀 Quick Start

1. Download the files above
2. Replace `YOUR-USERNAME` in `index.html` (2 places)
3. Replace `YOUR-GITHUB-USERNAME.github.io` (1 place)
4. Add gallery photos using filenames above
5. Push to GitHub
6. Done! (optional: create project pages later)

---

## 🆘 If Something Doesn't Show

**Photos not showing?**
- Check filename matches exactly (case-sensitive: `photo.jpg` ≠ `Photo.JPG`)
- Make sure it's in the root folder
- Wait a few minutes for GitHub to update

**Links broken (404)?**
- Project links: Make sure `projects/` folder exists with correct subfolders
- GitHub link: Did you replace `YOUR-USERNAME`?
- Check folder names have no spaces and are lowercase

**Video not playing?**
- Only MP4 format works
- Make sure `cnc-ai-demo.mp4` is in root folder
- File size shouldn't exceed 100 MB

---

## 💡 Pro Tips

- Use `.jpg` for photos (smaller file size)
- Use `.png` for screenshots (better quality for text)
- Use `.mp4` for videos (widely supported)
- All filenames: lowercase, no spaces, use hyphens instead (`my-photo.jpg` ✓, `MyPhoto.jpg` ✗)
- GitHub is case-sensitive on file names (unlike Windows)

---

## Done?

Once everything is pushed:
1. Visit `https://YOUR-USERNAME.github.io`
2. Test all links
3. Share on LinkedIn
4. Start networking!

Good luck! 🚀
