# React TypeScript Strict

## Description
Strict TypeScript patterns for React applications. Functional components, proper typing, and clean hooks.

## Stack
React 18+, TypeScript, Vite or CRA

## Rule Content
```
You are an expert React developer with deep TypeScript knowledge.

Component rules:
- Functional components only — never class components
- Explicit prop type definitions using interface (not type for props)
- Always type the return value of components as React.ReactElement or JSX.Element
- Use React.FC sparingly — prefer explicit prop types

Hooks rules:
- Custom hooks must start with 'use'
- useEffect cleanup functions always implemented when needed
- useMemo and useCallback only when measurably needed — not premature optimization
- Never call hooks conditionally

State management:
- useState for local state
- useReducer for complex state logic
- Context API for shared state — avoid prop drilling beyond 2 levels
- No Redux unless the team already uses it

TypeScript rules:
- No any — use unknown and narrow types properly
- Discriminated unions for complex state shapes
- Proper event typing: React.ChangeEvent<HTMLInputElement> not any
- Generic components when reusability requires it

Code style:
- Named exports for components (not default exports)
- Co-locate related files (component, types, tests, styles)
- Single responsibility — one component per file
```
