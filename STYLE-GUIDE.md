# Museum Planner style guide

Use this for **museumplanner.org** (including `index.html` in this repo), Kit broadcasts that point here, book landing pages, course descriptions, and static essays. The **homepage (v3)** and **long-form essays** share ink/cream/copper DNA but use different layouts—dark practitioner hub vs. light reading room for a single piece.

---

## Visual identity — Homepage (`index.html`, v3)

The public homepage is a **dark practitioner hub**: warm ink background, cream type, copper accents, three pillars (Community · Courses · Essays), and clear separation from **museumplanning.com**.

### Color tokens (CSS `:root` in `index.html`)

| Token | Approx. hex | Role |
|-------|----------------|------|
| **Ink** | `#111010` | Page background |
| **Ink mid** | `#1e1c1a` | Panels, cards |
| **Ink soft** | `#2a2622` | Secondary surfaces |
| **Cream** | `#f5f0e8` | Primary text |
| **Cream dim** | `#c8c0b4` | Body / secondary paragraphs |
| **Cream faint** | `rgba(245,240,232,0.15)` | Muted overlays |
| **Copper** | `#b5763a` | Eyebrows, rules, accents, primary CTA fill |
| **Copper light** | `#d4904a` | CTA hover |
| **Red** | `#8b2020` | Accent (use sparingly) |
| **Rule** | `rgba(245,240,232,0.1)` | Hairlines on dark |
| **Rule warm** | `rgba(181,118,58,0.3)` | Copper-tinted borders |

Do **not** introduce arbitrary rainbow accents. New components should reuse these tokens.

### Typography (Google Fonts, loaded in `index.html`)

| Role | Font | Usage |
|------|------|--------|
| **Display / hero** | **Playfair Display** | Hero headline, pillar titles, essay titles in lists |
| **UI / labels / nav / meta** | **DM Mono** | Top strip, masthead nav, section labels, post meta, buttons, audience tags |
| **Body** | **DM Sans** (light) | Hero deck, course blurbs, sidebar copy, footer |

**Logo in this template:** Text wordmark in Playfair with an italic copper **Planner**—not the circular PNG lockup on the homepage itself. Circular PNGs in `assets/` remain **Museum Planning** brand artwork for print, email, or **museumplanning.com**.

### Layout and components (homepage)

- **Top strip:** DM Mono; links to **museumplanning.com** and **mark-walhimer.com**.
- **Masthead:** Sticky ink bar; nav to `#courses`, `#essays`, `#community`, `#about`; **Hire Mark →** copper CTA.
- **Hero:** Eyebrow (DM Mono, copper) + Playfair headline; primary **Join the Community** / **Explore Courses**.
- **Pillars:** Three-column grid (Community · Courses · Essays) on desktop; stack on small screens.
- **Recent Writing:** `post-item` list; newest essay links to static HTML in-repo (e.g. `genz_town_square_article.html`); older items may use WordPress-style paths until migrated.
- **Archive link:** `/archive` for WordPress parity when the domain still serves the blog.

### Motion

- Subtle **fade-up** on hero and sections (short duration, ease). Avoid busy animation on editorial pages.

---

## Visual identity — Long-form essays (`genz_town_square_article.html`)

**Practitioner Intelligence** pieces use a **light reading room** on cream, distinct from the dark homepage but aligned on copper and serif tone.

### Color tokens (essay template)

| Token | Approx. hex | Role |
|-------|----------------|------|
| **Navy** | `#0d1b2a` | Masthead, hero, footer |
| **Mid blue** | `#354583` | In-article links |
| **Copper** | `#b87333` | Kicker, rules, emphasis |
| **Cream** | `#f7f3ed` | Page background |
| **Warm gray** | `#e8e2da` | Pull quotes, panels |

### Typography (essays)

| Role | Font | Usage |
|------|------|--------|
| **Headlines** | **Playfair Display** | Article `h1`, section heads |
| **Body** | **DM Sans** (light) | Paragraphs, deck |
| **Labels / meta** | **DM Mono** | Kicker, hero meta, tags |

### Essay chrome

- Masthead links back to **`index.html`** (Museum Planner home).
- Series line: **Practitioner Intelligence**; attribute research to **Museum Planning, LLC** where the piece is firm-branded, with **museumplanner.org** as the publication surface.
- Footer: series, date, and path home—not a duplicate consulting landing page.

---

## Consistency with museumplanning.com

- **Same family, different room:** Commercial site sells engagements; Museum Planner builds **community, courses, and literacy**. Visual language can differ (dark hub here; commercial site may stay light + circle mark).
- **Cross-links:** Always make **museumplanning.com** obvious for hiring; copper styling on this site should not obscure that path.
- **Favicon / social:** Prefer a mark derived from the Playfair wordmark or circle asset—pick one system and document the file in this repo when finalized.

---

## Voice

- **Expert and direct.** Write for educators, exhibit staff, emerging professionals, and decision-makers who are short on time.
- **Humane, not hype.** Acknowledge complexity (politics, funding, community, generational change) without drama or jargon walls.
- **First person when it's yours.** Mark's byline and practitioner tone match the homepage; product pages can use "we" for Museum Planning LLC where legally accurate.

## Terminology

- **Museum Planning** or **Museum Planning, LLC** — the consulting practice; hiring, feasibility, master planning, engagements.
- **Museum Planner** — this site and brand for community, courses, essays, and archive. Do not use "Museum Planner" to mean the LLC contract unless that's legally intentional.
- **Master plan / master planning** — reserve for real scope-of-work language; do not use for a low-ticket course title.

## Headlines and titles

- Prefer concrete nouns and stakes: who it's for, what changes.
- Avoid clickbait; avoid vague "The future of museums" unless the piece earns it in the first paragraphs.
- Display headlines may use **Playfair** with optional *italic* for contrast (see hero patterns in `index.html` and essay templates).

## Calls to action

- **Primary on Museum Planner:** Join community, explore courses, read essays, newsletter (when wired)—education and relationship.
- **Consulting path:** **Hire Mark →**, **museumplanning.com**, **mark@museumplanning.com**, and practice links must stay easy to find on templates that mirror the homepage.
- Do not imply that a course or book replaces feasibility study, master planning, or RFP-driven work.

## Email and Kit

- Subject lines: specific benefit or topic, under roughly 60 characters when possible.
- Preheader: complements the subject; does not repeat it verbatim.

## Inclusive and precise language

- Say **municipalities**, **institutions**, **boards**, **communities** where accurate; avoid defaulting to "cities" if counties or regional bodies are in scope.
- When discussing demographics or conflict, be factual and respectful; avoid stereotyping.

## Formatting (Markdown and web)

- Use sentence case for headings unless a proper noun requires otherwise.
- One idea per short paragraph on web; longer essays may use subheads every few screens.
- Link out to primary sources (government, museum, news) when citing policy or news events.

## Things to fix in draft

- Strip filler ("It goes without saying," "In today's ever-changing world").
- Replace vague intensifiers with data, examples, or a clear recommendation.

---

## Legacy assets (circle mark)

PNG circle lockups for **Museum Planning** (white label on red circle) live in `assets/`. Use them where the **red circle** brand is required (e.g. email signatures, slide decks, museumplanning.com). They are **not** the default hero mark on the current Museum Planner `index.html`; export a **Museum / Planner** circle variant if you need the circle on this property too.
