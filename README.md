# Yuvaguru - Personal Portfolio Website

A fully accessible, semantic HTML5 portfolio website demonstrating professional web development practices with a focus on accessibility and responsive design.

## 📋 Project Overview

This project is a multi-page personal portfolio website built as part of the **Thiranex Internship Program** (HTML5 Semantic Structure & Accessibility certification). The portfolio showcases a commitment to building web experiences that are accessible to everyone, regardless of ability or device.

The website has been audited and designed to meet **WCAG 2.1 Level AA accessibility guidelines** and implements modern HTML5 semantic standards with responsive CSS3 styling.

---

## 🎯 Purpose

This project demonstrates:
- Proper use of semantic HTML5 elements for meaningful document structure
- Comprehensive accessibility implementation following WCAG guidelines
- Keyboard navigation and screen reader compatibility
- Responsive design that works seamlessly across all devices
- SEO best practices through semantic markup and meta tags
- Professional front-end development standards

---

## 📄 Pages & Features

### **Home (index.html)**
- Hero section with clear call-to-action
- Skills showcase with responsive card grid layout
- Professional introduction and value proposition

### **About (about.html)**
- Personal background and professional goals
- Key strengths highlighted in an organized list
- Clear learning objectives and career direction

### **Projects (projects.html)**
- Responsive project portfolio grid
- Individual project cards with descriptions and technology tags
- Links to project demonstrations

### **Contact (contact.html)**
- Fully accessible contact form with semantic HTML structure
- HTML5 form validation for required fields
- Form fields: Name, Email, Topic (dropdown), and Message
- Keyboard-navigable fieldset with legend grouping
- Help text for form navigation guidance

---

## 🛠 Technologies Used

| Technology | Version | Purpose |
|-----------|---------|---------|
| **HTML5** | Living Standard | Semantic document structure |
| **CSS3** | Latest | Responsive styling and layout |
| **Flexbox** | CSS3 | Navigation and component layouts |
| **CSS Grid** | CSS3 | Multi-column card grids |
| **CSS Custom Properties** | CSS3 | Design system variables and theming |

---

## ♿ Accessibility Features

### Semantic HTML5 Elements
- `<header>`, `<nav>`, `<main>`, `<article>`, `<section>`, `<footer>` for meaningful document structure
- `<fieldset>` and `<legend>` for form organization
- Proper heading hierarchy (h1 → h2) throughout all pages
- List elements (`<ul>`, `<li>`) for all list content

### ARIA Implementation
- **aria-label**: Descriptive labels on navigation links and brand
- **aria-labelledby**: Section headings linked to content regions
- **aria-current="page"**: Active navigation indicator
- **aria-required="true"**: Required form field indication
- **aria-describedby**: Form help text linked to form element
- **aria-hidden="true"**: Visual-only content hidden from screen readers

### Keyboard Navigation
- **Tab key**: Full keyboard navigation through all interactive elements
- **Focus management**: Clear visual focus indicators with 3px amber outline
- **Skip-to-content link**: Allows keyboard users to bypass navigation and jump directly to main content
- **Logical tab order**: Navigation → Main Content → Footer
- **Form navigation**: All form inputs tab-accessible with proper focus styles

### Screen Reader Support
- Semantic elements provide structure and landmarks
- Form labels properly associated with inputs via `for` attribute
- Help text and descriptions available to screen readers
- Meaningful button and link text
- Aria-hidden properly masks decorative elements

### Form Accessibility
- **Grouped form controls** using `<fieldset>` and `<legend>`
- **Linked labels**: Each input has a `<label>` with proper `for` attribute
- **HTML5 validation**: Required attributes and email type validation
- **Autocomplete support**: Name and email fields include `autocomplete` attributes
- **Visual indicators**: Required fields marked with asterisks and aria-required
- **Focus visible**: All form inputs have clear focus outlines
- **Error-friendly structure**: Browser's native validation messages displayed

---

## 🔍 SEO Features

- **Meta tags**: Description, robots, and author meta tags on all pages
- **Semantic markup**: Proper heading hierarchy and structural elements
- **Responsive viewport**: Mobile viewport meta tag for proper rendering
- **Accessible URLs**: Clean, descriptive file names and navigation structure
- **Content organization**: Logical structure improves both user experience and search indexability

---

## 📱 Responsive Design

### Breakpoints
- **Mobile-first approach**: Base styles optimized for mobile (< 40rem / 640px)
- **Tablet & Desktop**: Flexible layouts scale up to 68rem (1088px) max-width

### Layout Changes at Mobile Breakpoint
- **Navigation**: Stacks vertically on small screens
- **Card grids**: 3-column layout on desktop → 1-column on mobile
- **Spacing**: Adjusted padding and margins for smaller screens
- **Typography**: Fluid font sizing using CSS `clamp()` function

### CSS Techniques
- **Flexbox**: Header navigation and content alignment
- **CSS Grid**: Multi-column project cards and skills showcase
- **CSS Custom Properties**: Centralized color and spacing values
- **min() function**: Responsive container widths
- **clamp() function**: Fluid typography scaling

---

## 📁 Project Folder Structure

```
portfolio-project/
├── index.html              # Home page
├── about.html              # About the developer
├── projects.html           # Project showcase
├── contact.html            # Contact form
├── css/
│   └── styles.css          # All styling and responsive design
└── README.md               # This file
```

---

## 🚀 How to Run the Project Locally

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- No build tools or server required

### Steps

1. **Download or clone the project**
   ```bash
   git clone <repository-url>
   cd portfolio-project
   ```

2. **Open in your browser**
   - **Option A**: Double-click `index.html` to open directly
   - **Option B**: Use a local server (recommended for best results)
     ```bash
     # Using Python 3
     python -m http.server 8000
     
     # Or using Node.js (http-server)
     npx http-server
     ```
   - **Option C**: Use Live Server extension in VS Code

3. **View the website**
   - Open `http://localhost:8000` (or the port shown in your terminal)
   - Navigate through all pages using the top navigation menu

### Testing Accessibility

- **Keyboard navigation**: Use the `Tab` key to navigate through all interactive elements
- **Skip link**: Press `Tab` once at page load to see the skip-to-main-content link
- **Screen reader testing**: 
  - Windows: NVDA (free) or JAWS
  - macOS: VoiceOver (built-in, activate with Cmd + F5)
  - Browser: Axe DevTools, WAVE browser extensions
- **Color contrast**: Test with WebAIM or Color Oracle tools
- **Responsive testing**: Use browser DevTools (F12) to test various device sizes

---

## 🎨 Design System

### Color Palette
- **Navy** (#102a43): Primary text and headings
- **Blue** (#0b5cab): Links and interactive elements
- **Text** (#1f2933): Body text
- **Muted** (#52606d): Secondary text and captions
- **Surface** (#ffffff): Card and container backgrounds
- **Border** (#9fb3c8): Subtle borders and dividers
- **Focus** (#f59e0b): Amber outline for keyboard focus (WCAG AAA compliant)

### Typography
- **Font family**: Arial, sans-serif (accessible and widely supported)
- **Base size**: 1rem (16px)
- **Line height**: 1.6 (improved readability)
- **Heading hierarchy**: Proper size scaling from h1 to h2

### Spacing & Layout
- **Container max-width**: 68rem (1088px)
- **Container padding**: 92% width with auto margins
- **Gap/spacing**: Consistent 1rem baseline with multiples
- **Border radius**: Subtle 0.25rem to 0.5rem on elements

---

## ✅ Quality Standards

### Accessibility Compliance
- ✅ WCAG 2.1 Level AA guidelines
- ✅ Semantic HTML5 structure
- ✅ ARIA landmarks and labels
- ✅ Keyboard navigation
- ✅ Screen reader compatible
- ✅ Color contrast ratios (AAA standard for focus indicators)

### Performance
- Minified CSS for optimal file size
- No external dependencies or third-party scripts
- Fast load times on all connection speeds
- Mobile-optimized performance

### Cross-Browser Compatibility
- ✅ Chrome/Chromium-based browsers
- ✅ Firefox
- ✅ Safari (macOS and iOS)
- ✅ Edge
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

---

## 📚 Learning Outcomes

This project demonstrates mastery of:
- Semantic HTML5 for meaningful document structure
- WCAG 2.1 accessibility guidelines implementation
- CSS3 responsive design patterns
- Form accessibility and validation
- Keyboard navigation and focus management
- Professional GitHub-ready project organization

---

## 🔗 Resources & References

- [MDN Web Docs - Semantic HTML](https://developer.mozilla.org/en-US/docs/Glossary/Semantic_HTML)
- [WCAG 2.1 Guidelines](https://www.w3.org/WAI/WCAG21/quickref/)
- [Web Accessibility by WAI](https://www.w3.org/WAI/)
- [CSS Tricks - Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [CSS Tricks - Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)
- [Accessible Forms Guide](https://www.w3.org/WAI/tutorials/forms/)

---

## 📄 License

This project was created as part of the Thiranex Internship Program.

---

## ✨ Project Highlights

| Feature | Status |
|---------|--------|
| Semantic HTML5 | ✅ Fully Implemented |
| WCAG Accessibility | ✅ Level AA Compliant |
| Responsive Design | ✅ Mobile, Tablet, Desktop |
| Keyboard Navigation | ✅ Fully Supported |
| Screen Reader Support | ✅ Optimized |
| SEO Optimization | ✅ Implemented |
| Form Validation | ✅ HTML5 Native |
| Focus Management | ✅ Clear Visual Indicators |
| Cross-Browser Support | ✅ Tested |

---

**Built with semantic HTML5 and modern CSS3** | **Designed for accessibility first** | **Mobile-responsive** | **Thiranex Internship 2026**
