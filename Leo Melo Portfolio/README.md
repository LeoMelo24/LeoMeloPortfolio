# Leo Melo Portfolio

A modern, responsive portfolio website showcasing skills, projects, and professional experience.

## 🌟 Features

- **Responsive Design**: Fully responsive layout that works seamlessly on desktop, tablet, and mobile devices
- **Modern UI/UX**: Clean, professional design with smooth animations and transitions
- **Interactive Navigation**: Sticky navigation with active section highlighting
- **Project Showcase**: Beautiful grid layout displaying featured projects with hover effects
- **Skills Section**: Comprehensive display of technical and soft skills
- **Contact Form**: Functional contact form with validation
- **Smooth Scrolling**: Enhanced user experience with smooth scroll behavior
- **SEO Optimized**: Proper meta tags and semantic HTML structure
- **Fast Loading**: Optimized assets and minimal dependencies

## 📁 Project Structure

```
Leo Melo Portfolio/
│
├── index.html              # Main HTML file
├── README.md              # Project documentation
│
├── css/
│   └── style.css          # Main stylesheet with responsive design
│
├── js/
│   └── script.js          # JavaScript for interactivity
│
├── images/                # Image assets
│   ├── profile-placeholder.jpg
│   ├── about-placeholder.jpg
│   ├── project-payroll.jpg
│   ├── project-inventory.jpg
│   ├── project-student.jpg
│   ├── project-chatbot.jpg
│   ├── project-shopify.jpg
│   └── project-wordpress.jpg
│
└── assets/                # Additional assets (CV, documents)
    └── Leo_Melo_CV.pdf   # Resume/CV file (to be added)
```

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- A text editor (VS Code, Sublime Text, etc.) for customization
- Basic knowledge of HTML, CSS, and JavaScript (optional)

### Installation

1. **Clone or Download** the repository
   ```bash
   # If using Git
   git clone https://github.com/LeoMelo24/portfolio.git
   
   # Or download as ZIP and extract
   ```

2. **Navigate** to the project folder
   ```bash
   cd "Leo Melo Portfolio"
   ```

3. **Open** `index.html` in your web browser
   - Double-click the `index.html` file, or
   - Right-click and select "Open with" your preferred browser

### Local Development Server (Optional)

For better development experience, use a local server:

**Using Python:**
```bash
# Python 3.x
python -m http.server 8000

# Python 2.x
python -m SimpleHTTPServer 8000
```

**Using Node.js (with live-server):**
```bash
npx live-server
```

**Using VS Code:**
- Install the "Live Server" extension
- Right-click on `index.html` and select "Open with Live Server"

## 🎨 Customization Guide

### 1. Personal Information

**Update HTML Content** (`index.html`):
- Search for "Leo Melo" and replace with your name
- Update contact information (email, phone, location)
- Modify social media links
- Update education and experience details
- Customize project descriptions

### 2. Replace Placeholder Images

Replace the SVG placeholders in the `images/` folder with your actual photos:
- `profile-placeholder.jpg` - Your profile photo (450x450px recommended)
- `about-placeholder.jpg` - About section photo (350x400px recommended)
- `project-*.jpg` - Project screenshots (600x400px recommended)

### 3. Add Your CV

Place your CV/Resume in the `assets/` folder:
- Name it `Leo_Melo_CV.pdf` or update the link in `index.html`

### 4. Color Scheme

Modify colors in `css/style.css` (CSS Variables):
```css
:root {
    --primary-color: #2563eb;      /* Main brand color */
    --secondary-color: #1e40af;    /* Secondary brand color */
    --accent-color: #3b82f6;       /* Accent color */
    /* ... other colors ... */
}
```

### 5. Fonts

Current font: **Poppins** from Google Fonts

To change fonts, update in `index.html`:
```html
<link href="https://fonts.googleapis.com/css2?family=YourFont:wght@300;400;500;600;700&display=swap" rel="stylesheet">
```

And in `css/style.css`:
```css
:root {
    --font-primary: 'YourFont', sans-serif;
}
```

### 6. Projects

Add/modify projects in the Projects section:
```html
<div class="project-card">
    <div class="project-image">
        <img src="images/your-project.jpg" alt="Project Name">
        <div class="project-overlay">
            <a href="project-url" class="project-link"><i class="fas fa-external-link-alt"></i></a>
        </div>
    </div>
    <div class="project-info">
        <h3>Project Title</h3>
        <p>Project description...</p>
        <div class="project-tags">
            <span class="tag">Tech1</span>
            <span class="tag">Tech2</span>
        </div>
    </div>
</div>
```

### 7. Skills

Update skills in the Skills section by modifying the skill items:
```html
<div class="skill-items">
    <span class="skill-item">Your Skill</span>
    <!-- Add more skills -->
</div>
```

### 8. Contact Form

The contact form currently uses a `mailto:` link. To implement a backend:

**Option 1: FormSpree**
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

**Option 2: Netlify Forms**
```html
<form name="contact" method="POST" data-netlify="true">
```

**Option 3: Custom Backend**
- Modify `js/script.js` contact form handler
- Connect to your backend API

## 🌐 Deployment

### GitHub Pages

1. Create a GitHub repository
2. Push your code to the repository
3. Go to Settings → Pages
4. Select the branch and folder
5. Your site will be available at `https://yourusername.github.io/repository-name`

### Netlify

1. Sign up at [Netlify](https://netlify.com)
2. Drag and drop your project folder
3. Your site will be live instantly

### Vercel

1. Sign up at [Vercel](https://vercel.com)
2. Import your GitHub repository
3. Deploy with one click

### Traditional Web Hosting

1. Compress the entire project folder
2. Upload to your hosting via FTP/cPanel
3. Extract and ensure `index.html` is in the root directory

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Opera (latest)

## 🔧 Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: Modern styling with Flexbox and Grid
- **JavaScript (ES6+)**: Interactive functionality
- **Font Awesome**: Icons
- **Google Fonts**: Typography

## 📋 Features Breakdown

### Navigation
- Fixed navigation bar
- Active link highlighting on scroll
- Smooth scrolling to sections
- Mobile hamburger menu

### Hero Section
- Eye-catching introduction
- Call-to-action buttons
- Social media links
- Animated scroll indicator

### About Section
- Professional summary
- Personal information grid
- Downloadable CV button

### Experience & Education
- Timeline layout
- Detailed work experience
- Educational background

### Projects
- Grid layout with hover effects
- Project overlays
- Technology tags
- Link to project demos

### Skills
- Categorized skill display
- Hover animations
- Soft skills section

### Contact
- Contact information cards
- Functional contact form
- Form validation
- Success notifications

### Additional Features
- Scroll to top button
- Intersection Observer animations
- Responsive design breakpoints
- Loading animations

## 🐛 Troubleshooting

**Images not loading:**
- Ensure images are in the correct folder
- Check file names match HTML references
- Verify image file extensions

**JavaScript not working:**
- Check browser console for errors
- Ensure `script.js` is linked correctly
- Clear browser cache

**Styles not applying:**
- Verify `style.css` is linked in HTML
- Clear browser cache
- Check CSS file path

**Contact form issues:**
- Currently uses mailto: link
- Configure backend service for production
- Check email client is set up

## 📝 To-Do / Future Enhancements

- [ ] Implement blog section
- [ ] Add project filtering by technology
- [ ] Include testimonials section
- [ ] Integrate Google Analytics
- [ ] Add more animation effects
- [ ] Implement multi-language support
- [ ] Add achievement badges
- [ ] Create printable resume version

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👤 Author

**Leo Melo**
- Website: [leomelo.dev](https://leomelo.dev)
- GitHub: [@LeoMelo24](https://github.com/LeoMelo24)
- LinkedIn: [leo-melo-dev](https://linkedin.com/in/leo-melo-dev)
- Email: info@leomelo.dev

## 🙏 Acknowledgments

- Font Awesome for icons
- Google Fonts for typography
- Inspiration from modern portfolio designs
- The web development community

## 📞 Support

For questions or support, please:
- Open an issue on GitHub
- Email: info@leomelo.dev
- Connect on LinkedIn

---

**Note**: Remember to replace all placeholder images with your actual photos and update all personal information before deploying to production.

Made with ❤️ by Leo Melo

