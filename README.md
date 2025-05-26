# Product Preview Card Component

A responsive product preview card built as a Frontend Mentor challenge. This project demonstrates modern HTML5, CSS3 (with custom properties), and accessibility best practices. The card is fully responsive, adapting seamlessly to mobile, tablet, and desktop devices.

![Product Preview Card Screenshot](./design/desktop-preview.jpg)

## Features

- **Responsive Design:** Adapts layout for mobile, tablet, and desktop using a mobile-first approach and CSS custom properties.
- **Accessible:** Semantic HTML, keyboard navigable, and accessible button states for all users.
- **Design Tokens:** Uses CSS variables for colors, spacing, and typography for easy theming and maintainability.
- **Pixel-Perfect:** Matches the provided Figma design specs for all breakpoints.
- **Interactive:** Button includes hover, active, and focus-visible states for a consistent experience across devices.

## Try it on your phone!

Scan the QR code below to open this project on your mobile device:

![QR Code to open the site](./images/product_review_qr_code.png)

Or visit: [https://weyehnr.github.io/product-preview-card-component-main/](https://weyehnr.github.io/product-preview-card-component-main/)

## Technologies Used

- HTML5
- CSS3 (Flexbox, Custom Properties, Media Queries)
- Google Fonts (Montserrat, Fraunces)

## Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/product-preview-card.git
   cd product-preview-card
   ```

2. **Open `index.html` in your browser.**
   - No build tools or dependencies required.

## Folder Structure

```
/
├── design/         # Design previews from Frontend Mentor
├── images/         # Project images and icons
├── styles/         # CSS files (layout, components, typography, colors)
├── index.html      # Main HTML file
├── README.md       # Project documentation
└── style-guide.md  # Provided style guide
```

## Customization

- **Colors, spacing, and typography** can be easily adjusted in the `styles/colors.css`, `styles/typography.css`, and `styles/layout.css` files.
- **Breakpoints** are defined in `styles/layout.css` for easy responsive adjustments.

## Accessibility

- Uses semantic HTML elements (`<main>`, `<article>`, `<button>`, etc.)
- Button is accessible via keyboard and screen readers.
- Sufficient color contrast and focus indicators.

## Credits

- Challenge by [Frontend Mentor](https://www.frontendmentor.io?ref=challenge)
- Coded by [Weyehn Reeves](#)

---

**Feel free to use, fork, or adapt this project for your own learning or portfolio!**

---

## Reflection

### What I'm Most Proud Of
- Achieving a fully responsive, pixel-perfect design that matches the Figma specs.
- Ensuring accessibility and keyboard navigation for all users.
- Structuring CSS for maintainability and scalability using design tokens and separation of concerns.
- Debugging and learning from real-world CSS cascade and specificity issues.

### What I'd Do Differently Next Time
- Start with a mobile-first approach from the beginning.
- Consider using a CSS preprocessor or utility framework for larger projects.
- Add automated accessibility and visual regression testing.
- Break the UI into reusable components if using a JS framework.
- Further optimize assets and add more documentation.

## Challenges Encountered & How I Overcame Them

### 1. CSS Cascade and Specificity Issues
**Challenge:** The mobile layout wasn't activating as expected; the card remained in a horizontal (desktop) layout even on small screens.

**How I Overcame It:** By separating layout/responsive styles into `layout.css` and keeping only visual styles in `components.css`, I restored the intended mobile-first, responsive behavior.

---

### 2. Responsive Breakpoints for Real Devices
**Challenge:** The initial mobile media query breakpoint was too narrow (400px), so the mobile layout didn't activate on many real devices.

**How I Overcame It:** I expanded the breakpoints to cover a wider range of devices, ensuring the mobile layout would activate for all popular phones and tablets.

---

### 3. Maintaining Consistent Units
**Challenge:** The project started with a mix of `px` and `rem` units, which could lead to inconsistent scaling and maintainability issues.

**How I Overcame It:** I refactored all fixed pixel values to use `rem` units, making the design more scalable, accessible, and consistent across devices.

---

### 4. Ensuring Button Interactivity Across Devices
**Challenge:** CSS `:hover` states don't work on touch devices, so the button's interactive feedback was missing on mobile and tablet.

**How I Overcame It:** I added `:active` and `:focus-visible` states to the button, ensuring that users on all devices (mouse, touch, keyboard) get consistent interactive feedback.

---

### 5. Debugging and Iterative Testing
**Challenge:** It was sometimes unclear why a style wasn't applying as expected, especially with overlapping CSS files and media queries.

**How I Overcame It:** I used browser DevTools extensively, tested with multiple device presets, and iteratively refined the CSS structure. I also asked for and reviewed the full CSS files to spot and resolve conflicts.

---

### 6. Following Figma Specs Closely
**Challenge:** Translating Figma's exact spacing, sizing, and color tokens into maintainable CSS required attention to detail and sometimes multiple iterations.

**How I Overcame It:** I used CSS custom properties (design tokens) and double-checked all values against the Figma specs, ensuring pixel-perfect implementation.


## Questions & Feedback

I'm looking for feedback on the following areas:

- Responsive layout: Does the card look and function well on all devices? Any edge cases?
- Accessibility: Any issues for screen readers, keyboard users, or color contrast?
- CSS architecture: Is my separation of layout and component styles clear? Are my design tokens effective?
- Code quality: Any redundant code or ways to simplify?
- Performance: Any optimizations for images or CSS?
- Interactivity: Is the button feedback clear and consistent?
- General: Any modern techniques or best practices I could apply?

**Please be as specific as possible—your input will help me improve!**
