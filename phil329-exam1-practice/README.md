# Phil 329 Exam 1 practice page

Two files, no build step:

- `index.html` — the page. Self-contained (all CSS/JS inline, one Google Fonts link).
- `bank.json` — the question pool the page deals from. The page fetches this file on load; if the fetch fails it falls back to a copy embedded in `index.html` (which may be older).

To revise questions: edit `bank.json` and push. Each item is `{id, type: "tf"|"mc"|"fib", topic, tier, stem, ...}`:
- tf: `answer` (true/false), `fix` (shown when false)
- mc: `options` (4 strings), `answer` (index of the correct one; options are shuffled on the page)
- fib: `answer` (model answer), `accept` (list of phrases; a student's answer counts if it contains any of them)

Topics and per-deal counts are fixed in `index.html` (`TOPICS` near the top of the script): descartes 3, elisabeth 3, ryle 3, smart 3, functionalism 4, qualia 3, varieties 2, synoptic 3.

Serve with GitHub Pages (Settings → Pages → deploy from branch, root). Opening `index.html` from disk works too, but then `bank.json` isn't fetched (browsers block file:// fetches) and the embedded copy is used.
