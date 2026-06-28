# Skill: Lovable Elite UI/UX Architecture (/pixel-perfect)

## Description
Enforces elite, human-grade UI design and layout structure across Lovable Vite + React, Tailwind, and shadcn/ui codebases. Trigger this when creating landing pages, dashboard modules, or layout components.

## Strict Structural Rules
1. Framework Focus: Always use modular React hooks and functional components. Split bloated sections into clean, individual sub-components inside the codebase.
2. Component Library: Prioritize headless `shadcn/ui` components for all interactive states (modals, dropdowns, sheets, tabs). Do not code custom raw states if a shadcn alternative exists.
3. CSS Grid & Flexbox: Mandate structured layouts. Rely completely on Tailwind flex rows/columns or `grid grid-cols-1 md:grid-cols-3 gap-6`. Never use arbitrary float positioning.

## Visual Design Constraints
1. Typographic Contrast: Maintain precise typography scales. Titles must use tracking-tight constraints (e.g., `text-3xl md:text-5xl font-bold tracking-tight text-foreground`). Subtexts must utilize explicit `text-muted-foreground`.
2. Responsive Guardrails: Every layout class written must be natively mobile-first. Test screen break points utilizing `sm:`, `md:`, and `lg:` prefixes. Prevent layout overflows.
3. Interactive Feedback: All buttons, link states, and interactive dashboard elements must contain smooth Tailwind transition triggers (e.g., `transition-all duration-200 hover:opacity-90 active:scale-[0.98]`).
4. Padding & Whitespace: Eradicate crowded interfaces. Apply a minimum baseline of `py-12 px-4 md:px-8` to structural sections to ensure proper whitespace breathing room.
