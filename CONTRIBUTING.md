# contributing

thank you for reading this far. the short version:

- **open an issue first** for anything bigger than a typo. the roadmap issues in each
  repository say what i would take gladly; the labels `good first issue` and
  `help wanted` mean exactly that.
- **keep the constraints**: python 3.10+, standard library only, public endpoints, no
  api keys. a dependency needs a very good reason, a paid data source has none.
- **tests run offline**: `python -m pytest -q` must pass without a network. anything
  that talks to a chain goes into `tests/test_live.py` behind the `*_LIVE=1` flag.
- **lint**: `ruff check .` with the settings in `pyproject.toml`. `pre-commit install`
  runs it for you.
- **data has a contract**: files under `data/` are read by other people. columns are
  only ever appended; see the repository's own CONTRIBUTING.md where it exists.
- **labels and addresses need a source**: a block explorer tag, an official page, an
  announcement. "everyone knows" is not a source.
- **commits**: small, one topic each, lowercase message that says what changed and why.
  sign them if you can; it is not required.

pull requests get a reply within a few days. if i do not merge something it is usually
because it adds a dependency, a key, or a call.
