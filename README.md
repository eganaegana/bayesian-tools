# Philosophy Teaching Tools

Interactive web-based tools for exploring concepts in epistemology and social philosophy. Developed for use in undergraduate and graduate philosophy courses at Rutgers University.

All tools are standalone HTML files with no external dependencies. Open any `.html` file in a browser to use it, or visit the [index page](index.html) for a categorized overview.

## Tools

### General Bayesian Tools

- **[Eikosogram Generator](juan-eikosogram-tool.html)** — Create and explore eikosograms (area-proportional probability diagrams). From Juan Comesana.
- **[The Importance of Base Rates](base-rates.html)** — See how prior probabilities shape the interpretation of evidence.
- **[Bayesian Conditional Probability Explorer](bayes-cp-explorer.html)** — Explore how priors and likelihoods determine posteriors, with step-by-step Bayes' theorem.

### Testimony

- **[Testimony & Speaker Reliability](testimony-tool.html)** — Model how sincerity, competence, and priors shape what we learn from what others say.

### Schelling on Segregation

- **[Schelling's Segregation Model](schelling-simulation.html)** — See how mild individual preferences can produce dramatic large-scale segregation.
- **[Schelling's Dining Hall Segregation](schelling-dining-hall.html)** — A dining hall simulation of Schelling's segregation dynamics.

### Scientific Communities

- **[Division of Cognitive Labor](kitcher-labor-explorer.html)** — Explore the relationship between problem-solving methods and theory choice in scientific communities. Based on Kitcher (1990).
  - [Student guide](guides/kitcher-labor-explorer-guide.docx)
- **[Zollman Effect Interactive Tool](zollman-simulation.html)** — Explore how network structure affects the spread of knowledge in scientific communities. Based on Zollman (2007, 2010).
  - [Student guide](guides/zollman-simulation-guide.docx)
- **[Selective-Sharing Propagandist Model](propagandist-simulation-selective-sharing.html)** — Simulate how selective sharing of evidence by a propagandist can distort community beliefs. Based on O'Connor & Weatherall (2018).
  - [Student guide](guides/propagandist-selective-sharing-guide.docx)
- **[Biased-Production Propagandist Model](propagandist-biased-production.html)** — Simulate how a propagandist running their own experiments and selectively publishing results can influence policymakers. Based on O'Connor & Weatherall (2018).
  - [Student guide](guides/propagandist-biased-production-guide.docx)
- **[Journalists as Unwitting Propagandists Model](journalist-fairness-simulation.html)** — Explore how journalistic practices like "fair" balanced reporting can slow policymakers from reaching accurate beliefs. Based on O'Connor & Weatherall (2018).
  - [Student guide](guides/journalist-fairness-guide.docx)

## Student Guides

The [guides/](guides/) folder contains `.docx` walkthrough documents for several of the tools. Each guide explains what the tool does, describes its key parameters, and includes a structured exploration activity (~20 minutes) with discussion questions. These are designed to be distributed to students alongside the tools.

## Technical Details

Each tool is a single self-contained HTML file with embedded JavaScript and CSS. No build step, no server, no dependencies. The simulations use seeded pseudorandom number generators (Mulberry32) for reproducibility, and Bayesian updating in odds form with likelihood ratios.
