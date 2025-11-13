# Private Mathematics Tutoring 📚

A modern, responsive website for private mathematics tutoring services in Kaluđerica, Belgrade, Serbia.

## 🎯 Project Overview

This is a beautiful, SEO-optimized website built with **Astro** for offering private mathematics tutoring to students in grades 1-8. The site features:

- **Hero Section** - Eye-catching introduction with call-to-action buttons
- **About Section** - Information about the instructor's qualifications and approach
- **Benefits Section** - Why private tutoring works
- **Services Section** - What students receive
- **Contact Section** - Multiple ways to get in touch
- **Responsive Design** - Works perfectly on desktop, tablet, and mobile devices

## 🛠️ Tech Stack

- **[Astro](https://astro.build/)** - Static site generator for fast, component-based web development
- **HTML5** - Semantic markup
- **CSS3** - Modern styling with custom properties and grid/flexbox layouts
- **No JavaScript frameworks** - Pure semantic HTML with minimal JavaScript

## 📁 Project Structure

```
src/
├── components/
│   ├── Hero.astro              # Hero section with main CTA
│   ├── About.astro             # Instructor information
│   ├── WhyPrivate.astro        # Benefits of private tutoring
│   ├── Benefits.astro          # Services and offerings
│   └── Contact.astro           # Contact form and footer
├── layouts/
│   └── Layout.astro            # Main layout with metadata
├── pages/
│   └── index.astro             # Home page (main entry point)
├── styles/
│   └── global.css              # Global styles and utilities
└── assets/                     # Images and other static assets
```

## 🚀 Getting Started

### Prerequisites

- **Node.js** 18.17.1 or higher
- **npm** or **pnpm** (pnpm recommended)

### Installation

1. Clone the repository:

```bash
git clone <repository-url>
cd math-class-private
```

2. Install dependencies:

```bash
pnpm install
```

Or with npm:

```bash
npm install
```

### Development

Start the development server:

```bash
pnpm dev
```

The site will be available at `http://localhost:3000` by default.

### Build

Create a production build:

```bash
pnpm build
```

### Preview

Preview the production build locally:

```bash
pnpm preview
```

## 🎨 Customization Guide

### Update Contact Information

Edit `/src/components/Contact.astro`:

- **Phone Number** (Line 28):

  ```html
  <a href="tel:+381000000000" class="contact-link">+381 00 000 0000</a>
  ```

- **Email Address** (Line 38):

  ```html
  <a href="mailto:primer@email.com" class="contact-link">primer@email.com</a>
  ```

- **Instagram Handle** (Line 48):

  ```html
  <a
    href="https://instagram.com/tvoj_profil"
    target="_blank"
    class="contact-link"
    >@tvoj_profil</a
  >
  ```

- **Footer Contact Info** (Lines 177-181):

  ```html
  <p>📞 +381 00 000 0000</p>
  <p>📧 primer@email.com</p>
  <p>📍 Kaluđerica, Beograd</p>
  ```

- **Working Hours** (Lines 184-187):
  ```html
  <p>Ponedeljak - Petak: 15:00 - 20:00</p>
  <p>Subota: 10:00 - 18:00</p>
  <p>Nedelja: Po dogovoru</p>
  ```

### Customize Colors

The site uses a professional teal and yellow color scheme. Edit `/src/styles/global.css` to customize:

- **Primary Colors**:

  - Teal: `#62b8a6` and `#34645a`
  - Yellow Accent: `#ffde59`

- **Text Colors**:
  - Dark Text: `#354d48`
  - Light Gray: `#666`

### Add Logo or Images

Place images in `/public/` directory and reference them in components:

```html
<img src="/your-image.png" alt="Description" />
```

### Update Site Metadata

Edit the title and description in `/src/pages/index.astro`:

```javascript
const siteTitle = "Your Custom Title";
const siteDescription = "Your custom description";
```

Also update the Layout metadata in `/src/layouts/Layout.astro` for SEO.

## 📱 Key Features

### Responsive Design

- Mobile-first approach
- Optimized for all screen sizes
- Touch-friendly interactive elements

### Performance

- Zero JavaScript by default
- Fast page loads
- Optimized images
- Static site generation

### SEO Optimized

- Semantic HTML5
- Meta tags for search engines
- Open Graph tags for social media
- Serbian language support (`lang="sr"`)

### Accessibility

- Semantic HTML structure
- Good color contrast
- Keyboard navigation support
- ARIA labels where needed

## 🎨 Component Overview

### Hero Component

- Large heading with badge
- Bulleted benefits list
- CTA buttons
- Floating decorative elements
- Instructor card with stats

### About Component

- Four cards highlighting qualifications:
  - Education (Master's degree)
  - Passion for mathematics
  - Teaching approach
  - Goals

### WhyPrivate Component

- Six reasons for private tutoring
- Highlight section with key results
- Number badges for visual interest

### Benefits Component

- Free trial lesson offer
- Referral discount program
- Checklist of included services

### Contact Component

- Highlight section emphasizing free trial
- Four contact methods:
  - Phone/SMS
  - Email
  - Instagram DM
  - Location
- Contact form with fields:
  - Parent name
  - Student name
  - Grade level (1-8)
  - Phone number
  - Email
  - Message
- Footer with business information

## 📧 Contact Form Integration

The contact form in `/src/components/Contact.astro` currently submits to a placeholder. To enable form submissions, you'll need to:

1. Add a form backend service like:

   - [Formspree](https://formspree.io/)
   - [Netlify Forms](https://www.netlify.com/products/forms/)
   - [EmailJS](https://www.emailjs.com/)

2. Update the form `action` attribute:
   ```html
   <form
     class="contact-form"
     action="https://formspree.io/f/YOUR_FORM_ID"
     method="POST"
   ></form>
   ```

## 🌐 Deployment

### Deploy to Netlify

1. Push code to GitHub
2. Connect your repository to Netlify
3. Set build command: `npm run build`
4. Set publish directory: `dist/`
5. Deploy!

### Deploy to Vercel

1. Connect your GitHub repository to Vercel
2. Vercel auto-detects Astro projects
3. Deploy with zero configuration

### Deploy Anywhere

Since Astro generates static HTML, you can deploy to:

- AWS S3 + CloudFront
- GitHub Pages
- Firebase Hosting
- Traditional web hosting

## 📄 License

This project is provided as-is for educational and business purposes.

## 🤝 Contributing

Feel free to customize this template for your needs. Some ideas:

- Add student testimonials section
- Integrate with scheduling system (Calendly, etc.)
- Add pricing information
- Create blog for math tips
- Add photo gallery

## 📚 Resources

- [Astro Documentation](https://docs.astro.build)
- [Astro Components Guide](https://docs.astro.build/en/basics/components/)
- [CSS Tips for Astro](https://docs.astro.build/en/guides/styling/)

## ✨ Features Coming Soon

- [ ] Online booking calendar integration
- [ ] Student testimonials carousel
- [ ] Blog for math learning tips
- [ ] Photo gallery
- [ ] Email notification system

---

**Last Updated:** November 2025

Made with ❤️ for mathematics education
