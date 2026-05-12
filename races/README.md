# Apex by Milla

Independent technical analysis of every 2026 Formula 1 Grand Prix, written by an aspiring race engineer.

**Live site:** [apexbymilla.com](https://apexbymilla.com)

---

## About

I'm Milla, 16, and Apex by Milla is the long-term portfolio project I'm building alongside my GCSEs as I work toward a career in Formula 1 race engineering. Each post breaks a race down through an engineering lens: tyre strategy under the new 2026 regulations, energy management with the 50/50 power unit split, active aero behaviour, post-race penalty analysis, and pit wall decision-making.

The site is designed to deepen in analytical depth over the course of the 2026 season. The goal is to demonstrate not just an interest in the sport, but a developing ability to read a race like a race engineer would.

---

## Stages of Development

The analytical depth of the writing is deliberately scaled across the season, in four stages, so the progression is visible to anyone reading the site chronologically:

- **Stage 1 (Rounds 1-3 — complete):** Foundations. Race overview, qualifying breakdown, technical breakdown covering tyre strategy and aerodynamics, race results, and DNF analysis.
- **Stage 2 (Rounds 4-8 — in progress):** Comparative and quantitative analysis. Added a Pace & Performance table comparing drivers by fastest lap, pit stop time, and gap at flag. Added an Engineering Question of the Race section that picks one specific pit-wall moment and dissects the trade-off. Added a Race Engineer's View paragraph offering my own pit-wall verdict. Added Sources sections citing primary FIA, F1, and Pirelli references.
- **Stage 3 (Rounds 9-14 — planned):** Data-driven analysis. Will introduce charts via the FastF1 Python library, a glossary page called The Apex Index explaining technical terms, and component reference graphics.
- **Stage 4 (Rounds 15-22 — planned):** Cross-race trend analysis, team upgrade tracking, season-long championship context.

---

## Tech Stack

Deliberately simple, so iteration is fast and the site is easy to maintain:

- **HTML5** for content and structure
- **CSS** — embedded inline in each HTML file (no separate stylesheet, to avoid a GitHub Pages cache issue I ran into early on)
- **Vanilla JavaScript** for interactive elements:
  - Mobile navigation hamburger toggle
  - Scroll-reveal animations via IntersectionObserver
  - Date-based "NEW" banner that auto-fades to "LATEST" seven days after a race publishes
- **GitHub Pages** for hosting
- **Custom domain** via Namecheap with HTTPS enforced
- **Python + Pillow** for one-off image processing (generating the 1200×630 social-share image with a solid background for link previews)
- **No framework, no build step** — kept simple so I can focus on the content and learn the fundamentals properly

---

## Engineering Practices

- **Primary-source citation:** every race report ends with a Sources section grouped by category (Official Race Data, Tyre Strategy, Race Report & Driver Quotes, plus race-specific groups). Sources are linked directly to formula1.com results pages, Pirelli race debriefs, FIA announcements, and reputable F1 journalism.
- **Fact-checking workflow:** before publishing, every technical claim (regulation values, tyre compounds, lap counts, weight specifications, etc.) is cross-checked against the FIA 2026 Technical Regulations summary, F1's official explainer pages, and McLaren's regulations breakdown.
- **On-road vs final classification:** post-race penalties that change the finishing order are flagged with an asterisk on the affected driver cards, with a footnote explaining the penalty. This distinguishes what happened on track from what the stewards' decisions changed.
- **Mobile responsive:** the Pace & Performance data table is wrapped in a horizontally-scrollable container so it doesn't break layout on phones.
- **Social link previews:** dedicated 1200×630 share image on a solid dark background so the logo is readable when the URL is shared on Instagram, Twitter, or messaging platforms.

---

## File Structure

```
apex-by-milla/
├── index.html                      Homepage
├── races/
│   ├── australia.html              Round 01 — Australian GP
│   ├── china.html                  Round 02 — Chinese GP (Sprint)
│   ├── japan.html                  Round 03 — Japanese GP
│   ├── miami.html                  Round 04 — Miami GP (Sprint, first Stage 2 post)
│   └── NEW-RACE-TEMPLATE.html      Stage 2 template for future races
├── logo.png                        Site logo (transparent background)
├── social-share.png                1200×630 link-preview image (solid dark bg)
├── me.jpg                          About-section portrait
├── sitemap.xml                     SEO sitemap
├── robots.txt                      Search engine crawler rules
├── CNAME                           GitHub Pages custom domain config
├── CHANGELOG.md                    Version history
└── README.md                       This file
```

---

## What's Next

Immediate roadmap:
- The Apex Index (glossary page explaining technical terms across the site)
- Static graphics for each indexed component (in-washing bargeboards, active aero modes, MGU-K, etc.)
- FastF1 integration for actual lap-by-lap charts in race reports (Stage 3)

---

## Contact

apexbymilla@gmail.com

[Instagram](https://instagram.com/apexbymilla) · [X](https://x.com/apexbymilla) · [TikTok](https://tiktok.com/@apexbymilla) · [Facebook](https://facebook.com/apexbymilla)

---

*Apex by Milla is an independent technical analysis project. Not affiliated with Formula 1, the FIA, or any F1 team.*
