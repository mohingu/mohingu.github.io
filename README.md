# Portfolio Website - Mohin Uddin

Personal portfolio website showcasing my work, experience, and projects.

🌐 **Live Site:** [https://mohingu.github.io](https://mohingu.github.io)

## Features

- ✨ Modern, responsive design
- 🌓 Dark/Light mode toggle
- 📱 Mobile-friendly
- 🎨 Smooth animations and transitions
- 📺 YouTube channel embeds
- 🎯 Project showcase
- 📧 Contact section with social links

## Sections

1. **Hero** - Introduction and call-to-action
2. **About** - Personal introduction and skills
3. **Experience** - Work history and achievements
4. **Education** - Academic background
5. **Projects** - Portfolio of apps and projects
6. **Certificates** - Professional certifications
7. **YouTube** - Embedded videos from both channels
8. **Contact** - Get in touch

## Customization Guide

### 1. Update Personal Information

#### Hero Section (`index.html` lines 31-62)
- Change your name, title, and description
- Update social media links (GitHub, LinkedIn, YouTube)

#### About Section (`index.html` lines 69-103)
- Rewrite the "About Me" paragraphs
- Update skills in the skills grid
- Add or remove skill tags

### 2. Add Your Experience

Find the Experience section (`index.html` lines 107-151) and replace the placeholder entries:

```html
<div class="timeline-item">
    <div class="timeline-dot"></div>
    <div class="timeline-content">
        <h3>Your Job Title</h3>
        <h4>Company Name</h4>
        <span class="timeline-date">Start Date - End Date</span>
        <ul class="timeline-description">
            <li>Your achievement or responsibility</li>
            <li>Another key point</li>
        </ul>
    </div>
</div>
```

### 3. Add Your Education

Find the Education section (`index.html` lines 155-180) and update with your degrees:

```html
<div class="timeline-item">
    <div class="timeline-dot"></div>
    <div class="timeline-content">
        <h3>Your Degree</h3>
        <h4>University Name</h4>
        <span class="timeline-date">Year - Year</span>
        <div class="timeline-description">
            <p><strong>Major:</strong> Your Major</p>
            <p><strong>GPA:</strong> X.XX/4.0</p>
        </div>
    </div>
</div>
```

### 4. Customize Projects

Find the Projects section (`index.html` lines 184-286) and update each project card:

- Replace placeholder images with your project screenshots
- Update project titles, descriptions, and tech tags
- Add links to live demos and GitHub repos

**Getting Project Screenshots:**
- Take screenshots of your projects
- Add them to an `images/` folder
- Update image src: `<img src="images/your-project.png" alt="Project Name">`

### 5. Add Certificates

Find the Certificates section (`index.html` lines 290-320) and add your certifications:

```html
<div class="certificate-card">
    <div class="certificate-icon">
        <i class="fas fa-certificate"></i>
    </div>
    <h3>Certificate Name</h3>
    <p class="certificate-issuer">Issuing Organization</p>
    <p class="certificate-date">Month Year</p>
    <a href="link-to-certificate" class="certificate-link" target="_blank">View Certificate</a>
</div>
```

### 6. Embed YouTube Videos

Find the YouTube section (`index.html` lines 324-397).

**To get video embed codes:**
1. Go to your YouTube video
2. Click "Share" → "Embed"
3. Copy the video ID from the URL (e.g., `dQw4w9WgXcQ`)
4. Replace `VIDEO_ID_1`, `VIDEO_ID_2`, etc. with your actual video IDs

Update channel names and links:
```html
<h3><i class="fab fa-youtube"></i> Your Channel Name</h3>
<a href="https://youtube.com/@yourchannel" target="_blank">
```

### 7. Update Contact Information

Find the Contact section (`index.html` lines 401-440) and update:
- Email address
- Location
- Social media links

### 8. Change Colors (Optional)

Edit `styles.css` (lines 1-20) to customize the color scheme:

```css
:root {
    --primary-color: #667eea;  /* Main brand color */
    --secondary-color: #764ba2; /* Secondary brand color */
    --accent-color: #f093fb;    /* Accent color */
}
```

## Deployment to GitHub Pages

1. **Create Repository**
   - Go to GitHub and create a new repository
   - Name it **exactly**: `mohingu.github.io`
   - Make it **public**

2. **Push Your Code**
   ```bash
   cd mohingu.github.io
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/mohingu/mohingu.github.io.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to repository Settings → Pages
   - Source: Deploy from branch `main`
   - Folder: `/ (root)`
   - Click Save

4. **Visit Your Site**
   - Your site will be live at: `https://mohingu.github.io`
   - May take a few minutes to deploy

## Adding Images

1. Create an `images` folder in the root directory
2. Add your images there
3. Reference them in HTML: `<img src="images/your-image.jpg" alt="Description">`

## Tech Stack

- **HTML5** - Structure
- **CSS3** - Styling with CSS Variables
- **JavaScript** - Interactivity and animations
- **Font Awesome** - Icons
- **GitHub Pages** - Hosting

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Performance Tips

- Optimize images before uploading (use tools like TinyPNG)
- Keep images under 500KB each
- Use webp format for better compression

## License

Feel free to use this template for your own portfolio!

## Questions?

If you need help customizing your portfolio, feel free to reach out!

---

Built with ❤️ by Mohin Uddin

