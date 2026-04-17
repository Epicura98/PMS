# Project UI Style Guide & Specifications

This document outlines the exact color theme, typography, and component styling used in the **Crockery Cutlery** Project. Use these specifications to apply an identical look and feel to other systems.

## 1. Typography
- **Primary Font Family**: `'Outfit'`, sans-serif.
- **Google Fonts Import**:
  ```css
  @import url('https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;500;600;700;800;900&display=swap');
  ```
- **Base Styles**:
  - `font-family: 'Outfit', sans-serif;`
  - Body Background: `#f5f3ff` (Light Lavender/Violet tint).

## 2. Color Palette

### Primary Colors (Violet/Lavender)
- **Primary Action**: `#7c3aed` (Tailwind `violet-600`)
- **Primary Hover**: `#6d28d9` (Tailwind `violet-700`)
- **Light Accent**: `#ede9fe` (Tailwind `violet-100`)
- **Subtle Accent**: `#f5f3ff` (Tailwind `violet-50`)
- **Shadow Color**: `rgba(139, 92, 246, 0.05)` (Violet shadow tint)

### Functional Accents
- **Success / Return**: `#10b981` (Tailwind `emerald-500`)
- **Info / Issued**: `#3b82f6` (Tailwind `blue-500`)
- **Balance / Special**: `#c026d3` (Tailwind `fuchsia-600`)
- **Warning / Alert**: `#ea580c` (Tailwind `orange-600`)
- **Danger / Delete**: `#ef4444` (Tailwind `red-500`)

### Neutral Palette (Slate)
- **Deep Text**: `#0f172a` (Tailwind `slate-900`)
- **Primary Text**: `#1e293b` (Tailwind `slate-800`)
- **Secondary Text**: `#475569` (Tailwind `slate-600`)
- **Subtle Text / Placeholder**: `#94a3b8` (Tailwind `slate-400`)
- **Borders / Dividers**: `#e2e8f0` (Tailwind `slate-200`)
- **Surface Background**: `#f0f2f8` (Light blue-grey tint)

## 3. Component Specifications

### Cards & Containers
- **Background**: `#ffffff` (White)
- **Border**: `1px solid #ede9fe` (violet-100)
- **Corner Radius**: `1rem` (16px / `rounded-2xl`)
- **Shadow**: `shadow-xl shadow-violet-500/5`
- **Hover Style**: `hover:shadow-violet-500/10 transition-all duration-500`

### Buttons
- **Primary Button**:
  - Background: Gradient `from-violet-600 to-fuchsia-500`
  - Text: White, font-semibold
  - Radius: `0.75rem` (12px / `rounded-xl`)
- **Ghost/Outline Button**:
  - Border: `1px solid #ede9fe`
  - Text: `#94a3b8` (slate-400)
  - Hover: `text-violet-600 hover:bg-violet-50`
- **Tab Buttons**:
  - Active: `bg-white text-violet-600 shadow-xl shadow-violet-100/50`
  - Inactive: `text-slate-500 hover:text-slate-700`

### Tables
- **Header Row**:
  - Background: `#f5f3ff` (violet-50) with `backdrop-blur-sm`
  - Text: `#7c3aed` (violet-600), bold, uppercase, tracking-widest (`0.2em`)
- **Body Rows**:
  - Border: `1px solid #f8fafc` (slate-50)
  - Hover: `bg-slate-50/50 transition-colors`
  - Cell Padding: `py-3.5 px-4`

### Form Inputs
- **Style**: `h-9 rounded-xl bg-white border border-slate-200 outline-none`
- **Focus State**: `border-violet-300 ring-4 ring-violet-500/5`
- **Labels (Special)**: Small, all-caps, tracking-widest (`text-[10px] font-black uppercase tracking-widest text-slate-400`).

## 4. Visual Flourishes
- **Backdrop Blur**: Use `backdrop-blur-sm` on sticky headers and modals.
- **Micro-Animations**:
  - Entry: `animate-in fade-in slide-in-from-bottom-6 duration-1000`
  - Hover: Use `scale-110` or `scale-[1.02]` for interactive elements.
- **Scrollbar**: Custom thin violet scrollbar.
  - Thumb: `#c4b5fd` (violet-300)
  - Width: 4px - 6px

## 5. UI Prompt Strategy
When prompting an AI to apply this theme, use the following:
> "Apply a modern, premium dashboard theme with a 'Violet/Lavender' professional aesthetic. Use the 'Outfit' font from Google Fonts. Background should be #f5f3ff with cards in white and #f0f2f8 sections. Primary actions should use #7c3aed or a violet-to-fuchsia gradient. Implement wide letter-tracking for uppercase labels, rounded-2xl corners (16px), and subtle violet shadows (shadow-violet-500/5). Tables should have a sticky violet-50 header with violet-600 bold text."
