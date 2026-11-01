# CCC181 Week 10: CampusConnect Mobile-First Login Page

React + TypeScript starter for the Week 10 group activity. The page is already
built. Your group's job is the **mobile-first CSS** and the **GitHub teamwork**.

## Run it

```bash
npm install
npm run dev          # open the local URL it prints
npm run dev:phone    # same, but your phone (same Wi-Fi) can open the Network URL
npm run build        # must finish with no errors before you submit
```

## Rules

- Edit only the CSS files in `src/styles/` (one member = one file). Do not edit `reset.css`.
- Plain CSS only. No Tailwind, Bootstrap, Material UI, styled-components, or any UI library.
- Phone styles first (no media query), then `min-width` queries only. Never `max-width`.
- Do not edit the `.tsx` files or rename classes. If you must, tell the group first.

## Group information (fill in)

| Item | Your answer |
| --- | --- |
| Group number | CAPPIS |
| Section | IT3A |
| Repository URL | https://github.com/enialle2/ccc181-week10-group-CAPPIS |

## Members (each member fills in their own row in their own commit)

| Member | Name | GitHub username | CSS file | What I did |
| --- | --- | --- | --- | --- |
| 1 (leader) | Ellaine Dulalas | enialle2 | `base.css` | I wrote base.css (...your full sentence...) |
| 2 | | | `nav.css` | |
| 3 | Zemeco M. Buntag | zemecobuntag | `form.css` | Styled the login form to be mobile-friendly and responsive on bigger screens. |

main

## Experiment 0: the page without the viewport tag

What did the page look like in DevTools phone mode **before** adding the viewport meta tag?
- Before adding the viewport meta tag, the page in DevTools phone mode specifically in an iPhone SE- looked zoomed out and very small, as if a full desktop page had been shrunk to fit the phone screen. The text was tiny and hard to read, and the layout looked like the desktop version instead of a phone layout.
What changed **after** adding it?
- After I added <meta name="viewport" content="width=device-width, initial-scale=1"> to index.html and reloaded, the page used the real phone width. The text became normal-sized and readable, and the layout stacked into a single column that fit the screen. This showed me that without the viewport tag, the browser assumes a wide desktop width, so the media queries and mobile styles don't behave properly on a phone.

> (write your answer here)

## DevTools test results

| Width   | What must be true                                                                                                  | Pass? |
| ------- | ------------------------------------------------------------------------------------------------------------------ | ----- |
| 360 px  | 1 column. Nav links stacked and 48px tall. Options and buttons stacked. Footer in 1 column. No sideways scrollbar. |       |
| 768 px  | Nav in one row (brand left, links right). Checkbox and link in one row. Two buttons side by side.                  |       |
| 1024 px | Brand panel and login card side by side. Footer in 3 columns. Heading is larger.                                   |       |
| 1280 px | Content centered and stops at 1200px.                                                                              |       |

### Breakpoints I observed

Using **Show media queries** and dragging slowly from 360 px to 1280 px, the layout changed at these exact widths:

> (write the widths here, and say whether any width looked broken)

Screenshots are in `screenshots/` as `360.png`, `768.png`, `1024.png`, `1280.png`.

## What our group learned (leader writes this last)

> (write your answer here)
