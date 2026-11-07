# Phil 329 Exam 2 practice page

Same setup as the Exam 1 page: `index.html` (self-contained, with an embedded fallback copy of the pool) + `bank.json` (the pool the page fetches on load). Serve with GitHub Pages, e.g. as `phil329-exam2-practice/` in bayesian-tools.

- `bank.json` = the 148 published Exam 1 (Unit 1A) items + the new-material items (`Phil329_Exam2_newmaterial_bank.json` one folder up is the full source, with tiers).
- Modes: "Like the real exam" = 8 Unit 1A items (one per Exam 1 topic) + 16 new; "New material only" = 24 new. Per-topic counts are in `NEW` near the top of the script.
- Format per deal is always 8 T/F, 8 MC, 8 fill-in (64 points).
- Fix vs the Exam 1 page: the fill-in matcher no longer accepts a student answer just because it's a substring of an accept phrase (that let answers like "same" or "true" through).
- Argument sets: entries with `type: "group"` (topic `arguments`) hold four sample arguments (`arguments: [{premises, conclusion}]`); ordinary tf/mc/fib items with `group: "<id>"` ask about them. A deal's arguments section = one random set with up to two of its questions (+ standalone items if the topic's quota is higher). Because a set may lack a needed format, a deal is occasionally 9/8/7 instead of exactly 8/8/8.
