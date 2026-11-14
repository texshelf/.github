# Contributing to texshelf

Thanks for wanting to help. The fastest way to make texshelf better is to add
a template people need, and that takes one pull request with one file.

## Add or update a template

Templates stay in their author's own repository. The
[registry](https://github.com/texshelf/registry) only holds a manifest that
points at a commit.

If the template is yours:

```console
texshelf new-template my-template   # or add texshelf.toml to an existing one
texshelf publish
```

`publish` checks the folder, then opens a pull request page on the registry
with the manifest filled in.

If the template belongs to someone else, check that its license allows
redistribution, then write the manifest by hand. The
[publishing guide](https://github.com/texshelf/texshelf/blob/main/docs/publishing.md)
walks through it. List the real authors, never yourself.

If you only know of a template that should be here, open a
[template request](https://github.com/texshelf/registry/issues/new/choose).

## Report a problem

| The problem is with | Open the issue in |
| --- | --- |
| The `texshelf` or `typshelf` command | [texshelf](https://github.com/texshelf/texshelf/issues/new/choose) |
| A template that is broken, outdated or mislabeled | [registry](https://github.com/texshelf/registry/issues/new/choose) |
| One of the official starters, such as `article` | [templates](https://github.com/texshelf/templates/issues/new/choose) |
| The website | [web](https://github.com/texshelf/web/issues/new/choose) |

For a security problem, follow [SECURITY.md](SECURITY.md) and do not open a
public issue.

## Change the code

Each repository's README explains how to build and test it. A few habits that
keep review short:

- Open an issue before a large change, so nobody writes code that will not be
  merged.
- Keep a pull request to one change.
- Run the tests and the formatter before you push. CI runs them again.
- Write commit messages that say what changed, in the imperative: "Add
  university filter".

## Review

Juan José reviews pull requests himself, usually within a few days. Template
submissions are merged once CI can fetch, audit and compile them and the
license checks out.

By contributing you agree that your work is released under the license of the
repository you contribute to, and that you follow the
[code of conduct](CODE_OF_CONDUCT.md).
