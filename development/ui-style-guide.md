# 🎨 UI Style Guide – Adaptive Music AI with Closed-Loop Learning

---

## 🎯 Purpose
This style guide ensures **visual consistency** across all screens of the MVP.  
It defines the core design language — colors, typography, and UI components — that developers and designers should follow.

---

## 1️⃣ Color Palette

| Color Name | Hex Code | Usage |
|------------|----------|-------|
| Primary Blue | #2D9CDB | CTA buttons, highlights |
| Secondary Purple | #9B51E0 | Accent elements, active states |
| Background Light | #F9FAFB | App background |
| Background Dark | #1B1B1B | Dark mode background |
| Text Primary | #212121 | Main text |
| Text Secondary | #6E6E6E | Subtext and labels |
| Success Green | #27AE60 | Positive feedback indicators |
| Error Red | #EB5757 | Errors, dislikes |

**Tip:** Always ensure **contrast ratio > 4.5** for accessibility.

---

## 2️⃣ Typography

**Primary Font:** [Inter](https://rsms.me/inter/) (Sans-serif)  
**Fallback:** Arial, Helvetica, sans-serif

| Usage | Font Weight | Size (px) | Example |
|-------|-------------|-----------|---------|
| H1 Headings | Bold (700) | 28px | "Your Music, Always Evolving" |
| H2 Subheadings | Semi-bold (600) | 22px | "Recommended Playlists" |
| Body Text | Regular (400) | 16px | "Choose your favorite genres" |
| Small Text | Regular (400) | 14px | "Last updated 2 hours ago" |
| Buttons | Semi-bold (600) | 16px | "Get Started" |

---

## 3️⃣ Iconography

**Icon Set:** [Feather Icons](https://feathericons.com/) (lightweight, scalable)

| Icon | Usage |
|------|-------|
| Play | Playback start |
| Pause | Playback stop |
| Skip | Skip track |
| Heart | Like/favorite |
| Thumbs Down | Dislike |
| Music | Genre selection |
| Search | Artist search |

---

## 4️⃣ UI Components

### Buttons
- **Primary Button:**
  - Background: Primary Blue (#2D9CDB)
  - Text: White (#FFFFFF)
  - Border-radius: 8px
  - Padding: 12px 20px
- **Secondary Button:**
  - Background: Transparent
  - Border: 1px solid Primary Blue
  - Text: Primary Blue

---

### Cards (Playlists)
- Background: White (#FFFFFF)
- Border-radius: 12px
- Shadow: 0px 4px 10px rgba(0,0,0,0.05)
- Cover image at top, text below

---

### Feedback Pop-Up
- Background: White (#FFFFFF)
- Border-radius: 10px
- Option buttons: Secondary Purple when selected
- Submit button: Primary Blue

---

## 5️⃣ Layout & Spacing

- **Grid System:** 8px spacing rule (all margins and paddings in multiples of 8)
- **Safe Area:** Respect top and bottom safe areas on mobile
- **Alignment:** Left-aligned for text, center-aligned for icons

---

## 6️⃣ Accessibility Guidelines
- **Font Size:** Minimum 14px for small text
- **Color Contrast:** Test using [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
- **Alt Text:** All images and icons must have descriptive alt text

---

## 📌 Next Step in ACSPO Flow
Proceed to **`development-plan.md`** – define the technical stack, development milestones, and deployment plan for the MVP.
