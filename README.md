# Site generator speed entry

[![make.fun · site-generator-speed-01-run-20261122](https://make.fun/badge/site-generator-speed-01-run-20261122.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![rank](https://make.fun/badge/site-generator-speed-01-run-20261122/benjaminkincses/site-generator-speed/rank.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)
[![reward](https://make.fun/badge/site-generator-speed-01-run-20261122/benjaminkincses/site-generator-speed/reward.svg)](https://make.fun/bounty/site-generator-speed-01-run-20261122?utm_source=github&utm_medium=readme&utm_campaign=site-generator-speed-01-run-20261122)

Builds one static site per input case. Run with Node.js 22.18 or later.

    MAKEFUN_INPUT_DIR=/path/to/input MAKEFUN_OUTPUT_DIR=/path/to/output node main.ts

The input directory contains cases.json and the output directory must exist. See make.fun's site-generator-speed-01-run-20261122 competition kit for the published practice inputs and expected answers.

This entry adapts the competition's MIT-licensed makefun-site 1.0.0 reference. The Markdown renderer escapes contiguous literal text in one pass. The template renderer caches leaf partials within one build when every free variable resolves to the same site-wide binding. Tag names share their normalized spellings and post layouts reuse computed card fields. No input or output is cached across sites.

REFERENCE-LICENSE and NOTICE retain upstream attribution for makefun-site, metalsmith and marked.
