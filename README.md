# Personal Portfolio Website

A modern, responsive portfolio website to showcase your resume, projects, and professional information.

## Features

- **Responsive Design**: Works perfectly on desktop, tablet, and mobile devices
- **Modern UI**: Clean, professional design with smooth animations
- **Interactive Elements**: Hover effects, smooth scrolling, and animated transitions
- **Contact Form**: Built-in contact form with validation
- **Project Showcase**: Dedicated section to display your projects
- **Skills Section**: Visual representation of your technical skills
- **Resume Section**: Timeline-based resume display with download option
- **SEO Friendly**: Proper HTML structure and meta tags

## File Structure

```
portfolio-website/
├── index.html          # Main HTML file
├── css/
│   └── styles.css      # Stylesheet
├── js/
│   └── script.js       # JavaScript functionality
├── images/             # Image assets
└── files/              # Resume and other files
```

## Customization Guide

### 1. Personal Information

Edit the following sections in `index.html`:

- **Navigation Logo**: Line 16 - Replace "Your Name" with your actual name
- **Hero Section**: Lines 37-42 - Update name, title, and description
- **Contact Information**: Lines 257-265 - Add your email, phone, and location
- **Footer**: Line 302 - Update copyright information

### 2. About Section

- **Line 63-66**: Replace the placeholder text with your personal story
- **Line 67-70**: Update your background and interests
- **Lines 74-97**: Modify the skills icons and names to match your expertise

### 3. Projects Section

For each project (Lines 111-186):
- Replace project images in the `images/` folder
- Update project titles and descriptions
- Modify technology tags to reflect what you used
- Add your actual project and GitHub links

### 4. Resume Section

- **Lines 208-223**: Update your work experience
- **Lines 231-238**: Modify your education information
- Add a PDF resume file to a `files/` folder and update the download link (Line 197)

### 5. Social Links

Update your social media links in the contact section (Lines 269-277).

## Setup Instructions

### Option 1: Direct File Opening
1. Double-click `index.html` to open in your browser
2. The website will work locally for testing

### Option 2: Local Server (Recommended)
1. Install a local server (Python, Node.js, or VS Code Live Server)
2. Serve the files from the project directory

**Python:**
```bash
cd portfolio-website
python -m http.server 8000
```

**Node.js (with http-server):**
```bash
npm install -g http-server
cd portfolio-website
http-server
```

### Option 3: Deploy Online
Deploy to platforms like:
- GitHub Pages
- Netlify
- Vercel
- Firebase Hosting

## Adding Images

1. **Profile Photo**: Add `profile.jpg` to the `images/` folder
2. **Project Images**: Add `project1.jpg`, `project2.jpg`, `project3.jpg` to the `images/` folder
3. **Resume**: Add your `resume.pdf` to a `files/` folder

## Color Customization

The website uses a blue color scheme. To change colors, modify these CSS variables in `styles.css`:

```css
/* Primary color (blue) */
#2563eb → Your preferred color

/* Accent color (yellow) */
#fbbf24 → Your preferred accent color
```

## Typography

The website uses Inter font from Google Fonts. To change the font:
1. Update the Google Fonts link in `index.html` (Line 8)
2. Update the font-family in `styles.css` (Line 9)

## Browser Support

- Chrome (recommended)
- Firefox
- Safari
- Edge
- Internet Explorer 11+

## Performance Tips

1. Optimize images (use WebP format if possible)
2. Minify CSS and JavaScript for production
3. Use a CDN for faster loading
4. Enable gzip compression on your server

## Contact Form Setup

The contact form currently shows a success message without actually sending emails. To make it functional:

1. **Backend Integration**: Connect to a server-side script (PHP, Node.js, Python)
2. **Email Service**: Use services like EmailJS, Formspree, or Netlify Forms
3. **Database**: Store messages in a database if needed

### EmailJS Setup (Recommended for static hosting):
1. Sign up at [EmailJS](https://www.emailjs.com/)
2. Create an email service and template
3. Replace the form submission code in `script.js` with EmailJS integration

## Customization Examples

### Changing the Hero Background
```css
.hero {
    background: linear-gradient(135deg, #your-color1 0%, #your-color2 100%);
}
```

### Adding More Skills
```html
<div class="skill-item">
    <i class="fab fa-your-icon"></i>
    <span>Your Skill</span>
</div>
```

### Adding More Projects
Copy the project card structure and update the content:
```html
<div class="project-card">
    <!-- Project content -->
</div>
```

## Support

If you need help customizing the website:
1. Check the code comments for guidance
2. Refer to this README file
3. Look up CSS/HTML/JavaScript tutorials online

## License

This template is free to use for personal and commercial projects.

---

**Happy coding! 🚀**
