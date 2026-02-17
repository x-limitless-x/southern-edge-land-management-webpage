# 🌲 Southern Edge Land Management 🚜

> 🏆 **Professional Land Management & Landscaping Services**  
> Excellence in Every Project Since Day One

---

## 📖 About This Project

Welcome to the official website repository for **Southern Edge Land Management** - a family-owned business dedicated to providing exceptional land management and landscaping services in the Greater Charlotte Region. This website showcases our comprehensive services, from professional grading and land clearing to drainage solutions and tree removal.

### 🎯 Project Mission

Create a modern, engaging, and user-friendly web presence that:
- ✨ Highlights our professional services with clarity and visual appeal
- 📱 Provides seamless experience across all devices (mobile-first design)
- 🤝 Makes it easy for customers to contact us and request estimates
- ⭐ Showcases real customer testimonials and project transformations
- 🔍 Optimizes for search engines to reach more potential customers

---

## 🚀 Features

### 🎨 Modern Design
- **Logo-Driven Color Palette** - Consistent green (#2c5530), gold (#ffd700), and orange (#ff6b35) theming
- **Responsive Layout** - Optimized for desktop, tablet, and mobile devices
- **Engaging Animations** - Smooth transitions and hover effects
- **Professional Typography** - Montserrat and Open Sans font pairing

### 🛠️ Core Services Showcase
- 🏗️ **Professional Grading** - Precision land grading for optimal drainage
- 🌲 **Land Clearing** - Complete vegetation removal and site preparation
- 🚜 **Forestry Mulching** - Eco-friendly land clearing solutions
- 🔧 **Culvert Installation** - Expert water flow management
- 💧 **Drainage Solutions** - Custom drainage system design
- 🧱 **Retention Walls** - Durable erosion control structures
- 🛣️ **Driveway Services** - Quality driveway installation and repair
- 🌳 **Tree Removal** - Safe and efficient tree removal

### 📊 Technical Features
- ✅ **SEO Optimized** - Meta tags, structured data (JSON-LD), sitemap.xml
- 🔗 **Social Media Integration** - Open Graph and Twitter Card support
- 📘 **Facebook Reviews** - Dynamic review loading with fallback testimonials
- 📍 **LocalBusiness Schema** - Enhanced local search visibility
- 🤖 **robots.txt** - Proper search engine crawling configuration
- 🔒 **Privacy Compliant** - Privacy policy and data deletion pages

### 🎭 Interactive Elements
- 📞 Click-to-call phone numbers for instant contact
- ✉️ Click-to-email for direct communication
- 📘 Facebook page integration with review display
- 💬 Featured testimonials with rating stars
- 📸 Project gallery highlights

---

## 🖼️ Image Gallery

This website features a collection of professional project photos showcasing our work:

### 📂 Available Images (`/assets/page/`)
The repository includes 23 high-quality images of completed projects:
- **Retaining Walls** - Concrete terraced walls with professional finishes
- **Drainage Systems** - Stormwater management and channel installations
- **Grading Projects** - Hillside excavation and site preparation
- **Complete Transformations** - Before and after project results

### 🎨 Image Implementation
Images are organized by service type and can be used for:
- Hero section backgrounds
- Service-specific galleries
- Before/after comparisons
- Project portfolio showcases
- Quality detail highlights

---

## 🌐 Live Website

🔗 **Production URL:** [https://southernedgelm.com/](https://southernedgelm.com/)

📱 **Responsive Design** - Optimized viewing on all devices:
- 💻 Desktop (1200px+)
- 📱 Tablet (768px - 1199px)
- 📱 Mobile (< 768px)

---

## 🏗️ Technology Stack

### Frontend
- **HTML5** - Semantic markup with accessibility features
- **CSS3** - Modern styling with CSS variables and flexbox/grid
- **JavaScript (ES6+)** - Interactive features and dynamic content loading

### Design System
- **CSS Custom Properties** - Centralized theming via variables
- **Google Fonts** - Montserrat & Open Sans typography
- **Responsive Units** - Fluid sizing with rem/em units
- **Mobile-First** - Progressive enhancement approach

### SEO & Performance
- **Structured Data** - JSON-LD LocalBusiness schema
- **Meta Tags** - Open Graph, Twitter Cards, canonical URLs
- **Sitemap** - XML sitemap for search engines
- **Semantic HTML** - Proper heading hierarchy and ARIA labels

---

## 📦 Repository Structure

```
southern-edge-land-management-webpage/
├── index.html              # Main homepage
├── privacy-policy.html     # Privacy policy page
├── data-deletion.html      # Data deletion instructions
├── styles.css              # Main stylesheet
├── robots.txt              # Search engine directives
├── sitemap.xml             # Site structure for SEO
├── LICENSE                 # Project license
├── README.md               # This file
└── assets/
    ├── logo.png            # Company logo (PNG)
    ├── logo.ico            # Favicon
    └── page/               # Project photos (23 images)
        ├── IMG_2291.JPEG   # Retaining wall details
        ├── IMG_2295.JPEG   # Complete grading project
        ├── IMG_2304.JPEG   # Drainage channel system
        └── ... (20 more images)
```

---

## 🚀 Setup & Deployment

### Local Development

1. **Clone the Repository**
   ```bash
   git clone https://github.com/x-limitless-x/southern-edge-land-management-webpage.git
   cd southern-edge-land-management-webpage
   ```

2. **Open in Browser**
   ```bash
   # Simple HTTP server (Python 3)
   python -m http.server 8000
   
   # Or use any local server of your choice
   # Then visit: http://localhost:8000
   ```

3. **Make Changes**
   - Edit HTML files for content updates
   - Modify `styles.css` for design changes
   - Add images to `/assets/page/` directory
   - Test responsiveness across device sizes

### GitHub Pages Deployment

This site is deployed using GitHub Pages:

1. **Push to Main Branch**
   ```bash
   git add .
   git commit -m "Update website content"
   git push origin main
   ```

2. **GitHub Pages Settings**
   - Navigate to repository Settings → Pages
   - Source: Deploy from branch `main`
   - Root directory: `/` (root)
   - Site is automatically built and deployed

3. **Custom Domain** (Optional)
   - Add `CNAME` file with your domain
   - Configure DNS settings with your provider
   - Enable HTTPS in GitHub Pages settings

---

## 📘 Facebook Reviews Integration

### Current Setup
The website displays featured testimonials by default and can load live Facebook reviews when configured.

### Configuration Steps

1. **Update `facebookReviewsConfig` in `index.html`:**
   ```javascript
   const facebookReviewsConfig = {
       reviewsEndpoint: 'https://yourdomain.com/api/facebook-reviews',
       pageBaseUrl: 'https://www.facebook.com/YourPageName'
   };
   ```

2. **Backend Endpoint Requirements:**
   - Create a secure server-side endpoint
   - Proxy Facebook Graph API requests
   - Return reviews in expected format
   - Never expose access tokens to browser

3. **Expected Response Format:**
   ```json
   {
       "data": [
           {
               "review_text": "Amazing service!",
               "reviewer": { "name": "John Doe" },
               "rating": 5,
               "created_time": "2026-01-15T10:30:00+0000"
           }
       ]
   }
   ```

4. **Fallback Behavior:**
   - Without endpoint: Shows featured testimonials
   - With endpoint errors: Falls back to testimonials
   - No reviews available: Displays helpful message

---

## 🎨 Customization Guide

### Colors (CSS Variables)
Edit `:root` variables in `styles.css`:
```css
--color-primary: #2c5530;        /* Deep forest green */
--color-primary-light: #4a7c4e;  /* Lighter green */
--color-accent-gold: #ffd700;    /* Gold accent */
--color-accent-orange: #ff6b35;  /* Orange accent */
```

### Typography
```css
--font-primary: 'Montserrat', sans-serif;  /* Headings */
--font-secondary: 'Open Sans', sans-serif; /* Body text */
```

### Layout Breakpoints
```css
/* Mobile: Default (< 768px) */
/* Tablet: 768px - 1199px */
/* Desktop: 1200px+ */
```

---

## 📞 Contact Information

### Business Contact
- **Phone:** 📞 [704-866-1124](tel:704-866-1124)
- **Email:** ✉️ [dylanmumbulo@southernedgelm.com](mailto:dylanmumbulo@southernedgelm.com)
- **Hours:** ⏰ Monday - Saturday, 7:00 AM - 6:00 PM
- **Service Area:** 📍 Greater Charlotte Region

### Social Media
- **Facebook:** 📘 [Southern Edge Land Management](https://www.facebook.com/profile.php?id=61563383788006)

### Website
- **Production:** 🌐 [https://southernedgelm.com/](https://southernedgelm.com/)

---

## 🤝 Contributing

While this is a business website, suggestions for improvements are welcome!

### How to Contribute
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Test across devices and browsers
5. Submit a pull request with description

### Development Guidelines
- ✅ Maintain existing color scheme and branding
- ✅ Ensure mobile responsiveness
- ✅ Test across major browsers (Chrome, Firefox, Safari, Edge)
- ✅ Follow existing code formatting
- ✅ Optimize images before committing
- ✅ Update README if adding new features

---

## 📄 License

This project is proprietary and belongs to Southern Edge Land Management. All rights reserved.

See [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- **Family-Owned Business** - Built with pride by the Southern Edge team
- **Community Focused** - Serving the Greater Charlotte Region
- **Quality Commitment** - Excellence in every project since day one

---

## 📈 Roadmap

### ✅ Completed
- [x] Responsive website design
- [x] SEO optimization with structured data
- [x] Facebook reviews integration (frontend)
- [x] Contact forms and click-to-call
- [x] Privacy policy and data deletion pages
- [x] Custom domain setup (southernedgelm.com)
- [x] Project photo gallery with real images
- [x] Image lazy loading for performance

### 🎯 Planned Enhancements
- [ ] Backend API for live Facebook reviews
- [ ] Advanced image optimization (compression, WebP format)
- [ ] Photo gallery lightbox for full-screen viewing
- [ ] Before/after image comparisons
- [ ] Service area map integration
- [ ] Customer testimonial video embeds
- [ ] Online estimate request form
- [ ] Blog section for landscaping tips

---

## ⚡ Quick Links

- 🌐 [Live Website](https://southernedgelm.com/)
- 📘 [Facebook Page](https://www.facebook.com/profile.php?id=61563383788006)
- 📞 [Call Us: 704-866-1124](tel:704-866-1124)
- ✉️ [Email Us](mailto:dylanmumbulo@southernedgelm.com)

---

<div align="center">

### 🌲 Transform Your Property Into Something Extraordinary 🚜

**Southern Edge Land Management**  
*Your trusted partner for professional land management services*

[![Call Now](https://img.shields.io/badge/📞_Call_Now-704--866--1124-2c5530?style=for-the-badge)](tel:704-866-1124)
[![Visit Website](https://img.shields.io/badge/🌐_Visit_Website-southernedgelm.com-4a7c4e?style=for-the-badge)](https://southernedgelm.com/)
[![Facebook](https://img.shields.io/badge/📘_Facebook-Follow_Us-1877f2?style=for-the-badge)](https://www.facebook.com/profile.php?id=61563383788006)

---

*Built with ❤️ by Southern Edge Land Management*  
*© 2026 All Rights Reserved*

</div>
