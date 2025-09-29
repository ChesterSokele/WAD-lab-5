Design Decisions & Challenges
Design Decisions
1. CSS Variables System
Decision: Used CSS custom properties for theming consistency

Why: Easy theme switching, maintainable code, color consistency

Implementation: Root-level color, spacing, shadow variables

2. Component-Based Architecture
Decision: Modular CSS classes per component type

Why: Scalable, reusable, easy to maintain

Example: .card, .btn, .chip classes are separate

3. Mobile-First Responsive Design
Decision: Mobile base styles, additions for larger screens

Why: Performance, progressive enhancement

Implementation: Media queries for tablets/desktops

4. Consistent Visual Hierarchy
Decision: Unified spacing, typography, and color system

Why: Professional appearance, better user experience

Implementation: Consistent padding, margins, and font sizes

⚠️ Challenges Faced
1. Dark Mode Implementation
css
/* Challenge: Maintaining contrast and readability */
body.dark-theme {
  --body-bg: #121212;      /* Deep dark for less eye strain */
  --card-bg: #1e1e1e;      /* Slightly lighter for depth */
--text-color: #e2e8f0;   /* High contrast light text */
Solution: Used a layered dark palette with sufficient contrast ratios

2. Component Consistency
Challenge: Making all components look consistent

Solution: Shared design tokens (variables) and consistent spacing

3. Responsive Behavior
Challenge: Components breaking on small screens

Solution: Flexible grids and stacked layouts on mobile

4. Browser Compatibility
Challenge: CSS Grid and custom properties support

Solution: Progressive enhancement and fallbacks
