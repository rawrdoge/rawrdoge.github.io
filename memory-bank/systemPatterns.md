# System Patterns

## Design Language: Glassmorphism

### Core Pattern
- **Frosted Glass Effect**: `backdrop-filter: blur(12px)` with `-webkit-` prefix
- **Transparency**: `background: rgba(255, 255, 255, 0.08)`
- **Border**: `1px solid rgba(255, 255, 255, 0.18)`
- **Shadow**: `box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37)`

### Gradient System
```css
/* Firefox */
background: -moz-linear-gradient(250deg, rgba(0,0,25,1) 0%, ...);
/* Chrome/Safari */
background: -webkit-linear-gradient(250deg, rgba(0,0,25,1) 0%, ...);
/* Standard */
background: linear-gradient(250deg, rgba(0,0,25,1) 0%, ...);
```

### Viewport Strategy
- Nav container: `70vw` (max 800px, min 300px)
- Breakpoints: 768px (mobile), 2560px (large desktop)
- Logo sizing: 120px default, 90px mobile, 150px large

### Layout
- Centered logo prominence (120px)
- Social links horizontal below logo
- Flexbox column layout for nav, row for social-links