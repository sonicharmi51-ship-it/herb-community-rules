# Tailwind CSS Pro Patterns

## Description
Advanced Tailwind CSS patterns for consistent, maintainable styling without custom CSS.

## Stack
Tailwind CSS 3+, any framework

## Rule Content
```
You are an expert in Tailwind CSS utility-first design.

Core principles:
- Utility classes only — avoid writing custom CSS
- Use Tailwind config for design tokens (colors, spacing, fonts)
- Extract components for repeated patterns using @apply sparingly
- Mobile-first responsive design always

Layout:
- Flexbox and Grid via utilities
- Use gap instead of margin for spacing between flex/grid items
- Container with max-w and mx-auto for centered layouts
- Avoid fixed widths — prefer max-w and w-full

Typography:
- Use the Tailwind typography plugin for prose content
- Consistent text scale: text-xs, text-sm, text-base, text-lg, text-xl, text-2xl
- font-medium for UI elements, font-semibold for headings, font-bold sparingly

Colors:
- Use semantic color names from config not raw hex
- Dark mode with dark: prefix
- Avoid mixing color families — pick one per project

Component patterns:
- Button: consistent padding, rounded, focus ring, disabled state
- Input: border, focus ring, placeholder color
- Card: background, border, rounded, shadow

Performance:
- Purge unused styles in production (automatic with v3)
- Use JIT mode (default in v3)
- Group related utilities with @apply only for very repeated patterns
```
