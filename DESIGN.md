# Lotta Portfolio Page — Locked Design

**Locked on:** 2026-04-11
**Purpose:** Single-scroll portfolio page for LinkedIn, founder accelerator applications, cold outreach.
**Audience:** SF founders, accelerator admissions, technical hiring managers who weight taste/personality/agency over pedigree.
**Hosting:** Vercel, with a GitHub repo as source of truth.

---

## Creative direction

**Vibe:** Calvin Klein 1995 print ad × Vogue Italia dark editorial × Nordic minimalism. Single long scroll. Feels like flipping through one issue of a luxury fashion-tech magazine. Generous blackspace. Restraint, not collage.

**Palette (three colors only):**
- Background: pure black `#0a0a0a`
- Primary text / headlines: ivory `#f2ece2`
- Chrome / captions / metadata / photo frames: warm bone `#e8ddc8`
- Single accent (section numbers, dividers, pull-quotes, link hover): **Tiffany Blue `#0ABAB5`** (Pantone 1837)

**Typography (two families):**
- Display serif (headlines, huge, thin weight): **Playfair Display** — Didot/Bodoni feel, free on Google Fonts
- Sans (body, captions, metadata): **Inter** — Neue Haas Grotesk feel, free on Google Fonts
- Everything lowercase except proper nouns and the name on the cover. Matches Lotta's LinkedIn voice.

**Photo treatment:** Desaturated slightly, grainy, generous blackspace around every image. Never full-bleed unless it's the cover hero. Tiny warm-bone typewriter-style captions underneath each photo. No rotation, no collage, no torn edges — this is CK, not Ray Gun.

**Layout:** Wide side margins (magazine gutter feel). Generous vertical spacing between sections. Mobile reads as a tall single column with the same content and hierarchy.

**Motion:** Minimal. Subtle scroll fade-ins for section headers. Eha ad video auto-plays muted and loops. No parallax, no fancy cursors, no confetti.

---

## Section-by-section

### 00 · Cover

- Top-left metadata strip (tiny bone sans): `issue 01 — spring 2026 — san francisco`
- Centered headline, huge thin Playfair, two lines:
  ```
  LOTTA-LORETTE
  KALMARU
  ```
- Sub-line directly below, italic ivory:
  > *i build things that ship. i make companies money. i move fast.*
- Bottom-left: `scroll ↓` in tiny bone sans
- Bottom-right: small b&w photo (`me_at_sf.jpeg`), framed in warm bone

### 01 · First job title: co-founder. (Eha Lighting)

- Section number `01` in Tiffany teal
- Headline: **first job title: co-founder.**
- Hero media: **`eha_ad.mov` converted to .mp4/.webm, auto-playing muted loop**, 1280px wide, framed in warm bone
- Body copy (short declarative sentences, CK pacing):
  > *at eighteen, co-founded eha lighting — a nordic design hardware company. designed and shipped a cordless lamp with powerbank functionality built into the base: no cables, no dock, it charged your phone. launched it on indiegogo. €10,000+ in year one. best estonian student company 2020. represented estonia at ja europe. entrepreneurial student of the year — estonian ministry of education.*
- Pull-quote offset to the side, italic Tiffany teal:
  > *"nordic design, with a battery inside."*
- Photo strip below the body: `eha_building_amp.jpeg`, `eha_team_winning.jpg`, `eha_magazine.jpeg`, `eha_booth_sales.jpeg` — four small frames, each with tiny bone captions (`tallinn, 2020` etc.)

### 02 · Ship it. Make them money. (STACC — stakeholder mgmt + DS)

- Section number `02` in Tiffany teal
- Headline: **four years shipping ml across energy, retail, and agritech.**
- Body:
  > *led a four-person team at estonian cell — live day-ahead energy forecasting, €100,000 saved year one, owned airflow monitoring and incident response. built the personalised discount engine for coop (330+ stores, millions of transactions, 600k+ loyalty members) — estonia's first. scoped e-agronom precision farming directly with agronomists, fused sentinel-3 satellite signals with local weather for soil temperature prediction.*
- Three pull-quotes down the side, each in Tiffany teal:
  - *"€100,000 saved. year one."*
  - *"first personalised discount engine in estonia."*
  - *"four-person team. production monitoring. i owned incidents."*
- Hero photo: one of the `meworking*.JPG` shots (pick the best), wide, cinematic, framed in warm bone

### 03 · ECB Scholar.

- Section number `03`
- Headline: **chosen by the european central bank.**
- One tight paragraph:
  > *competitive eu-wide scholarship for women in economics and tech. €10,000 grant plus ecb mentorship. selected for outstanding academic achievement and technical expertise.*
- Photo: `20241128_Women_Scholarship_Session_FE_PM_AMC_0659.JPG` — medium, framed, caption `ecb scholarship session, frankfurt, 2024`
- Deliberately quiet — the "credibility anchor" section

### 04 · Research.

- Section number `04`
- Headline: **a model that catches kidney disease 21 years before diagnosis.**
- Body:
  > *built the end-to-end pipeline across 13,000+ biobank participants. multi-modal — nmr metabolomics, 21 years of longitudinal environmental exposures, demographics. designed a novel deep unfolded neural architecture: non-black-box, neural network flexibility, fast inference. shipped uncertainty-aware outputs with 90% coverage guarantees. auc 0.76 at 80% sensitivity.*
- Tiny inline links under the body (Tiffany teal, underlined):
  - `live demo → conformal-triage-demo.streamlit.app`
  - `full resume →`
- Hero photo: one of `meworking4.JPG` or `meworking5.JPG`, b&w treatment

### 05 · Off the record. (About)

- Section number `05`
- Headline: **off the record.**
- One short paragraph:
  > *grew up in estonia. was the kid who took care of the animals — donkeys, chickens, sheep, horses, real ones, for years. co-founded a company at eighteen before i'd ever written a line of production code. came to machine learning from the math up. took the ferry across the baltic to school in helsinki. came to san francisco to find the heart of tech. still mostly here for the work and the animals. sf has more dogs than children. that was on the pros list.*
- Photo strip below: four square photos with tiny captions
  - `me_and_donkey.jpeg` — caption: *lotta and a donkey, estonia*
  - `me_and_cat.jpeg` — caption: *home, 2024*
  - `me_at_tartu_university.jpeg` — caption: *tartu, 2023*
  - `me_at_sf.jpeg` — caption: *san francisco, 2025*

### 06 · Contact / back page.

- Headline: **let's talk.**
- Three lines, clean monospaced feel:
  - `email — lotta.lorette@gmail.com`
  - `linkedin — linkedin.com/in/lotta-lorette-kalmaru`
  - `demo — conformal-triage-demo.streamlit.app`
- Tiny footer: `© 2026 lotta-lorette kalmaru · set in playfair & inter · printed in san francisco`

---

## Copy rules (locked)

- Everything lowercase except the name on the cover and proper nouns inside sentences (SF, JA Europe, Sentinel-3, etc.)
- Short declarative sentences in the CK rhythm
- Never "i had the opportunity to" or "i'm deeply inspired by"
- Always value-forward: what was built, what it did, what it saved or earned
- No exclamation marks anywhere

## Tech stack (locked)

- Single `index.html` file, embedded CSS, minimal vanilla JS
- Google Fonts CDN: Playfair Display + Inter
- No frameworks, no build step
- Assets: `images/` (optimized jpegs), `video/` (eha_ad.mp4 + .webm)
- Responsive: mobile reads as tall single column
- Host: **Vercel** (connected to a GitHub repo for auto-deploy)
- Repo: TBD — user will create on GitHub, local git repo initialized here first

## Pending user inputs (resolved at lock)

- **Eha headline:** *first job title: co-founder.* (chosen from four alternatives)
- **Accent color:** Tiffany Blue `#0ABAB5` (upgraded from muted oxidized teal)
- **Accent 2:** warm bone `#e8ddc8` (chrome/captions only)
- **SF line in About:** *came to san francisco to find the heart of tech.*
- **About length:** one short paragraph + four small photos
- **Structure:** single long scroll
- **Personal detail: animals** — donkeys, chickens, sheep, horses (animal caretaker as a teen)
- **Personal detail: ferry** — took the ferry across the baltic to school in helsinki from tallinn
- **Include the eha ad video** — as hero media in section 01, muted autoplay loop
