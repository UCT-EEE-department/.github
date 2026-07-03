# .github

Organisation-level GitHub configuration for the [UCT Department of Electrical Engineering](https://github.com/uct-eee-department). This is a special repository: GitHub treats several of its files as organisation-wide defaults rather than as ordinary repository content.

## What lives here

- **`profile/README.md`** is the public landing page shown on the organisation's Overview tab to anyone who visits. Edit this to change what the public sees.
- **`CONTRIBUTING.md`** is the default contributing guide. GitHub shows it automatically when someone opens an issue or pull request in any repository that does not supply its own.
- **`SECURITY.md`**, **`CODE_OF_CONDUCT.md`** and the **issue and pull request templates** in `.github/` act as organisation-wide defaults in the same way. All are optional.

Any repository in the organisation can override a default simply by providing its own copy of the file.

## What does not live here

This repository is **public**, so it must never contain anything sensitive or members-only.

- The **members-facing landing page** lives in the private `.github-private` repository, at `profile/README.md`. GitHub shows it to signed-in members under the "Member" view of the organisation profile.
- **Internal policy and operational notes** live in the private internal-docs repository.

## Editing

Clone and edit like any other repository:

```zsh
git clone https://github.com/uct-eee-department/.github.git
```

Changes to `profile/README.md` and to the default community health files take effect as soon as they are committed to the default branch. No release or deployment step is needed.

## Maintainers

See the [organisation profile](https://github.com/uct-eee-department) for the current list of administrators.
