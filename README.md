# lab5-css-foundations
**COMP 305 - Fall**

A modern, responsive login page featuring a two-column layout with CSS Grid, custom styling, and form validation.

## Live Demo
[View Live Site](https://chloeo-03.github.io/lab5-css-foundations/)

## Features

- **CSS Grid Layout**: Two-column responsive design (40% / 60% split)
- **Flexbox Alignment**: Centered content within sections
- **CSS Variables**: Centralized styling with custom properties
- **Form Validation**: Red border highlighting for invalid inputs
- **Hover Effects**: Smooth transitions on buttons and links
- **Responsive Design**: Mobile-friendly breakpoints
- **Custom Typography**: Comfortaa font from Google Fonts
- **Gradient Background**: Blue gradient on the branded section

## Technologies Used

- HTML5
- CSS3
- JavaScript (for form validation)
- Google Fonts (Comfortaa)

## CSS Techniques

- CSS Grid for two-column layout
- Flexbox for content alignment
- CSS custom properties (variables)
- Relative units (rem, em, vh)
- Media queries for responsive design
- Pseudo-classes (:hover, :focus, :active)
- CSS transitions and transforms

## Browser Compatibility

Tested on:
- Google Chrome
- Mozilla Firefox
- Safari

## Implementation Notes

### Design Decisions

- Used a 40/60 grid split to give more space to the form section
- Applied a blue gradient to the branded section for visual appeal
- Implemented red border validation for better user feedback
- Added smooth transitions for professional feel
- Used Comfortaa font for a modern, friendly appearance


### Challenges Encountered and Solutions

1. **Grid Layout Stacking Issue**: The two columns were stacking vertically instead of displaying side-by-side
   - **Problem**: Had a comma between grid column values: `grid-template-columns: 40%, 60%`
   - **Solution**: Removed the comma to use correct syntax: `grid-template-columns: 40% 60%`
   - **Learning**: CSS Grid column values should be space-separated, not comma-separated

2. **Missing Colon in :root**: CSS variables weren't working initially
   - **Problem**: Wrote `root {` instead of `:root {`
   - **Solution**: Added colon before `root` to properly define CSS custom properties
   - **Learning**: CSS pseudo-classes require a colon prefix

3. **Button Hover Not Working**: Hover state wasn't applying to the submit button
   - **Problem**: Had a space in the selector: `button [type="submit"]`
   - **Solution**: Removed space: `button[type="submit"]`
   - **Learning**: Attribute selectors must be attached directly to the element with no space

4. **Invalid Display Property**: Had `display: grid;` inside the `:root` block
   - **Problem**: Display properties don't belong in CSS variable declarations
   - **Solution**: Removed the invalid property from `:root` and placed grid on body element
   - **Learning**: `:root` is only for defining CSS custom properties (variables)

5. **Spacing Syntax Errors**: Multiple spacing issues with units
   - **Problem**: Had spaces between numbers and units: `1.25 rem`, `42 rem`
   - **Solution**: Removed spaces: `1.25rem`, `42rem`
   - **Learning**: CSS units must be written without spaces between value and unit

6. **Typo in Variable Names**: Some CSS variables had typos
   - **Problem**: `--front-weight-semibold` instead of `--font-weight-semibold`, `--text-placehodler` instead of `--text-placeholder`
   - **Solution**: Carefully checked and corrected all variable names
   - **Learning**: Variable typos cause properties to not apply; double-check spelling

7. **Focus Selector Spacing**: Input focus states weren't working
   - **Problem**: Had space before `:focus`: `input[type="email"] :focus`
   - **Solution**: Removed space: `input[type="email"]:focus`
   - **Learning**: Pseudo-class selectors must be attached directly without spaces

8. **Paragraph Line Breaks**: Text wasn't breaking at the correct points to match design
   - **Problem**: Natural text wrapping didn't match the reference image
   - **Solution**: Added `<br>` tags at specific points in the paragraph
   - **Learning**: Sometimes manual line breaks are needed to match specific designs


## Resources

- [CSS Grid Guide - CSS Tricks](https://css-tricks.com/snippets/css/complete-guide-grid/)
- [Flexbox Guide - CSS Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [CSS Custom Properties - MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties)
- [CSS Units - MDN](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Values_and_units)
- [Mozilla Developer Network (MDN)](https://developer.mozilla.org/)

## 📄 License
This project is licensed under the **MIT License** — see [LICENSE](LICENSE) for details.

## Author
Chloe Ogamba