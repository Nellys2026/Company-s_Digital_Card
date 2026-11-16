# Nellys Tech — Theme, Color & Design System (`global.css` & `global.js`)

## 1. Theme Architecture
- Controlled by the `[data-theme="light"]` and `[data-theme="dark"]` attribute on `<html>`.
- Persisted in `localStorage` under the key `nellys_theme`.
- Logo auto-switches between:
  - **Light Theme:** `nellys-logo-light.svg` (Deep Cyan `#0099DD`–`#0077B6` `N` + Midnight Navy `#0B0F19` `T`)
  - **Dark Theme:** `nellys-logo-dark.svg` (Bright Cyan `#38BDF8`–`#00A3E0` `N` + Crisp White `#FFFFFF` `T`)

---

## 2. Color Tokens (`:root` vs `[data-theme="dark"]`)

| Token | Light Theme (Soft Indigo Mist) | Dark Theme (Midnight Tech) |
| :--- | :--- | :--- |
| `--bg-page` | `#EEF2FF` | `#090D16` |
| `--bg-surface` | `#F8FAFF` | `#111827` |
| `--bg-surface-2` | `#E0E7FF` | `#1E293B` |
| `--bg-card` | `#FFFFFF` | `#111827` |
| `--bg-header` | `rgba(224, 231, 255, 0.96)` | `rgba(9, 13, 22, 0.95)` |
| `--bg-footer` | `#E0E7FF` | `#030712` |
| `--text-primary` | `#0F172A` | `#F1F5F9` |
| `--text-secondary` | `#334155` | `#CBD5E1` |
| `--text-muted` | `#64748B` | `#94A3B8` |
| `--border-color` | `#C7D2FE` | `#1E293B` |
| `--accent` | `#4F46E5` (Indigo) / `#0284C7` (Sky) | `#38BDF8` (Cyan) |
| `--accent-indigo` | `#6366F1` | `#818CF8` |
| `--accent-emerald` | `#059669` | `#34D399` |
| `--accent-amber` | `#D97706` | `#FBBF24` |
| `--card-shadow` | `0 4px 20px rgba(79, 70, 229, 0.06)` | `0 4px 30px rgba(0, 0, 0, 0.5)` |

---

## 3. Typography & Visual Patterns
- **Primary Font Stack:** `'Plus Jakarta Sans', 'Inter', sans-serif`
- **Service Card Photo Overlay System:**
  - `.service-card` uses real service photography (`assets/services/service-01.jpg` – `service-20.jpg`) with `.service-card-bg` and `.service-card-overlay` for high-contrast readability in both Light and Dark themes.
- **Interactive Animations:**
  - `.letter-reveal` / `.split-char` for headline character reveals.
  - `.reveal-on-scroll`, `.reveal-from-left`, `.reveal-from-right`, `.reveal-scale` for scroll-triggered animations.
