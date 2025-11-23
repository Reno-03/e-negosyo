# 🛒 eNegosyo - Filipino Snack Store

A fully responsive e-commerce website for Filipino snacks and junk food, built with pure HTML5 and CSS3. Features mobile-first design with CSS Grid layout and three responsive breakpoints.

## 🎯 Project Overview

eNegosyo is a mock online store showcasing popular Filipino snacks like Oishi, Piattos, Chippy, and more. This project represents the culmination of my HTML/CSS fundamentals learning journey, demonstrating responsive design principles and modern layout techniques.

## ✨ Features

- **Mobile-First Responsive Design**: Optimized for mobile, tablet, and desktop screens
- **CSS Grid Layout**: Advanced grid system that adapts across 3 breakpoints (768px, 1024px, 1400px)
- **Custom CSS Variables**: Maintainable color scheme using `:root` properties
- **Interactive Elements**: 
  - Hover effects on navigation, products, and buttons
  - Smooth transitions and transform animations
  - Social media contact buttons
- **Complete E-commerce Layout**:
  - Product catalog with 6 Filipino snack items
  - Category filter sidebar
  - Order form with validation
  - About Us section
  - Contact footer with social links
- **Semantic HTML5**: Proper use of header, nav, main, section, footer tags
- **Form Elements**: Text inputs, email validation, dropdown selects, radio buttons

## 🛠️ Technologies Used

- **HTML5**: Semantic markup, forms, and accessibility features
- **CSS3**: Grid, Flexbox, custom properties, media queries, transitions
- **FontAwesome SVG Icons**: Social media and UI icons

## 📚 What I Learned

This capstone project helped me master:

1. **CSS Grid**: Complex multi-area layouts with `grid-template-areas`
2. **Mobile-First Approach**: Building from mobile up with progressive enhancement
3. **Responsive Design**: Three breakpoints for mobile → tablet → desktop
4. **CSS Custom Properties**: Using `:root` variables for consistent theming
5. **Form Styling**: Custom inputs, selects, radio buttons with validation
6. **Layout Composition**: Combining Grid and Flexbox appropriately
7. **Box Model Mastery**: Consistent spacing with padding, margins, and gaps
8. **Hover States**: Interactive feedback with `filter`, `transform`, and transitions

## 🎨 Design Details

### Color Scheme
```css
--primary: #fa9600   /* Orange - CTAs and buttons */
--secondary: #fa6000 /* Darker orange - accents */
--dark: #6b4203      /* Brown - header and text */
--light: #fff9ef     /* Cream - background */
```

### Responsive Breakpoints
- **Mobile**: < 768px (single column, stacked layout)
- **Tablet**: 768px - 1024px (horizontal navigation)
- **Desktop**: 1024px+ (2-column grid with sidebar)
- **Large Desktop**: 1400px+ (3-column grid with both sidebars)

### Layout Grid Areas
```
Mobile:           Tablet/Desktop (1024px+):      Large (1400px+):
┌─────────┐      ┌─────────┬─────────┐          ┌─────┬─────┬─────┐
│ header  │      │  header  header  │          │  header header header │
├─────────┤      ├─────────┴─────────┤          ├─────┼─────┼─────┤
│ sidebar │      │  left-sidebar     │          │ left│prod │order│
├─────────┤      ├─────────┬─────────┤          │ side│list │side │
│products │      │products │ order   │          │ bar │     │ bar │
├─────────┤      │         │ sidebar │          ├─────┴─────┴─────┤
│ order   │      ├─────────┴─────────┤          │  footer footer footer │
├─────────┤      │  footer  footer  │          └─────────────────┘
│ footer  │      └─────────┴─────────┘
└─────────┘
```

## 🚀 How to View

Simply open `index.html` in your browser. No dependencies or build process required!

## 📂 Project Structure
```
enegosyo-website/
├── index.html              # Main HTML structure
├── style.css               # All styling and responsive design
├── assets/                 # Product images
│   ├── oishi-prawn-crackers-spicy.png
│   ├── piattos-cheese.png
│   ├── chippy-barbeque.jpg
│   ├── nova-multigrain.jpg
│   ├── presto-creams-peanut-butter.png
│   └── skyflakes-crackers.jpg
├── screenshots/
│   └── live.png           # Project preview
└── README.md              # Project documentation
```

## 🌐 Live Demo & Preview

**[👉 View Live Project](https://your-username.github.io/enegosyo-website/)**

![eNegosyo Website Preview](screenshots/live.png)
*Fully responsive Filipino snack e-commerce site with mobile-first design*

## 💡 Key Implementation Highlights

### Mobile-First CSS Grid
```css
/* Mobile (default) */
.grid-container {
  display: grid;
  grid-template-areas:
    'header'
    'left-sidebar'
    'product-listing'
    'place-order-sidebar'
    'footer';
}

/* Desktop (1400px+) */
@media (min-width: 1400px) {
  .grid-container {
    grid-template-columns: 1fr 2fr 1fr;
    grid-template-areas:
      "header header header"
      "left-sidebar product-listing place-order-sidebar"
      "footer footer footer";
  }
}
```

### Responsive Product Grid
```css
.product-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmin(280px, 1fr));
  gap: 30px;
}
```

## 🎓 Learning Context

This project was built as a **challenge project** after completing the first three modules of SoloLearn's Introduction to HTML course. It demonstrates:
- Solid understanding of HTML fundamentals
- CSS layout techniques (Grid + Flexbox)
- Responsive design principles
- Form handling and validation
- Modern web design patterns

## 📱 Responsive Features

- **Navigation**: Vertical stack (mobile) → Horizontal menu (tablet+)
- **Product Grid**: Single column → 2 columns → 3 columns (auto-fit)
- **Sidebars**: Stacked (mobile) → Side-by-side (desktop)
- **Forms**: Full-width (mobile) → Constrained sidebar (desktop)

## 🔮 Future Enhancements

- Add JavaScript for:
  - Functional cart system
  - Form validation feedback
  - Category filtering
  - Product search
- Implement backend/database integration
- Add product detail pages
- Create user authentication
- Shopping cart and checkout flow

## 👨‍💻 About

Created as the capstone project for my HTML/CSS learning journey. This represents my progression from basic CSS concepts to building a complete, responsive website from scratch using modern layout techniques.

**Timeline**: Completed CSS styling in one day after planning the HTML structure.

---

**Note**: This is a practice/educational project. Product images and branding are used for demonstration purposes only.