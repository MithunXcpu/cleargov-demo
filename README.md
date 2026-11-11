# Rochester Hills budget transparency demo

An independent Solutions Engineer demo by Mithun Manjunatha. Four static HTML pages walk through a short presentation about the public Rochester Hills, Michigan transparency portal.

This is a personal prototype for interview practice. It is not an official ClearGov or Gravity product, it is not affiliated with the City of Rochester Hills, and it does not host or control the live portal.

Figures on the pages are demo talking points. The slides cite [rochesterhills.opendata.report](https://rochesterhills.opendata.report) (2025 Amended / 2026 Adopted) as their source.

## How to open it

No install or build. Open `index.html` in a browser. The pages link to each other with relative paths, so a local file open is enough.

From this folder you can also serve them:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000/`.

The pages load Inter from Google Fonts when you are online and fall back to the system font otherwise.

## Pages

| Page | What it shows |
| --- | --- |
| [`index.html`](index.html) | Hub. Cards open the click path, the slides, the public portal (new tab), and the takeaway. A note under the cards describes the suggested demo order. |
| [`clickpath.html`](clickpath.html) | Presenter guide for a ~35 minute walkthrough. Twelve steps sit in four phases (Tell, Show, Tell, Q&A). Each step has a talk track; some add portal links, numbers to mention, or likely questions. A start/pause/reset timer, progress, and Previous/Next buttons are included. Arrow Down or `J` advances a step, Arrow Up or `K` goes back, and `R` opens a data sidebar. |
| [`slides.html`](slides.html) | Five-slide deck: title, agenda, key budget figures, a cue to switch to the live portal, and a close. Arrow keys or the on-screen buttons move between slides (Space also goes forward). `N` toggles speaker notes. |
| [`takeaway.html`](takeaway.html) | Leave-behind reference. Static sections cover the Water & Sewer Operating Fund, revenue and expenditure line items, the July 2025 rate table, all nine capital programs in the six-year plan, and three value points. A sticky nav jumps to each section. |

The hub’s suggested flow is: keep the click path on a second screen, share the slides, switch to the public portal when the deck cues the live demo, then return to the slides and share the takeaway.
