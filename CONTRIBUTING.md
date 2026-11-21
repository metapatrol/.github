# Contributing

Thanks for taking the time.

This is the default for metapatrol repositories that do not have a
`CONTRIBUTING.md` of their own. Where a project has one, that one applies.

## How this repository works

The project is developed in a private Forgejo instance and push-mirrored here.
Issues and pull requests opened on GitHub are carried into Forgejo by
[forgejo-github-bridge](https://github.com/metapatrol/forgejo-github-bridge), where the maintainers work, and everything
they say comes back here. Releases are cut in Forgejo and published here. From
your side it is an ordinary GitHub project; a bot account posts the
maintainers' replies, naming who wrote them.

## Issues

Open an issue for bugs, questions and ideas. Please include the version, what
you expected, what happened, and the relevant output — with tokens and keys
removed.

## Pull requests

- Target **`develop`**. Pull requests against other branches are not picked up.
- Use [Conventional Commits](https://www.conventionalcommits.org/): `feat:` and
  `fix:` make a release, `chore:`, `ci:`, `docs:` and `build:` do not.
  Versions and the changelog are derived from them.
- Run the project's checks before pushing; its README or `Makefile` names them.
- Explain the why in the commit body when the diff does not.
- If you change CI configuration (`.forgejo/`, `.github/`), say why in the
  description. Such pull requests are read with particular care before any
  workflow of theirs runs.

### What happens after you open one

1. Your branch is imported into the maintainers' Forgejo. CI runs there once a
   maintainer has read your changes and approved the run.
2. Review comments appear on your pull request, posted by the bot and
   attributed to the maintainer.
3. When it is merged, the bot says so; your authorship is kept.

## Security

Please do not report security problems in public issues. See
[SECURITY.md](SECURITY.md).

## License

By contributing you agree that your contributions are licensed under the
project's licence (`LICENSE` in the repository).
