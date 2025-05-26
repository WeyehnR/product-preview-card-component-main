# Product Preview Card Component

This is my take on the Product Preview Card challenge from Frontend Mentor. I wanted to build something that looks and feels just like the Figma mockups—fully responsive, accessible, and easy to maintain. Along the way, I learned a lot about real-world CSS, accessibility, and how to keep my codebase tidy for the future.

![Product Preview Card Screenshot](./design/desktop-preview.jpg)

## Features

- **Looks great everywhere:** The card adapts to mobile, tablet, and desktop. I used a mobile-first approach and CSS custom properties to make sure it scales smoothly.
- **Accessible for everyone:** Semantic HTML, keyboard navigation, and clear button states mean anyone can use it, whether they're on a phone, using a screen reader, or just tabbing through.
- **Design tokens:** Colors, spacing, and typography are all managed with CSS variables, so it's easy to tweak or theme.
- **Pixel-perfect:** I sweated the details to match the Figma design at every breakpoint.
- **Interactive:** The button responds to hover, active, and focus-visible states, so it feels right on any device.

## Try it on your phone!

Want to see it live on your device? Scan the QR code below:

![QR Code to open the site](./images/product_review_qr_code.png)

Or just visit: [https://weyehnr.github.io/product-preview-card-component-main/](https://weyehnr.github.io/product-preview-card-component-main/)

## Tech Stack

- HTML5
- CSS3 (Flexbox, Custom Properties, Media Queries)
- Google Fonts (Montserrat, Fraunces)

## Getting Started

1. **Clone the repo:**
   ```bash
   git clone https://github.com/your-username/product-preview-card.git
   cd product-preview-card
   ```
2. **Open `index.html` in your browser.**
   - No build tools or dependencies—just open and go!

## Project Structure

```
/
├── design/         # Design previews from Frontend Mentor
├── images/         # Project images, icons, and QR code
├── styles/         # CSS files (layout, components, typography, colors)
├── index.html      # Main HTML file
├── README.md       # Project documentation
└── style-guide.md  # Provided style guide
```

## Customization

- **Colors, spacing, and typography** are all in `styles/colors.css`, `styles/typography.css`, and `styles/layout.css`.
- **Breakpoints** are set in `styles/layout.css` for easy responsive tweaks.

## Accessibility

- Semantic HTML (`<main>`, `<article>`, `<button>`, etc.)
- Button is keyboard and screen reader accessible.
- Good color contrast and visible focus indicators.

## Credits

- Challenge by [Frontend Mentor](https://www.frontendmentor.io?ref=challenge)
- Coded by [Weyehn Reeves](#)

---

**Feel free to use, fork, or adapt this project for your own learning or portfolio!**

---

## Reflection

### What I'm Most Proud Of

- **Nailing the Responsive, Pixel-Perfect Design:**  
  I made sure the card looks just like the Figma mockups—no matter what device you're on. It's fully responsive and pixel-perfect, just the way it's meant to be.

- **Building for Everyone:**  
  Accessibility wasn't an afterthought. I wanted anyone to be able to use this card, whether they're using a keyboard, a screen reader, or just tapping on their phone.

- **Organizing CSS for Real-World Projects:**  
  I used design tokens and kept my CSS organized and tidy, always thinking about how I (or someone else) might want to update or expand the project in the future.

- **Learning from Real CSS Challenges:**  
  I definitely wrestled with the quirks of CSS cascade and specificity. There were moments of frustration, but I stuck with it, debugged, and learned a ton about how CSS really works in a real project.

### What I'd Do Differently Next Time
- Start with a mobile-first approach from the beginning.
- Maybe use a CSS preprocessor or utility framework for bigger projects.
- Add automated accessibility and visual regression testing.
- Break the UI into reusable components if using a JS framework.
- Further optimize images and add more documentation.

## Challenges Encountered & How I Overcame Them

### 1. CSS Cascade and Specificity Issues
**Challenge:** The mobile layout wasn't activating as expected; the card stayed in a horizontal (desktop) layout even on small screens.

**How I Overcame It:** I realized my component styles were overriding my layout styles. By moving all layout/responsive rules to `layout.css` and keeping only visual styles in `components.css`, I got the mobile-first, responsive behavior working as intended.

---

### 2. Responsive Breakpoints for Real Devices
**Challenge:** My first mobile media query was too narrow (400px), so the mobile layout didn't activate on many real devices.

**How I Overcame It:** I researched common device widths and expanded my breakpoints to cover a wider range, so the mobile layout now works on all popular phones and tablets.

---

### 3. Maintaining Consistent Units
**Challenge:** I started with a mix of `px` and `rem` units, which made things inconsistent and harder to scale.

**How I Overcame It:** I refactored everything to use `rem` units, making the design more scalable and accessible.

---

### 4. Ensuring Button Interactivity Across Devices
**Challenge:** CSS `:hover` doesn't work on touch devices, so the button's feedback was missing on mobile and tablet.

**How I Overcame It:** I added `:active` and `:focus-visible` states to the button, so users on any device (mouse, touch, keyboard) get consistent feedback.

---

### 5. Debugging and Iterative Testing
**Challenge:** Sometimes styles just wouldn't apply as expected, especially with overlapping CSS files and media queries.

**How I Overcame It:** I used browser DevTools a lot, tested with different device presets, and kept refining my CSS structure. I also reviewed the full CSS files to spot and fix conflicts.

---

### 6. Following Figma Specs Closely
**Challenge:** Translating Figma's exact spacing, sizing, and color tokens into maintainable CSS took a lot of attention to detail and a few iterations.

**How I Overcame It:** I used CSS custom properties (design tokens) and double-checked all values against the Figma specs to get a pixel-perfect result.


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
