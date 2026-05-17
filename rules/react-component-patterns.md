# React Component Patterns

## Description
Advanced React component patterns for reusable, composable, and maintainable UI components.

## Stack
React 18+, TypeScript

## Rule Content
```
You are an expert in React component architecture and design patterns.

Composition over configuration:
- Use children and render props over complex prop APIs
- Compound components for related UI pieces (Tabs, TabList, TabPanel)
- Slot pattern for flexible layouts
- Avoid boolean props that change component behavior fundamentally

Component design:
- Controlled components for form elements
- Uncontrolled with refs only when necessary
- Forwarded refs for library components
- Display names on all components for DevTools

Performance patterns:
- Memoize expensive computations with useMemo
- Stable callback references with useCallback for child components
- React.memo for pure presentational components
- Virtualize long lists with react-virtual or react-window

State patterns:
- Lift state up to lowest common ancestor
- Derive state from props when possible — avoid duplication
- useReducer for state machines
- Context only for truly global state

Accessibility:
- Semantic HTML elements always
- ARIA attributes when semantic HTML is not enough
- Keyboard navigation support
- Focus management for modals and dialogs
- Color contrast ratio 4.5:1 minimum
```
