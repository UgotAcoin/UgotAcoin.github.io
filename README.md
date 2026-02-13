# Game Developer Portfolio

A clean, professional portfolio website for showcasing your game development projects and skills.

## 🚀 Quick Start - GitHub Pages Setup

### 1. Create a GitHub Repository

1. Go to [GitHub](https://github.com) and create a new repository
2. Name it `yourusername.github.io` (replace `yourusername` with your actual GitHub username)
   - Example: If your username is `johndoe`, name it `johndoe.github.io`
3. Make it **Public**
4. Do NOT initialize with README (we already have files)

### 2. Upload Your Portfolio

**Option A: Using GitHub Web Interface (Easiest)**
1. In your new repository, click "uploading an existing file"
2. Drag and drop these files:
   - `index.html`
   - `style.css`
   - `script.js`
   - `README.md`
3. Commit the files

**Option B: Using Git Command Line**
```bash
git init
git add .
git commit -m "Initial portfolio commit"
git branch -M main
git remote add origin https://github.com/yourusername/yourusername.github.io.git
git push -u origin main
```

### 3. Enable GitHub Pages

1. Go to your repository Settings
2. Click on "Pages" in the left sidebar
3. Under "Source", select "main" branch
4. Click Save

Your site will be live at `https://yourusername.github.io` in a few minutes!

## ✏️ Customization Guide

### Personal Information

**Update these sections in `index.html`:**

1. **Line 6** - Page title:
   ```html
   <title>Your Name - Game Developer Portfolio</title>
   ```

2. **Line 11** - Nav brand (your name):
   ```html
   <div class="nav-brand">YourName</div>
   ```

3. **Line 22-23** - Hero section:
   ```html
   <h1>Game Developer</h1>
   <p class="hero-subtitle">Specializing in...</p>
   ```

4. **Line 34-44** - About section - write your own bio

5. **Line 189-200** - Contact links:
   ```html
   <a href="mailto:your.email@example.com">...</a>
   <a href="https://github.com/yourusername">...</a>
   <a href="https://linkedin.com/in/yourprofile">...</a>
   ```

### Adding Your Projects

Each project card follows this structure:

```html
<div class="project-card">
    <div class="project-image">
        <img src="your-screenshot.png" alt="Project Name">
    </div>
    <div class="project-content">
        <h3>Your Project Title</h3>
        <p class="project-tech">Technologies • Used • Here</p>
        <p class="project-description">
            Describe what you built, what problems you solved,
            and what makes it technically interesting.
        </p>
        <div class="project-links">
            <a href="https://github.com/you/project" class="project-link">GitHub</a>
            <a href="https://youtu.be/demo" class="project-link">Demo</a>
        </div>
    </div>
</div>
```

**To add project screenshots:**
1. Add image files to your repository (create an `images` folder)
2. Update the `src` attribute: `<img src="images/project1.png" alt="Project Name">`

**Or use screenshots from your GitHub repository:**
- Upload images to your GitHub repo
- Use the raw GitHub URL: `https://raw.githubusercontent.com/yourusername/repo/main/screenshot.png`

### Updating Skills

Modify the skills section (lines 148-187) to match your actual skillset.

### Color Scheme

Want to change colors? Edit the CSS variables in `style.css` (lines 8-15):

```css
:root {
    --primary-color: #2C3E50;      /* Main dark color */
    --secondary-color: #3498DB;    /* Accent color (links, highlights) */
    --accent-color: #E74C3C;       /* Not currently used, but available */
    --text-primary: #2C3E50;
    --text-secondary: #7F8C8D;
    --bg-light: #ECF0F1;
    --bg-white: #FFFFFF;
}
```

## 📸 Adding Images

### Project Screenshots

1. **Local Images:**
   - Create an `images` folder in your repository
   - Add your screenshots there
   - Reference them: `<img src="images/screenshot.png">`

2. **From GitHub Repository:**
   - Upload to your game project repo
   - Get the raw URL (click image → Raw button)
   - Use that URL in your src attribute

3. **From External Hosting:**
   - Upload to Imgur, CloudFlare, etc.
   - Use the direct image URL

### Profile Photo (Optional)

Add to the About section:
```html
<div class="about-content">
    <img src="images/profile.jpg" alt="Your Name" style="width: 200px; border-radius: 50%; margin-bottom: 2rem;">
    <p>Your bio here...</p>
</div>
```

## 🎨 Advanced Customization

### Adding More Sections

Copy any section and modify it:
```html
<section id="new-section" class="new-section">
    <div class="container">
        <h2>Section Title</h2>
        <!-- Your content -->
    </div>
</section>
```

### Adding a Resume PDF

1. Add your resume PDF file to the repository
2. Update the resume link (line 198):
   ```html
   <a href="resume.pdf" target="_blank" class="contact-btn">Resume</a>
   ```

### Custom Domain (Optional)

1. Buy a domain (e.g., from Namecheap, Google Domains)
2. In your repository, create a file named `CNAME`
3. Add your domain: `yourname.dev`
4. Configure DNS settings at your domain provider

## 📱 Testing

- Test on mobile: Use Chrome DevTools (F12 → Toggle Device Toolbar)
- Check all links work
- Verify images load
- Test on actual mobile devices

## 🔧 Troubleshooting

**Site not loading?**
- Wait 5-10 minutes after first deployment
- Check GitHub Pages is enabled in Settings
- Ensure repository is public
- Verify the repository name is `yourusername.github.io`

**Images not showing?**
- Check file paths are correct
- Ensure images are committed to the repository
- Try using absolute URLs for external images

**CSS not applying?**
- Clear browser cache (Ctrl+Shift+R)
- Check `style.css` is in the same folder as `index.html`

## 📝 Tips for Game Dev Portfolios

1. **Quality over quantity** - Show your 3-4 best projects
2. **Be specific** - "Implemented client-side prediction reducing perceived latency by 40%" is better than "worked on networking"
3. **Include metrics** - Frame rates, player counts, performance improvements
4. **Show code** - Link to GitHub repos when possible
5. **Add videos** - GIFs or YouTube demos are powerful
6. **Keep it updated** - Add new projects as you build them

## 🎓 Next Steps

- [ ] Replace all placeholder text with your information
- [ ] Add your actual projects with descriptions
- [ ] Upload project screenshots
- [ ] Test all links
- [ ] Add your resume PDF
- [ ] Share on LinkedIn, Twitter, and in job applications

Good luck with your job search! 🚀
