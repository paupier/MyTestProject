# Style Guide: "Production Systems" Presentation Slide

A reference guide for recreating the visual aesthetic of the Rockwell Automation "Software Defined System" presentation slide.

---

## 1. Brand Identity

### Logo
- **Shape**: Regular hexagon (flat-top orientation)
- **Background**: Deep red (`#C0182A`)
- **Text**: "RA" in bold white, sans-serif, centered
- **Placement**: Top-right corner, moderate size (approximately 8–10% of slide width)
- **Padding**: Slight internal padding between text and hexagon edges

---

## 2. Color Palette

### Primary Colors
| Role | Name | Hex | Usage |
|------|------|-----|-------|
| Background | Deep Navy | `#080E1A` | Slide/canvas background |
| Accent | Amber Orange | `#F5820A` | Primary highlight, glows, right border bar |
| Highlight | Vivid Cyan | `#00D4FF` | Data lines, wireframe structures, UI elements |
| Text Primary | Pure White | `#FFFFFF` | Main body text |
| Text Accent | Golden Yellow | `#F7C948` | Subheading labels, emphasized text |

### Secondary / UI Colors
| Role | Name | Hex | Usage |
|------|------|-----|-------|
| Brand Red | Rockwell Red | `#C0182A` | Logo background |
| Panel BG | Dark Slate | `#0D1826` | Dashboard panel fills |
| Muted Cyan | Steel Blue | `#2A6B8A` | Secondary data lines |
| Glow Orange | Soft Amber | `#FF9A30` | Halo/glow effects on 3D elements |
| Grid Line | Dim Gray | `#1E2B3A` | Subtle grid overlays |

### Gradient Usage
- **Background glow**: Radial gradient from `#1A2B40` (center) to `#080E1A` (edges)
- **Orange bar** (right edge): Solid vertical stripe in `#F5820A`, approximately 3–4% of slide width
- **Ambient light**: Soft orange radial glow emanating from the center-right of the 3D model

---

## 3. Typography

### Font Family
- **Primary**: Sans-serif geometric font (e.g., **Neue Haas Grotesk**, **Aktiv Grotesk**, or fallback: `Inter`, `Arial`)
- **All text**: Left-aligned, no decorative serifs

### Text Hierarchy

| Element | Style | Weight | Size (relative) | Color |
|---------|-------|--------|-----------------|-------|
| Main headline line 1 | `Production systems that` | Regular (300–400) | ~5.5% of slide height | White `#FFFFFF` |
| Main headline line 2 | `learn and adapt` | **Bold (700–800)** | ~5.5% of slide height | White `#FFFFFF` |
| Main headline line 3 | `real-time` | Regular (300–400) | ~5.5% of slide height | White `#FFFFFF` |
| Section label | `SOFTWARE DEFINED SYSTEM` | **Bold uppercase** | ~2.5% of slide height | Golden Yellow `#F7C948` |

### Type Rules
- Line-height: tight (1.1–1.2×)
- Letter-spacing on section label: wide (`0.15em`)
- No text shadows; rely on contrast against dark background
- Text block anchored to **lower-left** quadrant, with generous margin from bottom and left edges

---

## 4. Layout & Composition

```
┌─────────────────────────────────────────────┬──┐
│                                        [RA] │  │
│                                             │  │
│         [Complex Dashboard UI / 3D Model]   │  │
│                                             │  │
│                                             │O │
│  Production systems that                   │R │
│  learn and adapt real-time                 │A │
│                                             │N │
│  SOFTWARE DEFINED SYSTEM                   │G │
│                                    [15]    │E │
└─────────────────────────────────────────────┴──┘
```

### Grid
- **Slide ratio**: 16:9
- **Safe zone margin**: ~6% from all edges for text and logo
- **Right edge accent bar**: Solid vertical stripe, full height, ~3.5% of slide width, color `#F5820A`
- **Slide number**: Small white text, bottom-right corner (inside safe zone, left of orange bar)

---

## 5. Background Dashboard / HMI Visualization

This is the most complex element — a layered, dark industrial control/monitoring interface.

### Structure
- Multiple **panel regions** arranged in a grid-like layout, each simulating HMI (Human-Machine Interface) screens
- Panels have subtle dark borders (`#1E2B3A`) and very low opacity fills
- Overall feel: a live operations dashboard for a smart factory

### Key Visual Sub-Elements

#### 3D Wireframe Building Model (Center)
- Isometric or perspective view of a multi-story industrial facility
- Rendered in **cyan/teal lines** (`#00D4FF`) with low-opacity fills (`rgba(0,212,255,0.05)`)
- Surrounded by an amber/orange **glow halo** (`#FF9A30`, blur radius ~40px)
- Slight upward-facing camera angle

#### Data Panels (Left and Right)
- Bar charts, line graphs, and status indicators
- Chart bars: alternating orange (`#F5820A`) and cyan (`#00D4FF`)
- Small text labels in white or light gray
- Thin horizontal divider lines in `#1E2B3A`

#### Circular / Radial Indicators (Right side)
- Concentric circle gauges or donut charts
- Colors: orange and cyan
- Glowing edge effect using `box-shadow` or a blurred duplicate layer

#### Data Flow Lines / Connection Lines
- Thin lines (`1–2px`) in cyan (`#00D4FF`) connecting elements
- Some with animated dash or arrow hints (for motion design contexts)
- Subtle glow: `drop-shadow(0 0 4px #00D4FF)`

#### Status Indicators / Tags
- Small rectangular pill-shaped elements
- Fill: orange `#F5820A` or red `#C0182A`
- White text, small and tight

### Depth & Atmosphere
- **Depth-of-field blur**: Elements toward edges of the dashboard appear slightly blurred/defocused
- **Light bloom**: Center of the image has increased brightness/glow
- **Overall opacity**: The entire dashboard layer sits at roughly 75–85% opacity over the dark background to keep text readable

---

## 6. Effects & Visual Treatments

| Effect | Description |
|--------|-------------|
| Ambient glow | Radial orange glow (`#FF9A30`) behind the 3D model, ~300px blur |
| Neon edge glow | Cyan elements have a `drop-shadow(0 0 6px #00D4FF)` treatment |
| Panel depth | Subtle `box-shadow: inset 0 0 20px rgba(0,0,0,0.5)` on panels |
| Grain/noise | Very subtle film grain overlay (opacity 3–5%) for cinematic feel |
| Vignette | Dark radial vignette at corners to focus attention on center |

---

## 7. Photography / Stage Context (for composite scenes)

If the slide is shown in a physical venue context (as in the source image):
- Stage lighting: warm amber/tungsten tones
- Screen luminance should read well against dimly lit environments
- Presenters or physical elements in foreground should not require style changes to the slide itself

---

## 8. Do's and Don'ts

### Do
- Use dark backgrounds exclusively; never light/white backgrounds
- Keep text strictly left-aligned and in the lower-left region
- Apply orange and cyan as the only two accent colors
- Maintain high contrast between text and the dashboard background layer
- Use uppercase and wide letter-spacing for sub-labels

### Don't
- Don't use gradients on text (flat colors only)
- Don't place primary text over the densest part of the dashboard UI
- Don't use more than two accent colors (orange + cyan) in a single composition
- Don't use rounded corners on the outer slide frame
- Don't add drop shadows to text; rely on contrast alone
