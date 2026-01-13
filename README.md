# Portfolio Website

A modern, responsive portfolio website showcasing frontend and backend projects with smooth animations and interactive features.

## Features

- **Responsive Design**: Fully responsive layout that works on all devices (desktop, tablet, mobile)
- **Modern UI**: Clean and professional design with gradient effects and smooth animations
- **Project Filtering**: Filter projects by category (All, Frontend, Backend, Full Stack)
- **Smooth Scrolling**: Smooth navigation between sections
- **Contact Form**: Functional contact form for visitor inquiries
- **Scroll Animations**: Elements animate as you scroll down the page
- **Mobile Navigation**: Hamburger menu for mobile devices
- **Scroll-to-Top Button**: Quick navigation back to the top of the page
- **Social Media Links**: Connect with visitors through social media

## Sections

1. **Home/Hero**: Introduction with name, title, and call-to-action buttons
2. **About**: Brief description of skills and background
3. **Skills**: Categorized display of frontend, backend, and tools
4. **Projects**: Filterable grid of project cards with images and descriptions
5. **Contact**: Contact form and contact information
6. **Footer**: Copyright and social links

## Technologies Used

- HTML5
- CSS3 (with CSS Variables and Animations)
- Vanilla JavaScript (ES6+)
- Font Awesome Icons

## Customization Guide

### 1. Personal Information

Edit `index.html` to update:
- Your name in the hero section (line 41)
- Your role/title (line 42)
- About section description (lines 61-70)
- Contact information (lines 308-320)

### 2. Projects

To add/edit projects, modify the project cards in `index.html` (starting at line 156):

```html
<div class="project-card" data-category="frontend">
    <div class="project-image">
        <img src="your-image-url" alt="Project Name">
        <div class="project-overlay">
            <a href="live-demo-url" class="project-link" target="_blank">
                <i class="fas fa-external-link-alt"></i>
            </a>
            <a href="github-url" class="project-link" target="_blank">
                <i class="fab fa-github"></i>
            </a>
        </div>
    </div>
    <div class="project-content">
        <h3>Project Title</h3>
        <p>Project description...</p>
        <div class="project-tags">
            <span class="tag">Technology 1</span>
            <span class="tag">Technology 2</span>
        </div>
    </div>
</div>
```

**Categories**: Use `data-category` attribute with values:
- `frontend` - Frontend projects
- `backend` - Backend projects
- `fullstack` - Full stack projects

### 3. Skills

Update the skills in `index.html` (lines 85-125). Add or remove `<span class="skill-item">` tags:

```html
<span class="skill-item">Your Skill</span>
```

### 4. Colors

Customize the color scheme in `styles.css` by modifying CSS variables (lines 2-10):

```css
:root {
    --primary-color: #6366f1;     /* Main accent color */
    --secondary-color: #8b5cf6;   /* Secondary accent color */
    --text-color: #1f2937;        /* Main text color */
    --text-light: #6b7280;        /* Light text color */
    --bg-color: #ffffff;          /* Background color */
    --bg-secondary: #f9fafb;      /* Secondary background */
}
```

### 5. Social Media Links

Update social media URLs in `index.html`:
- Hero section social links (lines 50-54)
- Footer social links (lines 335-339)

Replace `#` with your actual social media profile URLs.

### 6. Project Images

Replace placeholder images with your actual project screenshots. Options:
- Use image URLs from your projects
- Create an `images` folder and use relative paths: `images/project-name.jpg`
- Use services like Imgur or Cloudinary to host images

### 7. Contact Form

The contact form currently shows an alert. To make it functional:

1. **Option A: Using a Backend API**
   - Uncomment the fetch code in `script.js` (lines 91-107)
   - Replace `/api/contact` with your backend endpoint
   - Create a backend API to handle form submissions

2. **Option B: Using FormSubmit or Similar Service**
   - Update the form action in `index.html`:
   ```html
   <form action="https://formsubmit.co/your@email.com" method="POST">
   ```

3. **Option C: Using EmailJS**
   - Sign up at [EmailJS](https://www.emailjs.com/)
   - Follow their documentation to integrate

## Optional Enhancements

### Enable Typing Effect

Uncomment line 178 in `script.js` to enable the typing effect for the hero subtitle:
```javascript
typeEffect();
```

### Add More Animations

The scroll reveal animations are already implemented. You can add more elements to animate by adding them to the selector on line 123 of `script.js`.

## Installation & Usage

1. Download or clone this repository
2. Open `index.html` in your web browser
3. Customize the content as described above
4. Deploy to your preferred hosting service

## Deployment Options

- **GitHub Pages**: Free hosting for static sites
- **Netlify**: Drag and drop deployment
- **Vercel**: Simple deployment with Git integration
- **Traditional Hosting**: Upload files via FTP

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## File Structure

```
web-portofolio/
│
├── index.html          # Main HTML file
├── styles.css          # All styles and animations
├── script.js           # JavaScript functionality
└── README.md          # Documentation (this file)
```

## Tips for Best Results

1. **Images**: Use high-quality project screenshots (recommended size: 800x500px)
2. **Descriptions**: Keep project descriptions concise (2-3 sentences)
3. **Links**: Ensure all project links work (live demos and GitHub repos)
4. **Testing**: Test on multiple devices and browsers
5. **Performance**: Optimize images for web (compress before uploading)
6. **SEO**: Update meta tags in the `<head>` section

## License

Feel free to use this template for your personal portfolio. No attribution required.

## Support

If you encounter any issues or have questions, feel free to modify the code to suit your needs.

---

**Built with ❤️ for developers**
