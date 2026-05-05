# Museum Planner style guide

Use this for **museumplanner.org** (including `index.html` in this repo), Kit broadcasts that point here, book landing pages, and course descriptions. It is aligned with the **current static homepage**: dark editorial layout, serif reading tone, and clear separation from **museumplanning.com**.

---

## Visual identity — Museum Planner site (`index.html`)

The public homepage is a **dark “reading room”**: warm ink background, cream type, copper accents, and restrained red for emphasis—not a light Inter + circle lockup template.

### Color tokens (CSS `:root` in `index.html`)

| Token | Approx. hex | Role |
|-------|----------------|------|
| **Ink** | `#141210` | Page background |
| **Ink mid** | `#2a2520` | Panels, distinction block |
| **Ink soft** | `#3d3830` | Secondary surfaces |
| **Cream** | `#f5f0e8` | Primary text |
| **Cream dim** | `#e8e2d6` | Body / secondary paragraphs |
| **Cream mute** | `#b8b0a2` | Muted labels |
| **Copper** | `#b5763a` | Eyebrows, rules, accents, primary CTA fill |
| **Red** | `#c0392b` | Accent (use sparingly; pairs with `--red-soft` where defined) |
| **Rule** | `rgba(245,240,232,0.12)` | Hairlines on dark |
| **Rule warm** | `rgba(181,118,58,0.25)` | Copper-tinted borders |

Do **not** introduce arbitrary rainbow accents. New components should reuse these tokens.

### Typography (Google Fonts, loaded in `index.html`)

| Role | Font | Usage |
|------|------|--------|
| **Display / logo wordmark** | **Playfair Display** | Masthead “Museum**Planner**” (second word in copper), hero `h1`, card titles, post titles, book titles |
| **Body / long reading** | **Source Serif 4** (light/regular) | Body copy, excerpts, sidebar bio |
| **UI / labels / nav** | **DM Sans** | Masthead nav (uppercase, letterspaced), section labels, meta lines, buttons, footer |

**Logo in this template:** Text wordmark in Playfair with a copper-highlighted second word—not the circular PNG lockup on the homepage itself. Circular PNGs in `assets/` remain the **Museum Planning** brand artwork for print, email, or properties that use the red circle mark.

### Layout and components

- **Masthead:** Sticky, translucent ink bar; nav links muted cream → cream on hover; **Hire Mark →** uses copper outline CTA (`nav-cta`).
- **Hero:** Eyebrow line (DM Sans, copper, uppercase) + large Playfair headline; body in Source Serif; inline link to **museumplanning.com** in copper, no underline clutter.
- **Main + sidebar grid** (desktop): main column for sections; sidebar for bio, books, **The Practice** links, contact card.
- **Section labels:** DM Sans, 10px-ish feel, wide letterspacing, uppercase, copper, bottom rule (`section-label`).
- **Distinction block:** `ink-mid` background, **3px copper** left border—use for “two sites, two purposes” messaging.
- **Responsive:** Stack columns under ~900px; trim some nav items on very small screens as in the template.

### Motion

- Subtle **fade-up** on hero and page body (short duration, ease). Avoid busy animation on editorial pages.

### Consistency with museumplanning.com

- **Same family, different room:** Commercial site sells engagements; Museum Planner sells **attention and literacy**. Visual language can differ (editorial dark here; commercial site may stay light + circle mark).
- **Cross-links:** Always make **museumplanning.com** obvious for hiring; copper/red styling on this site should not obscure that path.
- **Favicon / social:** Prefer a mark derived from Playfair wordmark or circle asset—pick one system and document the file in this repo when finalized.

---

## Voice

- **Expert and direct.** Write for decision-makers and practitioners who are short on time.
- **Humane, not hype.** Acknowledge complexity (politics, funding, community) without drama or jargon walls.
- **First person when it’s yours.** Mark’s byline and “where the arguments live” tone match the homepage; product pages can use “we” for Museum Planning LLC where legally accurate.

## Terminology

- **Museum Planning** or **Museum Planning, LLC** — the consulting practice; hiring, feasibility, master planning, engagements.
- **Museum Planner** — this site and brand for writing, archive, books, public thinking. Do not use “Museum Planner” to mean the LLC contract unless that’s legally intentional.
- **Master plan / master planning** — reserve for real scope-of-work language; do not use for a low-ticket course title.

## Headlines and titles

- Prefer concrete nouns and stakes: who it’s for, what changes.
- Avoid clickbait; avoid vague “The future of museums” unless the piece earns it in the first paragraphs.
- Display headlines may use **Playfair** with optional *italic* for contrast (see hero pattern in `index.html`).

## Calls to action

- **Primary on Museum Planner:** Read, archive, books, newsletter (when wired)—education and relationship.
- **Consulting path:** **Hire Mark →**, **The Practice** block, **mark@museumplanning.com**, and links to **museumplanning.com** must stay easy to find on templates that mirror the homepage.
- Do not imply that a course or book replaces feasibility study, master planning, or RFP-driven work.

## Email and Kit

- Subject lines: specific benefit or topic, under roughly 60 characters when possible.
- Preheader: complements the subject; does not repeat it verbatim.

## Inclusive and precise language

- Say **municipalities**, **institutions**, **boards**, **communities** where accurate; avoid defaulting to “cities” if counties or regional bodies are in scope.
- When discussing demographics or conflict, be factual and respectful; avoid stereotyping.

## Formatting (Markdown and web)

- Use sentence case for headings unless a proper noun requires otherwise.
- One idea per short paragraph on web; longer essays may use subheads every few screens.
- Link out to primary sources (government, museum, news) when citing policy or news events.

## Things to fix in draft

- Strip filler (“It goes without saying,” “In today’s ever-changing world”).
- Replace vague intensifiers with data, examples, or a clear recommendation.

---

## Legacy assets (circle mark)

PNG circle lockups for **Museum Planning** (white label on red circle) live in `assets/`. Use them where the **red circle** brand is required (e.g. email signatures, slide decks, museumplanning.com). They are **not** the default hero mark on the current Museum Planner `index.html`; export a **Museum / Planner** circle variant if you need the circle on this property too.
