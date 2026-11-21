---
version: alpha
name: "Genealogy research template by 8B"
description: "Family history research one-pager in pale paper sheets with coloured index tabs on a black desk, handwritten notes and stamped photos. Free HTML template by 8B, MIT."
colors:
  primary: "#1b1b1b"
  secondary: "#474747"
  tertiary: "#c5b9c4"
  neutral: "#0d0d0d"
  surface: "#e6ebed"
  on-surface: "#1b1b1b"
  desk: "#0d0d0d"
  paper-blue: "#d4dce5"
  paper-sage: "#cbcfc6"
  paper-mauve: "#c5b9c4"
  slip: "#f6f8f9"
typography:
  headline-display:
    fontFamily: Reddit Sans
    fontSize: 96px
    fontWeight: 800
    lineHeight: 0.9
    letterSpacing: -0.055em
  headline-lg:
    fontFamily: Reddit Sans
    fontSize: 84px
    fontWeight: 800
    lineHeight: 0.9
    letterSpacing: -0.055em
  headline-md:
    fontFamily: Reddit Sans
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.025em
  body-lg:
    fontFamily: Reddit Sans
    fontSize: 20px
    fontWeight: 400
    lineHeight: 1.38
    letterSpacing: -0.005em
  body-md:
    fontFamily: Reddit Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
  label-caps:
    fontFamily: Reddit Sans
    fontSize: 12px
    fontWeight: 600
    lineHeight: 1.3
    letterSpacing: 0.09em
  button:
    fontFamily: Reddit Sans
    fontSize: 13px
    fontWeight: 700
    lineHeight: 1
    letterSpacing: 0.1em
  note-hand:
    fontFamily: Playwrite US Trad
    fontSize: 17px
    fontWeight: 400
    lineHeight: 1.55
  pressed-word:
    fontFamily: Playwrite US Trad
    fontSize: 300px
    fontWeight: 400
    lineHeight: 1
rounded:
  none: 0px
  tab: 10px
  stamp: 5px
  full: 9999px
spacing:
  gutter: 30px
  sheet-max: 820px
  sheet-gap: 28px
  sheet-padding-x: 26px
  sheet-padding-top: 56px
  tab-bar-height: 40px
  tab-width: 50px
  tab-height: 104px
  field-height: 50px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.surface}"
    typography: "{typography.button}"
    rounded: "{rounded.none}"
    padding: "12px 20px"
    height: 44px
  button-primary-hover:
    backgroundColor: "{colors.paper-blue}"
    textColor: "{colors.primary}"
  text-link:
    textColor: "{colors.on-surface}"
    typography: "{typography.button}"
    padding: "2px 1px"
  index-tab:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
    rounded: "{rounded.tab}"
    width: 50px
    height: 104px
  paper-sheet:
    backgroundColor: "{colors.paper-blue}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.none}"
    padding: "56px 26px"
  price-slip:
    backgroundColor: "{colors.slip}"
    textColor: "{colors.primary}"
    padding: "10px 14px"
  step-badge:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.surface}"
    typography: "{typography.label-caps}"
    padding: "3px 6px"
  input-field:
    backgroundColor: transparent
    textColor: "{colors.primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.none}"
    padding: "14px 6px"
    height: 50px
---

# Kinfold

## Overview

Kinfold is a one-page website for a family history research service that hands each client a bound folder of what it found. The one idea is a desk covered in paper: pale sheets in four quiet tints lie on a black ground, index tabs stick out of their edge, photos carry perforated stamp edges, and big handwritten words are pressed into the sheets. It should feel like an archive reading room, patient and tactile, written for families who arrive with one photograph. The demo firm, people, prices and letters are invented.

## Colors

Eight values sit in `:root`, `--color-1` to `--color-8`.

- **Desk (#0d0d0d):** the page ground, under a faint grain, and the mask colour of the stamp edges.
- **Surface (#e6ebed):** pale paper sheets, the pale index tabs, button labels and text set straight on the desk.
- **Paper-blue (#d4dce5):** blue sheets and tabs, and the panel that turns in when a button is hovered.
- **Paper-sage (#cbcfc6):** sage sheets and tabs, the bars drawn under the archive titles, the highlight on a hovered link.
- **Paper-mauve (#c5b9c4):** mauve sheets and tabs, and the bar behind a hovered question.
- **Primary (#1b1b1b):** text on paper, buttons, rules, chart dots and lines, the thread, dark step badges.
- **Secondary (#474747):** small grey text on paper such as chart details, photo captions, the towns under the letters and placeholders.
- **Slip (#f6f8f9):** price slips, step slips, the Story panel and tab, and the highlight edge of the pressed words.

Contrast on paper is 14:1 for primary and 7:1 for secondary on the pale sheet. The blue, sage and mauve tints are for grounds only; never mix them into text.

## Typography

- **Reddit Sans**, one variable face for weights 400 to 800, carries all running text. Headings are weight 800, uppercase, tight (line height 0.9, tracking -0.055em). Labels are 12px, weight 600, uppercase, tracked 0.09em. Buttons and links are 13px, weight 700, tracked 0.1em. Body text is regular.
- **Playwrite US Trad**, a single weight of schoolroom handwriting, is the voice of notes: photo captions, the open chart entries, letter signatures and the huge pressed words. Never use it for headings or paragraphs.

`headline-display` is the opening heading, 96px on wide screens (11vw on phones, capped at 92px). `headline-lg` sets every other section heading, 84px at most and 42px at least. `headline-md` is the 24px step, package and panel title. `body-lg` is the 20px lead under each heading. `pressed-word` is clamp(120px, 22vw, 300px). The four spellings in the opening and the package prices are Reddit Sans 800 at 58px and 50px.

## Layout

Everything stands in one sheet column, 820px at most, set left of centre so the index tabs fit in the space on the right. On phones the sheets fill the width less 16px and the tabs form a 40px bar along the top. Sheets are separated by a 28px strip of desk (16px on phones) and padded 56px by 26px on wide screens.

- Each sheet is a heading, a lead and one device: stepped slips, folder tabs with a panel, a pedigree chart, a portrait row (two by two on phones), a fee list, a form table.
- The archives and letters sections have no sheet; they sit on the desk in pale text.
- Questions and contact split into a narrow head and a wide body at 900px and above.
- The side gutter is 16px to 30px.

## Elevation & Depth

Depth is paper. A shadow token, a 1px contact line plus a soft 22px drop, lifts slips, folder panels and the ledger window. Sheets themselves are flat and sit on the grain of the desk. Index tabs run back under the sheet edge, so a hovered or current tab slides out of the paper. The huge pressed words use two text shadows, a dark one up and left and a light one down and right, to look debossed; their depth changes with the scroll.

## Shapes

- Sheets, buttons, fields and badges have square corners.
- Index tabs and folder tabs round only their outer corners, 10px.
- Photos except the ledger are cut with a perforated stamp edge, a 5px scallop (4px in the portraits and opening snapshots, 7px to 9px in the room photo). A few sit rotated by one or two degrees.
- Chart entries are marked by a 9px dot, filled for known people, an open ring for the three still being looked for.
- Rules are 1px lines in primary; the chart lines are 1.2px and the thread 1.5px.
- Opening photos are desaturated, and the portraits are greyscale.

## Components

- **button-primary:** a dark block, 44px high, with a panel in paper-blue that turns in from its left edge on hover while the label darkens.
- **text-link:** 13px bold uppercase, underlined by 1px; a sage highlight sweeps behind it on hover.
- **index-tab:** a tinted tab, 50px wide and 104px tall on wide screens with vertical text, level along the top on phones. The current one is pushed out further.
- **paper-sheet:** a tinted ground with a dot grid and grain, text in primary.
- **price-slip:** a near-white slip with a shadow; the visit card and the reply note are tilted a degree or two.
- **step-badge:** a small dark label for the step number, inked in by a bar.
- **input-field:** a label column of 104px and a control with a 1px underline, no box.

## Motion

The page loads no animation library. Scroll scenes are CSS scroll-driven animations (named view timelines), written per section in `<style data-8b-part="scene:...">` blocks. A small inline motion kit at the end of the body numbers list items into `--i`, measures distances into CSS variables, adds `is-in` to `data-8b-motion` elements as they arrive (`settle` for slips and photos, `ink` for the highlighter behind step labels), pauses endless loops off screen, and smooths the mouse wheel (fine pointers only; touch scrolls natively). The huge pressed words (`press`) deepen as their sheet crosses the screen, and the letters (`roll`) loop sideways. A gate script in the head sets `data-8b-live` on the root only when the browser supports `animation-timeline` and the visitor has no reduced-motion preference; every scroll rule is scoped to it. The one idea: the folder is assembled as you read, with paper settling into place.

- **Opening:** on load the heading rises, the intro, buttons and four spelling rows slide up one after another, and the two stamped photos settle.
- **Archives:** a paper-edged window with an enlarged copy of the ledger (added by a short scene script) moves down the dimmed photo while the five titles are underlined in turn.
- **Method:** an ink thread (an SVG path the scene script draws from the slips' positions) draws between four tilted slips, and each slip straightens as the thread reaches it.
- **Folder:** tabs switch panels with a click or the arrow keys; photos drop into place.
- **Case:** a stage that sticks for about one and a half screens of scrolling (a 250vh track), zoomed on the client, pulls back while each generation's lines, dots and names appear; each generation is timed from the entry's `--i`.
- **People:** four portraits start joined as one perforated block and tear apart into their places, four in a row on wide screens and two by two on phones, as names wipe in. The start offsets are inline variables on each card.
- **Letters:** five slips scroll sideways in a 70 second loop (the letters script doubles the row), paused on hover or focus.
- **Room:** the photo grows from a small tilted stamp to the full width.
- **Fees:** a slip built by the scene script from each package's name and price sticks beside the list and flips over to the package being read.
- **Footer:** a raking light crosses the pressed word.

With reduced motion, and in browsers without CSS scroll-driven animations (Firefox today), `data-8b-live` is not set: the entrances, the scroll scenes and the smooth wheel are off and scrolling is the browser's own. Sheets read in full, the tree stands finished in normal flow with its lines, the pressed words rest at a fixed depth, the fees are a plain list with no turning slip and the letters wrap into a grid. Tab and button hovers still run. If a scene's script throws, the kit logs an error and switches off that scene's styles, so only its section stays static.

## Do's and Don'ts

- Do keep the black desk and the four paper tints; never put a coloured gradient or a bright accent on them.
- Do keep corners square except the outer corners of tabs.
- Do keep Playwrite US Trad for notes and pressed words only.
- Do cut new photos with the stamp edge, and keep the opening snapshots and the portraits grey.
- Don't add drop shadows to sheets, glass cards, stock icons or round avatars.
- Don't add a second display face or lowercase headings; headings stay uppercase and tight.
- Do keep chart entries in the order the section script and the CSS read: client first, then two parents per entry.
- Don't add other scroll effects over the page's own.
