# CSS Modern Skill

## 🎯 Purpose

A comprehensive CSS reference and guidance skill based on the CSS Pocket
Reference (5th Edition, Eric A. Meyer) and modern CSS specifications. Provides
accurate, up-to-date information on selectors, properties, layout systems, and
best practices.

## 📚 Knowledge Base

- CSS Pocket Reference, 5th Edition (O'Reilly, 2018)
- CSS Selectors Level 3 & 4
- CSS Flexible Box Layout Module Level 1
- CSS Grid Layout Module Level 1
- CSS Cascading and Inheritance Level 4
- Modern CSS features: Container Queries, Cascade Layers, Color Level 4/5

## ✨ Capabilities

### Selector Reference

- Universal, type, class, ID, and attribute selectors
- Combinators: descendant (space), child (`>`), adjacent sibling (`+`), general sibling (`~`)
- Structural pseudo-classes: `:nth-child()`, `:first-of-type`, `:empty`, etc.
- Interaction pseudo-classes: `:hover`, `:focus`, `:active`, `:checked`
- Pseudo-elements: `::before`, `::after`, `::first-letter`, `::first-line`

### Property Reference

- Complete alphabetical reference for CSS3 properties
- Inheritance and animation metadata for each property
- Value syntax conventions and accepted value types
- Initial values, computed values, and applicability

### Layout Systems

- **Flexbox**: `flex`, `flex-direction`, `justify-content`, `align-items`, etc.
- **Grid**: `grid-template-areas`, `grid-column`, `grid-row`, `gap`, etc.
- **Box Model**: `margin`, `padding`, `border`, `box-sizing`
- **Positioning**: `static`, `relative`, `absolute`, `fixed`, `sticky`

### Modern CSS Features

- Cascade Layers (`@layer`) for style precedence control
- Container Queries (`@container`) for component-level responsiveness
- Modern color syntax: `oklch()`, `color-mix()`, relative colors
- Logical properties: `margin-inline`, `padding-block`, etc.
- Subgrid and masonry layout patterns

### Media & Feature Queries

- Responsive design with `@media` queries
- Feature detection with `@supports`
- Dynamic viewport units: `svh`, `dvh`, `lvh`

## 💡 Usage Guidelines

### When to Use This Skill

- Looking up CSS property syntax, values, or browser support
- Understanding selector specificity and cascade resolution
- Implementing modern layout patterns (Flexbox/Grid)
- Debugging CSS precedence or inheritance issues
- Writing accessible, maintainable CSS

### Response Format

1. **Direct Answer**: Provide the specific property/selector information requested
2. **Syntax Example**: Show valid CSS syntax with explanation
3. **Browser Support**: Note any compatibility considerations when relevant
4. **Best Practice**: Suggest modern, accessible approaches
5. **Related Properties**: Link to complementary properties when helpful

### Example Interaction

**User**: "How do I center a div vertically and horizontally?"

**Response**:

```css
/* Modern approach using Flexbox */
.container {
  display: flex;
  justify-content: center;  /* horizontal */
  align-items: center;      /* vertical */
}

/* Alternative: Grid */
.container {
  display: grid;
  place-items: center;  /* shorthand for both axes */
}

/* Legacy fallback: absolute positioning */
.child {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
