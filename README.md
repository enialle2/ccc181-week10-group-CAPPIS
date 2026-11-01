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
| 1 (leader) | Ellaine Dulalas | enialle2 | `base.css` | I wrote base.css (page layout and brand panel from phone to 1280px) and added the viewport meta tag and .gitignore. |
| 2 | | | `nav.css` | |
| 3 | Zemeco M. Buntag | zemecobuntag | `form.css` | Styled the login form to be mobile-friendly and responsive on bigger screens. |

## Experiment 0: the page without the viewport tag

What did the page look like in DevTools phone mode **before** adding the viewport meta tag?

What changed **after** adding it?

> I first noticed the effect of the viewport tag in DevTools phone mode (iPhone SE), and I repeated the check later, after base.css and form.css had already been added, so the page was already styled. With the viewport meta tag commented out, the page was laid out as if the screen were much wider than the phone. The content was cut off on the right side, so the heading and the sign-in card did not fit and I would have had to scroll sideways or zoom out to see them. After restoring `<meta name="viewport" content="width=device-width, initial-scale=1">` and reloading, the page used the real phone width. The layout fit the screen, the text was a normal readable size, and everything stacked in a single column. This showed me that without the viewport tag, the browser assumes a wide desktop width, so the mobile styles and media queries do not behave as intended.

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
