# Style Guide & Design System: LoboThExile.github.io

## 1. Design Direction & Persona
* **Owner:** LoboThExile (Lobo)
* **Domain:** `https://lobothexile.github.io`
* **Archetype:** Precision engineering, terminal-inspired dark aesthetics, grounded builder portfolio.
* **Core Philosophy (Anti-Slop):**
  * **No generic AI tropes:** Avoid neon purple-to-pink gradient hero text, blurry radial background orbs, and copy-paste identical cards.
  * **Authentic voice:** Present real projects (Minecraft datapacks, Arduino hardware systems, developer utilities, web apps) with concise, truthful descriptions.
  * **Restraint:** High visual contrast, crisp typography, disciplined accent color usage, and lightweight zero-dependency architecture.

---

## 2. Color Palette & Tokens

| Token | Hex / Value | Role |
| :--- | :--- | :--- |
| `--bg-base` | `#090d13` | Deep canvas background |
| `--bg-surface` | `#111620` | Card, container, and section surfaces |
| `--bg-elevated` | `#18202d` | Interactive hover states, elevated chips |
| `--border-subtle` | `#232d3f` | Default card borders, structural dividers |
| `--border-hover` | `#3c4c66` | Focused/hovered element borders |
| `--text-primary` | `#f0f6fc` | Headings, hero statement, primary titles |
| `--text-secondary`| `#919eb0` | Body copy, repo descriptions, subtitles |
| `--text-muted` | `#586577` | Metadata, tags, timestamps, mono indicators |
| `--accent-primary`| `#38bdf8` | Terminal cyan: primary links, active badges, highlights |
| `--accent-active` | `#0284c7` | Pressed / active state for interactive elements |
| `--status-online` | `#22c55e` | Signal green: live status indicator |

---

## 3. Typography & Spacing Scale

### Font Stacks
* **Monospace (Headings, tags, terminal prompts):**
  `'JetBrains Mono', 'Fira Code', 'SFMono-Regular', Consolas, 'Courier New', monospace`
* **Sans-Serif (Body prose, longform reading):**
  `system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif`

### Type Hierarchy
* **Display / Hero H1:** `2.25rem` (`36px`), line-height `1.2`, weight `700`, monospace
* **Section Heading H2:** `1.35rem` (`21px`), line-height `1.3`, weight `600`, monospace
* **Card Title H3:** `1.05rem` (`17px`), line-height `1.4`, weight `600`, sans-serif
* **Body Text:** `0.925rem` (`14.8px`), line-height `1.6`, weight `400`, sans-serif
* **Mono Badges / Metadata:** `0.775rem` (`12.4px`), line-height `1.4`, weight `500`, monospace

### Spacing System
* Base unit: `4px`
* Common rhythm: `8px` (compact), `16px` (standard gap), `24px` (card padding), `48px` (section separator)
* Max container width: `840px` (centered single-column layout for high density and readability)

---

## 4. Layout & Structural Hierarchy

1. **Top Bar / Header:**
   * Clean status chip: `● Available on Discord` (`lobothexile`)
   * Quick links: `GitHub`, `Projects`, `Stack`

2. **Hero Terminal Block:**
   * Prominent handle: `LoboThExile`
   * Direct, grounded subtitle: Game logic developer, systems tinkerer, and utility builder.
   * Compact quick stats: Public repos, primary languages, active learning track.

3. **Featured Projects (Differentiated Cards):**
   * **Flagship (Highlight card):**
     * `Pointmatch` — Minecraft Datapack
     * `SemestraEnterprise` — Modern web application
   * **Tools & Experiments (Grid):**
     * `antigravity-account-switcher` — Developer utility
     * `The-Wild-Hunt` — PvP game mechanic
     * `SecurityAlarmArduino` — Laser & photoresistor IoT system
     * `Die-Of-Death-Mod` — Game mod

4. **Technical Competencies (Categorized Chips):**
   * **Languages:** Java, Python, Luau, C++, JavaScript / TypeScript, HTML/CSS
   * **Domains:** Minecraft Datapack Development, Arduino / Embedded Logic, Web Frontends, Tooling

5. **Connect / Footer:**
   * Discord copy badge (`lobothexile`) with one-click clipboard feedback
   * Direct GitHub link (`github.com/LoboThExile`)
   * Fast, static, 0KB runtime bloat footprint

---

## 5. UI Elements & Interaction States

* **Buttons & Cards:**
  * Subtle 1px solid border (`--border-subtle`).
  * 6px border radius (no exaggerated pill shapes on large containers).
  * Subtle background shift on hover (`--bg-surface` -> `--bg-elevated`).
  * Instant, snappy transition: `transition: border-color 0.15s ease, background-color 0.15s ease`.
* **Badges:**
  * Pill-shaped (`border-radius: 9999px`), padding `2px 8px`.
  * Monospace, subtle contrasting border.
* **Accessibility & Performance:**
  * Fully keyboard navigable with crisp `:focus-visible` outline (`2px solid var(--accent-primary)`).
  * Contrast ratio >= 4.5:1 (WCAG AA compliant for all body text; >= 7:1 for headers).
  * `color-scheme: dark;` declared on root.
  * No external web font render-blocking (uses system font stack with standard fallback).
