# t3code-bench-wachi

Replayed pull requests from [pingdotgg/t3code](https://github.com/pingdotgg/t3code) (MIT License), used as a code-review benchmark.

Each case has two branches: `replay/pr-<n>/base` holds the tree of the original PR's base, and `replay/pr-<n>/head` holds the tree of the earliest PR commit that a review bot commented on, with the base as its parent. Each replay PR therefore shows the same diff the bots reviewed. The original commit shas are in each commit message and PR body.

GitHub Actions is disabled in this repository and no secrets are configured. Wachiman runs locally on the owner's machine and its findings are posted as PR comments with `gh`.

The method and the reference bot threads are in [niway-dev/wachiman-benchmarks](https://github.com/niway-dev/wachiman-benchmarks), under `t3code/replays/`.

The t3code code in the replay branches is copyright its authors and is redistributed under its MIT License, which is included in each tree.
