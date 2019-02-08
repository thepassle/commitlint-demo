# Commitlint demo

I've been thinking of configuring commitlint for our d20 app. Commitlint is a linter for commit messages that has a very small impact, with great results. It's not a framework, it doesn't force anything on you, it just holds your hand in writing nice commit messages.

The only thing that is required from you is following the following conventions. You still git add/commit/push like normally.

```sh
git add .
git commit -m "docs: add commitlint demo"
git push
```

## Conventional commits

### Types:

- `feat`: when developing a new feature
- `fix`: bug fixes
- `docs`: documentation only changes
- `style`: style only changes
- `refactor`: code changes thats neither a bugfix or a feature add
- `perf`: performance improvement
- `test`:  add missing tests or correcting existing ones
- `build`: anything that affects the build
- `chore`: anything that doesnt involve code
- `revert`: revert previous commit

### Examples:

`type(scope?): subject  #scope is optional`

- `feat(block-debtor): add block debtor dialog`
- `feat: implement button`
- `fix(dialog-bug): reset dialog after closing`
- `docs: update changelog`
- `style: add breakpoint on dialog for mobile`
- `refactor(block-debtor): use async/await for api calls`
- `perf: -`
- `test: dialog shows correct info`
- `build: retrigger/whatever`
- `chore: add commitlint`
- `revert: revert <hash>`
