# Kriya Tutorials - Landing Page

A modern, responsive landing page for **Kriya Tutorials**, a professional Maths & Science tutoring service based in Cambridge, UK.

![Kriya Tutorials](https://img.shields.io/badge/Education-Tutoring-blue)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## 📋 Table of Contents

- [Features](#features)
- [Demo](#demo)
- [Installation](#installation)
- [Usage](#usage)
- [Customization](#customization)
- [Contact Form Setup](#contact-form-setup)
- [Browser Support](#browser-support)
- [File Structure](#file-structure)
- [Technologies Used](#technologies-used)
- [License](#license)

## ✨ Features

### Design & UI
- 🎨 **Modern Gradient Design** - Beautiful purple/blue gradient color scheme
- 📱 **Fully Responsive** - Works perfectly on all devices (desktop, tablet, mobile)
- ✨ **Smooth Animations** - Engaging hover effects and transitions
- 🎯 **Professional Layout** - Clean, organized sections with clear hierarchy
- 🌟 **Decorative Elements** - Floating gradient backgrounds and animated icons

### Sections
1. **Header/Navigation**
   - Sticky header with blur effect
   - Smooth scroll navigation
   - Educational logo with graduation cap icon

2. **Hero Section**
   - Eye-catching headline
   - Clear value proposition
   - Call-to-action button

3. **Features Section**
   - 6 key benefits with icons
   - Animated hover cards
   - Compressed, scannable content

4. **Subjects Section**
   - Subjects offered (Maths, Physics, Chemistry, Biology, Further Maths)
   - GCSE & A-Level specifications
   - Glass-morphism design with hover effects

5. **Testimonials Section**
   - Student and parent testimonials
   - Quote styling with decorative elements
   - Social proof for credibility

6. **Contact Section**
   - Contact information (email, phone, location)
   - Multiple call-to-action buttons
   - Modal contact form

7. **Footer**
   - Copyright information
   - Professional branding

### Interactive Contact Form
- 📝 **Modal Popup Form** - Opens when clicking CTA buttons
- 📧 **Email Integration** - Sends inquiries to vikash.tigs@gmail.com
- ✅ **Form Validation** - Required field validation
- 🎨 **Beautiful Design** - Smooth animations and professional styling
- ⌨️ **Keyboard Support** - Close with ESC key
- 📱 **Mobile Optimized** - Works perfectly on all screen sizes

## 🚀 Demo

Simply open the `kriya-tutorials-landing.html` file in any modern web browser to see the landing page in action.

## 📥 Installation

1. **Download the file**
   ```bash
   # Download kriya-tutorials-landing.html to your computer
   ```

2. **No build process required** - This is a single, self-contained HTML file with embedded CSS and JavaScript

3. **Open in browser**
   ```bash
   # Double-click the file, or
   # Right-click → Open with → Your browser of choice
   ```

## 💻 Usage

### For Development
```bash
# Simply open the HTML file in your browser
open kriya-tutorials-landing.html

# Or with a local server (optional)
python -m http.server 8000
# Then visit http://localhost:8000/kriya-tutorials-landing.html
```

### For Deployment
Upload the `kriya-tutorials-landing.html` file to any web hosting service:
- GitHub Pages
- Netlify
- Vercel
- Traditional web hosting (cPanel, etc.)

## 🎨 Customization

### Changing Colors
Find and replace the gradient colors in the `<style>` section:

```css
/* Primary gradient (purple/blue) */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);

/* Change to your brand colors, e.g., green/teal */
background: linear-gradient(135deg, #11998e 0%, #38ef7d 100%);
```

### Updating Contact Information

1. **Email Address**
   ```javascript
   // Find this line in the JavaScript section (near the end)
   const mailtoLink = `mailto:vikash.tigs@gmail.com?subject=...`;
   
   // Change to your email
   const mailtoLink = `mailto:your.email@example.com?subject=...`;
   ```

2. **Phone Number**
   ```html
   <!-- Find in the contact section -->
   <p>📱 <a href="tel:+441223123456">+44 1223 123 456</a></p>
   
   <!-- Update to your number -->
   <p>📱 <a href="tel:+1234567890">+1 234 567 890</a></p>
   ```

3. **Location**
   ```html
   <p>📍 Cambridge, UK</p>
   
   <!-- Change to your location -->
   <p>📍 Your City, Country</p>
   ```

### Modifying Content

All content is in plain HTML. Simply find the section you want to modify and update the text:

```html
<!-- Hero Section -->
<h1>Excel in Maths & Science</h1>
<p>Expert tutoring in Cambridge...</p>

<!-- Update to your content -->
<h1>Your Headline Here</h1>
<p>Your description here...</p>
```

### Adding/Removing Subjects
```html
<!-- In the subjects section -->
<div class="subject-card">
    <h3>📐 Mathematics</h3>
    <p>GCSE & A-Level</p>
</div>

<!-- Add more subjects by copying and pasting -->
<div class="subject-card">
    <h3>🎭 Drama</h3>
    <p>GCSE</p>
</div>
```

## 📧 Contact Form Setup

### How It Works
1. User clicks "Book Your Free Consultation" or "Contact Us Now"
2. Modal popup appears with the contact form
3. User fills in: Name, Phone, Email, Message
4. On submit, it opens the user's default email client with:
   - **To:** vikash.tigs@gmail.com
   - **Subject:** Free Consultation Request from [Name]
   - **Body:** Formatted with all form details

### Email Configuration
```javascript
// Find this function in the script section
function submitForm(event) {
    event.preventDefault();
    
    const name = document.getElementById('name').value;
    const phone = document.getElementById('phone').value;
    const email = document.getElementById('email').value;
    const message = document.getElementById('message').value;
    
    // Update the email recipient here
    const mailtoLink = `mailto:YOUR_EMAIL@example.com?subject=...`;
    
    window.location.href = mailtoLink;
}
```

### Alternative: Backend Integration
If you want to send emails directly without opening the email client, you'll need to integrate with a backend service:

**Options:**
- **Formspree** - https://formspree.io
- **EmailJS** - https://www.emailjs.com
- **Google Forms** - Free and simple
- **Custom Backend** - PHP, Node.js, Python, etc.

## 🌐 Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

**Note:** The page uses modern CSS features like:
- CSS Grid
- Flexbox
- CSS Gradients
- Backdrop filters
- CSS Animations

Older browsers (IE11 and below) are not supported.

## 📁 File Structure

```
kriya-tutorials-landing.html
│
├── <head>
│   ├── Meta tags (charset, viewport)
│   ├── Title
│   └── <style> (embedded CSS)
│       ├── Global styles
│       ├── Header/Navigation
│       ├── Hero section
│       ├── Features section
│       ├── Subjects section
│       ├── Testimonials section
│       ├── Contact section
│       ├── Modal styles
│       ├── Footer
│       └── Responsive styles (@media queries)
│
└── <body>
    ├── Header (sticky navigation)
    ├── Hero section
    ├── Features section
    ├── Subjects section
    ├── Testimonials section
    ├── Contact section
    ├── Footer
    ├── Modal (contact form)
    └── <script> (JavaScript for modal functionality)
```

## 🛠️ Technologies Used

- **HTML5** - Semantic markup
- **CSS3** - Modern styling and animations
  - Flexbox
  - CSS Grid
  - Gradients
  - Transitions
  - Animations
  - Backdrop filters
- **JavaScript (Vanilla)** - Interactive contact form
  - No frameworks or libraries required
  - Pure ES6+ JavaScript

## 📱 Responsive Breakpoints

```css
/* Mobile devices */
@media (max-width: 480px) {
    /* Extra small screens */
}

/* Tablets */
@media (max-width: 768px) {
    /* Small to medium screens */
}

/* Desktop */
/* Default styles apply to screens larger than 768px */
```

## 🎯 SEO Optimization

The page includes:
- Semantic HTML5 elements
- Proper heading hierarchy (h1, h2, h3)
- Meta viewport tag for mobile
- Descriptive title tag
- Clean, accessible markup

**Recommended additions:**
```html
<!-- Add these to the <head> section for better SEO -->
<meta name="description" content="Expert Maths & Science tutoring in Cambridge. GCSE and A-Level tutoring with proven results. 95% of students achieve A*-B grades.">
<meta name="keywords" content="maths tutoring, science tutoring, Cambridge, GCSE, A-Level, physics, chemistry, biology">
<meta name="author" content="Kriya Tutorials">

<!-- Open Graph for social sharing -->
<meta property="og:title" content="Kriya Tutorials | Maths & Science Excellence">
<meta property="og:description" content="Expert tutoring in Cambridge for GCSE and A-Level students">
<meta property="og:type" content="website">
```

## 🔧 Troubleshooting

### Contact Form Not Working
- Check that the email address in the JavaScript is correct
- Ensure the user has a default email client set up
- Test in different browsers

### Styling Issues
- Clear browser cache
- Check if all styles are in the `<style>` tag
- Verify no ad blockers are interfering

### Mobile Display Problems
- Ensure viewport meta tag is present
- Test in actual devices, not just browser dev tools
- Check for any `overflow-x: hidden` conflicts

## 📝 License

This is a custom-built landing page. Feel free to use and modify it for your own projects.

## 👤 Contact

**Kriya Tutorials**
- 📧 Email: vikash.tigs@gmail.com
- 📱 Phone: +44 1223 123 456
- 📍 Location: Cambridge, UK

---

**Built with ❤️ for education**

*Last updated: February 2026*
