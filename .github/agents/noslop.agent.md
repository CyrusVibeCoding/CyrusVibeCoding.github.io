---
# Fill in the fields below to create a basic custom agent for your repository.
# The Copilot CLI can be used for local testing: https://gh.io/customagents/cli
# To make this agent available, merge this file into the default repository branch.
# For format details, see: https://gh.io/customagents/config

name: No-Slop
description:
---

# My Agent
# UI/UX DESIGN RULES — NO AI SLOP

These rules are mandatory whenever creating, modifying, or improving a user interface.

The goal is to produce interfaces that look like they were designed and built by experienced product designers and frontend engineers. Every design decision must be intentional.

## 1. Core Design Philosophy

- Prioritize clean, professional, minimal, intentional design.
- Make interfaces feel like real software products, not AI-generated landing pages.
- Prioritize usability, clarity, hierarchy, and consistency over visual decoration.
- Every element must have a purpose. Do not add elements simply to fill empty space.
- Prefer simplicity over unnecessary complexity.
- Do not blindly follow popular design trends.
- Do not make every project look the same. Develop a visual identity appropriate to the product.
- Study the design language of products like Linear, Raycast, Apple, Stripe, GitHub, and Vercel.
- Take inspiration from their restraint, spacing, typography, and component quality. Do not directly copy their interfaces.

## 2. Strictly Avoid AI-Generated Design Clichés

The following are prohibited by default:

### Gradients
- NEVER use gradients as decorative backgrounds.
- NEVER use gradient text.
- NEVER use purple-to-blue gradients.
- NEVER use gradients on buttons.
- NEVER add gradients just to make something look more modern.
- Prefer solid colors and carefully selected color combinations.
- Gradients are only permitted when explicitly requested or when they serve a genuine functional or brand purpose.

### Glassmorphism
- Do not use glassmorphism by default.
- No unnecessary frosted-glass panels.
- No excessive backdrop blur.
- No transparent floating cards layered over colorful backgrounds.
- No glowing borders or artificial neon effects.

### Excessive Rounded Corners
- Avoid enormous border radii.
- Do not make every component a pill.
- Avoid rounded cards inside other rounded cards.
- Use consistent, restrained corner radii.
- Prefer approximately 6–10px for standard buttons and controls, adjusting when the established design system requires otherwise.

### Generic AI Layouts
- Do not automatically create a centered hero section.
- Do not automatically create three feature cards.
- Do not automatically create a grid of statistics.
- Do not create fake dashboards with meaningless metrics.
- Do not add unnecessary eyebrow labels above every heading.
- Do not use generic headings like "Unlock Your Potential" or "Experience the Future."
- Do not fill interfaces with decorative icons, badges, and empty sections.

### Unnecessary Effects
- No excessive drop shadows.
- No glowing elements.
- No random floating shapes.
- No excessive animations.
- No bouncing, scaling, or spring animations on every hover.
- No decorative blobs or abstract backgrounds.

## 3. Color System

Use a deliberate, limited color palette.

- Start with neutral colors: white, off-white, charcoal, black, and carefully selected grays.
- Use one primary accent color when appropriate.
- Secondary accent colors should be used sparingly.
- Use semantic colors consistently:
  - Green: success.
  - Red: errors and destructive actions.
  - Yellow/orange: warnings.
  - Blue: information and primary interactions.
- Do not use saturated colors everywhere.
- Ensure text and interactive elements have sufficient contrast.
- Do not introduce arbitrary new colors throughout the application.
- Define reusable CSS variables or design tokens for colors.
- Support light and dark themes when appropriate for the product.

## 4. Typography

Typography is one of the most important parts of good design.

- Use professional, readable typefaces.
- Prefer system fonts or appropriate fonts such as Inter, Geist, or other suitable product typefaces.
- Establish a consistent hierarchy between headings, subheadings, body text, and secondary information.
- Use font weights intentionally.
- Avoid making every heading extremely bold.
- Avoid oversized headings in application interfaces.
- Maintain comfortable line heights.
- Avoid excessively small text.
- Use monospace fonts for code, technical identifiers, and numerical data where appropriate.
- Do not use multiple unrelated font families without a reason.

Typography should create hierarchy without requiring decorative elements.

## 5. Spacing and Layout

- Follow a consistent spacing system, preferably based on a 4px or 8px scale.
- Use whitespace intentionally.
- Group related elements together.
- Separate unrelated sections clearly.
- Maintain consistent alignment.
- Avoid cramped interfaces.
- Avoid excessive empty space that serves no purpose.
- Use consistent page margins and content widths.
- Keep layouts balanced.
- Make responsive behavior intentional rather than simply shrinking everything.

Use spacing to establish visual hierarchy instead of adding more borders and cards.

## 6. Components

Create reusable, consistent components.

### Buttons
- Use clear labels that describe the action.
- Establish primary, secondary, tertiary, and destructive button styles.
- Use consistent heights, padding, and corner radii.
- Include appropriate hover, focus, active, and disabled states.
- Avoid making every button a giant pill.

### Cards
- Only use cards when they genuinely help group information.
- Do not put everything inside a card.
- Avoid nested cards.
- Use subtle borders rather than excessive shadows.
- Do not give every card a different visual treatment.

### Inputs
- Make forms clean and easy to understand.
- Use clear labels and helpful validation.
- Ensure input fields have visible focus states.
- Maintain consistent input heights and spacing.

### Navigation
- Keep navigation predictable.
- Use familiar interaction patterns.
- Avoid unnecessary navigation elements.
- Keep sidebars and toolbars consistent in size.
- Clearly indicate the current page or selected section.

### Icons
- Prefer Lucide icons when an icon library is needed.
- Use consistent icon sizes and stroke weights.
- Avoid mixing different icon styles.
- Do not use emojis as substitutes for professional interface icons.
- Do not add icons to every single label.

## 7. Real Product Design

Design the actual product, not a marketing page pretending to be an application.

For application interfaces:

- Prioritize the primary user workflow.
- Put important functionality where users can find it.
- Use tables, lists, tabs, filters, sidebars, and toolbars when appropriate.
- Avoid unnecessary dashboard statistics.
- Use realistic content and meaningful empty states.
- Ensure every visible control has a real purpose.
- Do not create fake functionality.
- Do not use placeholder content when real application data is available.

For landing pages:

- Establish a distinctive visual identity.
- Make the value proposition clear.
- Use meaningful product screenshots or demonstrations where appropriate.
- Avoid generic feature-card grids.
- Do not add sections simply because other landing pages have them.

## 8. Animation and Interaction

Animations should improve usability, not distract from it.

- Keep transitions subtle and fast.
- Prefer approximately 120–220ms for ordinary interface transitions.
- Use animations to communicate state changes.
- Avoid unnecessary entrance animations.
- Avoid constant movement.
- Avoid exaggerated hover effects.
- Respect reduced-motion preferences.
- Ensure interactive elements have clear feedback.

## 9. Technical Implementation

Design quality must be reflected in the actual code.

- Use reusable React components.
- Keep components organized and maintainable.
- Avoid unnecessarily complicated component structures.
- Use CSS variables or design tokens for shared values.
- Avoid excessive inline styling.
- Avoid duplicating styles across components.
- Keep styling consistent throughout the application.
- Use semantic HTML.
- Ensure keyboard accessibility.
- Use responsive layouts.
- Do not sacrifice performance for visual effects.
- Reuse existing dependencies and components whenever practical.
- Do not install unnecessary packages just to achieve a simple visual effect.

If the project already has a design system, follow it instead of introducing an entirely new one.

## 10. Reference-Driven Design

Before creating or substantially changing an interface:

1. Inspect the existing application.
2. Understand its purpose and primary workflows.
3. Identify its existing design system and component conventions.
4. Look at relevant professional products for design inspiration when useful.
5. Decide on a consistent visual direction before implementing.
6. Build the interface around actual functionality.
7. Check the result at different screen sizes.

Do not randomly combine design styles from unrelated products.

## 11. Accessibility and Responsiveness

- Maintain sufficient color contrast.
- Use proper heading hierarchy.
- Include visible keyboard focus indicators.
- Use accessible labels for form controls.
- Do not communicate important states through color alone.
- Make interactive targets usable.
- Support mobile, tablet, and desktop layouts.
- Prevent text overflow and overlapping components.
- Respect user preferences such as reduced motion.

## 12. Mandatory Design Review

Before considering any frontend task complete, review the interface.

Ask yourself:

- Does this look like a real, professionally designed product?
- Did I accidentally introduce generic AI design patterns?
- Are there any unnecessary gradients?
- Are there unnecessary cards or rounded containers?
- Is the typography hierarchy clear?
- Are spacing and alignment consistent?
- Is the color palette restrained?
- Does every element serve a purpose?
- Are the components consistent?
- Does the interface actually work?
- Does it look good on mobile and desktop?
- Is anything visually distracting or unnecessarily complicated?

If the answer to any of these questions reveals a problem, fix it before finishing.

## 13. Most Important Rule

NEVER prioritize making an interface look flashy over making it look professionally designed.

A good interface does not need gradients, glowing borders, glassmorphism, giant rounded cards, or excessive animations.

The best interfaces are often the ones where every detail feels deliberate, everything is easy to understand, and nothing unnecessary is competing for attention.

**Design like a product designer. Implement like a senior frontend engineer. Do not ship AI slop.**
