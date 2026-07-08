# Navigation & Structure Guide

## 🎉 WHAT'S BEEN COMPLETED

Your portfolio is now **fully structured and connected**! Here's what's been set up:

### ✅ All 6 Project Pages Created
1. End-of-Arm Tooling (EOAT) - Featured project
2. DIY CNC Milling Machine
3. AI-Powered CNC Operator  
4. Structural Steel Squat Rack
5. ATG Internship - Robotics & Automation
6. Reverse Engineering - Aircraft Component

### ✅ All Navigation Links Added
- Main portfolio → Click any project card → Goes to project detail page
- All project pages → Click "← Back to portfolio" → Returns to main portfolio
- Featured EOAT card has special hover effects and call-to-action

### ✅ Professional Project Pages
Each project page includes:
- Project title, date, and role
- Comprehensive overview
- Image gallery layout (ready for your photos)
- Key specifications display
- Technical details sections  
- Skills & technologies used
- Contact links and GitHub integration

**→ The only thing left to do: Add your image files!** (See "Next Steps" section below)

---

## 🔗 Links Between Pages

### Main Portfolio → Project Pages
- **Featured Project Card**: Click anywhere on the EOAT featured project card to go to the detailed project page
- Visual feedback: The card now has hover effects (lift animation) and a "View full project details →" call-to-action link
- Path: `/projects/eoat-tooling/`

### Project Pages → Main Portfolio
- **Back Link**: Located at the top of each project page
- Path: `← Back to portfolio` (appears in both header and above the title)
- Works on all project detail pages

---

## 📂 File Structure

```
github-portfolio/
│
├── index.html                          ← Main portfolio homepage (fully linked!)
├── NAVIGATION_GUIDE.md                 ← This file
├── FILENAMES_REFERENCE.md              ← Image naming reference
├── PROJECT_PAGES_SETUP.md              ← Setup instructions
│
└── projects/
    ├── eoat-tooling/
    │   ├── index.html                  ✅ DONE
    │   └── (images: eoat-assembly.jpg, solidworks-model.jpg, technical-drawing.jpg, robot-cell.jpg)
    ├── cnc-milling/
    │   ├── index.html                  ✅ DONE
    │   └── (images: machine-overview.jpg, cnc-in-action.jpg, solidworks-cad.jpg)
    ├── cnc-ai-operator/
    │   ├── index.html                  ✅ DONE
    │   └── (images: web-interface.jpg, cncjs-screenshot.jpg, wiring.jpg)
    ├── squat-rack/
    │   ├── index.html                  ✅ DONE
    │   └── (images: rack-render.jpg, solidworks-drawing.jpg, fabricated.jpg)
    ├── atg-internship/
    │   ├── index.html                  ✅ DONE
    │   └── (images: fanuc-robot.jpg, eoat-adapter.jpg, bin-picking.jpg)
    └── reverse-engineering/
        ├── index.html                  ✅ DONE
        └── (images: cmm-measurement.jpg, solidworks-reconstruction.jpg, iso-drawing.jpg)
```

---

## 🎯 How to Add More Projects

### Step 1: Create a new folder
Copy the entire `projects/eoat-tooling/` folder and rename it:
- `projects/cnc-milling/`
- `projects/squat-rack/`
- `projects/atg-internship/`
- etc.

### Step 2: Update the project page
Edit the new project's `index.html`:

1. **Update meta tags** (top of file):
   ```html
   <meta name="description" content="YOUR PROJECT TITLE - Description here">
   <meta property="og:title" content="YOUR PROJECT TITLE | Matěj Král">
   <meta property="og:description" content="Short description">
   <meta property="og:image" content="../your-image.jpg">
   <title>YOUR PROJECT TITLE | Matěj Král</title>
   ```

2. **Update page content** (body section):
   - Replace `<h1>` with your project title
   - Replace `<p class="meta">` with project date and role
   - Update Overview section
   - Update image filenames in image grid
   - Update Specifications
   - Update Technical Details
   - Update Skills & Technologies tags

3. **Add project images**:
   - Place images in the project folder with the exact filenames referenced in the HTML

### Step 3: Add link from main portfolio
In the main `index.html`, find the "Selected Projects" section and add a project card:

```html
<article class="project-card">
  <a href="projects/your-project-folder/" style="text-decoration: none; color: inherit;">
    <div class="project-gallery">
      <!-- Add your gallery images -->
      <div class="gallery-thumb" onclick="openLightbox('project-id', 0)" role="button"></div>
    </div>
    <h3>Your Project Title</h3>
    <p class="project-copy">Project description...</p>
    <p style="color: var(--accent); font-weight: 600;">View details →</p>
  </a>
</article>
```

---

## ✅ Key Improvements Made

### 🎉 **ALL PROJECTS FULLY SET UP AND LINKED**

1. **6 Complete Project Pages**
   - ✅ End-of-Arm Tooling (EOAT) - Featured project link from main portfolio
   - ✅ DIY CNC Milling Machine - Full technical documentation
   - ✅ AI-Powered CNC Operator - Flask + WebSocket backend showcase
   - ✅ Structural Steel Squat Rack - FEA & DFM analysis
   - ✅ ATG Internship - Robotics & automation projects
   - ✅ Reverse Engineering - Aircraft component reconstruction

2. **Navigation Working Both Ways**
   - Main portfolio → Click any project card → Goes to detailed project page
   - Project pages → Click "← Back to portfolio" → Returns to main portfolio
   - All 6 projects are fully clickable and navigable

3. **All Links Fixed**
   - ✅ CNC Milling link corrected to point to `/projects/cnc-milling/`
   - ✅ Squat Rack now has working link
   - ✅ ATG Internship now has working link
   - ✅ Reverse Engineering now has working link
   - ✅ Featured EOAT card is clickable with hover effects

4. **Each Project Page Includes**
   - Clear project title and date/role
   - Comprehensive overview section
   - Image gallery with placeholder filenames
   - Key specifications in organized layout
   - Technical details explaining the engineering
   - Skills and technologies used
   - Contact information and GitHub links
   - Consistent design matching main portfolio

5. **File Structure is Clean**
   - All projects in `/projects/` folder
   - Relative image paths work across all pages
   - Portable structure - can be moved anywhere
   - No external dependencies beyond Google Fonts

---

## 🚀 Next Steps - Add Your Images!

The structure is complete. Now you just need to add images to each project folder:

### EOAT Tooling (`projects/eoat-tooling/`)
- `eoat-assembly.jpg` - Complete assembly mounted on robot
- `solidworks-model.jpg` - 3D CAD model screenshot
- `technical-drawing.jpg` - ISO 13715 drawing
- `robot-cell.jpg` - Full robot cell integration

### CNC Milling (`projects/cnc-milling/`)
- `machine-overview.jpg` - Complete CNC machine photo
- `cnc-in-action.jpg` - Machine operating/cutting material
- `solidworks-cad.jpg` - CAD model or screenshot

### AI CNC Operator (`projects/cnc-ai-operator/`)
- `web-interface.jpg` - Web dashboard screenshot
- `cncjs-screenshot.jpg` - CNCjs interface
- `wiring.jpg` - Hardware connections/electronics

### Squat Rack (`projects/squat-rack/`)
- `rack-render.jpg` - SolidWorks 3D render
- `solidworks-drawing.jpg` - Technical drawing
- `fabricated.jpg` - Actual fabricated rack photo

### ATG Internship (`projects/atg-internship/`)
- `fanuc-robot.jpg` - FANUC robot setup
- `eoat-adapter.jpg` - 3D printed adapter
- `bin-picking.jpg` - Bin picking system in action

### Reverse Engineering (`projects/reverse-engineering/`)
- `cmm-measurement.jpg` - CMM measurement setup/point cloud
- `solidworks-reconstruction.jpg` - Reconstructed CAD model
- `iso-drawing.jpg` - Aerospace technical drawing

### Gallery Photos for Main Portfolio Root (already referenced)
Keep these in the root folder (`/`):
- `photo.jpg` - Your hero portrait
- `eoat-assembly.jpg`, `solidworks-model.jpg`, `technical-drawing.jpg`, `robot-cell.jpg`
- `czechskills-podium.jpg`, `czechskills-programming.jpg`, `czechskills-diploma-photo.jpg`
- Plus all other gallery images for the main portfolio sections

---

## ✨ Testing Your Portfolio

1. **Open main portfolio** (`index.html`)
2. **Click featured EOAT card** → Should navigate to `/projects/eoat-tooling/`
3. **Click "View project →" buttons** → Should navigate to each project page
4. **Click "← Back to portfolio"** → Should return to main page
5. **All images display** → If image files are named correctly and placed in right folders

---

## 📋 Quick Checklist

- [ ] Add all image files to project folders (see filename lists above)
- [ ] Test clicking on all project cards from main portfolio
- [ ] Test "Back to portfolio" links on each project page
- [ ] Verify all images load correctly
- [ ] Check responsive design on mobile (click hamburger menu)
- [ ] Update GitHub username in portfolio (replace YOUR-USERNAME placeholders if any remain)
- [ ] Test on different browsers (Chrome, Firefox, Safari, Edge)

---

## 📋 For Future Edits

- All project pages have the same structure for consistency
- Image file paths are relative (`../filename.jpg`) for easy portability
- The CSS is built into each HTML file for simplicity
- No external dependencies beyond Google Fonts
