> # Client Refactoring!
> Revite is currently being deprecated and replaced with a Solid.js client, for more information see https://github.com/revoltchat/revoltchat-solid-client-monorepo/issues/14 with information on how to contribute for the time being.

# Finding Issues

You can find issues using the main project board, here are some categories you should look at in-order:
1. If you are new to the code base or are looking for issues we really need help with, look at ["What can I help with?"](https://github.com/orgs/revoltchat/projects/3/views/11)
2. Issue Board ["Free Issues"](https://github.com/orgs/revoltchat/projects/3/views/1): issues that anyone can pick up and are generally free to work on.
3. Issue Board ["Todo"](https://github.com/orgs/revoltchat/projects/3/views/1): these are issues that are probably fine to pick up, but please ask first since a lot of these tend to be complicated and potentially already planned.
4. Working on new issues and fixes: ideally you should run new features by us, most fixes are probably going to be alright though, we wouldn't want to reject any PRs that we don't deem suitable after work has already been done. If it's a fix, make sure to make an issue for it first, if it's a new feature, it may be better suited in [Feature Suggestions](https://github.com/revoltchat/revolt/discussions/categories/feature-suggestions).

Any issues marked with "Future Work" or with a milestone greater than the current milestone are out of bounds and should not be worked on since it's likely that the team already has a plan in place, any work you may do may conflict with prior ideas, and your work may potentially be rejected if it does fit the criteria exactly. In general, these issues are just postponed to reduce long term technical debt, i.e. allow current issues to be handled.

# Working on Issues

Be sure to:
- Follow the contributing guidelines below.
- Notify us when you're working on an issue, either by leaving a comment (you don't necessarily need to be assigned to an issue) or if you forget, be sure to link your PR back to the original issue by including "Fixes \#1" in your PR to ensure we keep track of this stuff.

# Contributing

- Commit using [Conventional Commit style](https://www.conventionalcommits.org/en/v1.0.0-beta.2/).
- Use `prettier` in relevant repositories using Typescript, use `cargo fmt` in those using Rust.
  **Note:** PRs should only format files that have been changed to avoid conflicts.
- Try to keep each PR bound to a single feature or change, multiple bug fixes may be fine in some cases.
  This is to avoid your PR getting stuck due to parts of it having conflicts or other issues.

### Contributing Source Translations

You may have to add or modify source translations to achieve something in the client, to modify source translations:
- PR your translations to the [translations repository](https://github.com/revoltchat/translations).
- Use these translations in your local client, but do not commit changes to the `external/locale` submodule as to avoid conflicts with other PRs.
- Language definitions will be updated accordingly after merge.

# Merging Pull Requests

To keep commit history nice and tidy, always use [Conventional Commit style](https://www.conventionalcommits.org/en/v1.0.0-beta.2/) for any merge commit messages. And where possible:
1. `Squash and Merge` for bug fixes / small features, especially if the fix has multiple iterations, [example](https://github.com/revoltchat/revite/pull/492), or if the commits don't follow conventional commit style.

Beyond this point you should usually check with a maintainer on how to merge, (drop a message in the "Ready to merge" channel), and should only proceed with the following if the commits follow [Conventional Commit style](https://www.conventionalcommits.org/en/v1.0.0-beta.2/):

2. Prefer to `Rebase and Merge` where possible.
3. Create a merge request with commit message similar to `chore: merge something from x (#1)`.

# Triage

If you are part of the triage team, or are interested in triage, the [full guide is available here](https://github.com/orgs/revoltchat/teams/triage-team/discussions/1).
