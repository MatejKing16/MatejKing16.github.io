# Project Pages Setup Guide

## Folder Structure

Your GitHub repo should look like this:

```
your-repo/
│
├── index.html                    (main portfolio — already done)
├── photo.jpg                     (hero photo)
├── cv.pdf                        (CV file)
├── 
├── projects/                     (new folder — create this)
│   ├── eoat-tooling/            (one folder per project)
│   │   ├── index.html           (project detail page)
│   │   ├── photo-1.jpg          (photos specific to this project)
│   │   ├── photo-2.jpg
│   │   └── photo-3.jpg
│   │
│   ├── cnc-ai-operator/
│   │   ├── index.html
│   │   ├── demo-video.mp4
│   │   ├── photo-1.jpg
│   │   └── photo-2.jpg
│   │
│   ├── cnc-milling/
│   │   ├── index.html
│   │   ├── photo-1.jpg
│   │   └── photo-2.jpg
│   │
│   └── (more projects...)
│
├── eoat-assembly.jpg            (photos for main gallery stay here)
├── solidworks-model.jpg
├── technical-drawing.jpg
├── robot-cell.jpg
├── czechskills-podium.jpg
├── (all other gallery photos...)
│
└── README.md                     (optional, but good for GitHub)
```

**Key point**: Gallery photos for the main `index.html` stay in the root folder. Each project gets its own folder under `projects/` with its own photos.

---

## Step-by-Step Setup

### 1. Create the projects folder

In your GitHub repo, create a new folder called `projects` at the root level (same level as `index.html`).

### 2. For each project, create a subfolder

Example: `projects/eoat-tooling/`

### 3. Copy the template

Copy the file `projects-template.html` (I provided) into each project folder and rename it to `index.html`.

### 4. Edit the project page

Open the `index.html` in the project folder and find these placeholders:

```html
<h1>PROJECT_TITLE</h1>
```

Replace all of these:
- `PROJECT_TITLE` → your actual project name (e.g., "End-of-Arm Tooling for Bag-in-Box Palletization")
- `PROJECT_DATE` → when you built it (e.g., "March 2026")
- `PROJECT_ROLE` → what you did (e.g., "Design & Engineering")
- `PROJECT_SHORT_DESC` → 1-2 sentence description
- In the Overview section: write 2-3 sentences about what the project was
- In Technical Details: explain your design decisions
- In Specifications: add the actual specs (timeline, status, whatever is relevant)
- Replace the image filenames with your actual photos: `img-1.jpg`, `img-2.jpg`, etc.
- Replace skill tags with the actual skills you used

### 5. Add your photos

Drop the photos into the project folder. Name them whatever you want, just make sure the filenames in the HTML match.

### 6. Update main index.html

The main portfolio already has a link ready:
```html
<a class="project-link" href="./projects/cnc-ai-operator/index.html">View project →</a>
```

This link will automatically work once you create `projects/cnc-ai-operator/index.html`.

---

## Which Projects Need Pages?

You already have projects mentioned in the main page. Here are the project folders to create:

1. **eoat-tooling** → End-of-Arm Tooling (featured project)
2. **cnc-ai-operator** → AI CNC Operator (already has a "View project" link)
3. **cnc-milling** → DIY CNC Milling Machine
4. **squat-rack** → Structural Steel Squat Rack
5. **atg-internship** → ATG Internship / FANUC Robotics
6. **reverse-eng** → Reverse Engineering (aircraft exhaust pipe)

The CNC milling and squat rack project cards currently don't have "View project" links — you can either:
- Add links once you create those project pages
- Or just leave them as gallery-only projects (fine for now)

---

## GitHub Instructions

1. **Create the `projects` folder** in your repo
2. **Create subfolders** for each project
3. **Add `index.html`** to each project folder (use the template)
4. **Add photos** to each project folder
5. **Push everything to GitHub**

Example Git commands:
```bash
mkdir projects/eoat-tooling
cp projects-template.html projects/eoat-tooling/index.html
# Edit the HTML file, add photos
git add projects/
git commit -m "Add project detail pages"
git push
```

---

## SEO Notes

Each project page automatically gets:
- Meta tags (description, og:image, og:title)
- Proper heading structure (h1, h2, h3)
- Fast load times

To make it even better:
- Use descriptive filenames for photos (`technical-drawing-v2.jpg` is better than `img1.jpg`)
- Write genuine content in the Technical Details section
- Link to your GitHub repos if you have code for the project

---

## Example: cnc-ai-operator project

Here's what `projects/cnc-ai-operator/index.html` would look like:

```html
<!-- In the <h1> -->
<h1>DIY CNC Mill with AI Control</h1>
<p class="meta">January 2025 · Solo Project</p>

<!-- In Overview -->
<p>Built a fully functional CNC milling machine in my home workshop, 
then added a web-based AI interface (Google Gemini) that lets me 
command it in plain English. Also integrated computer vision (OpenCV) 
for real-time monitoring.</p>

<!-- In photos section, add actual images -->
<img src="mill-overview.jpg" alt="Complete CNC setup">
<img src="web-interface.jpg" alt="AI control panel">

<!-- Specs -->
<div class="spec-item">
  <div class="spec-label">Work Area</div>
  <div class="spec-value">350×350×80mm</div>
</div>

<!-- Skills -->
<span class="tag">Python</span>
<span class="tag">Flask</span>
<span class="tag">OpenCV</span>
<span class="tag">Linux</span>
<span class="tag">CNCjs</span>
```

---

## Do NOT

- Don't fake testimonials or reviews
- Don't copy this text exactly — write your own descriptions
- Don't break the folder structure — links depend on it being exact

---

## Questions?

If a "View project" link in the main portfolio shows a 404, it means either:
1. The `projects/` folder doesn't exist yet
2. The subfolder name is wrong (check spelling and lowercase)
3. The `index.html` file isn't inside that folder

Double-check the folder structure above and you'll be fine.
