# Contributing to photon-mosaic

Contributors to photon-mosaic are absolutely encouraged, whether to fix a bug, develop a new feature, or add to the documentation.

## Before you start

Before starting work on a contribution, please check the repository issue tracker to see if there's already an issue describing what you have in mind.

- If there is, add a comment to let others know you're willing to work on it.
- If there isn't, please create a new issue to describe your idea.

We strongly encourage discussing your plans before you start coding—either in the issue itself or on our [Zulip chat](https://neuroinformatics.zulipchat.com/#narrow/channel/500681-photon-mosaic).
This helps avoid duplicated effort and ensures your work aligns with the project's scope and roadmap.

Keep in mind that we often use issues liberally to track development.
Some may be vague or aspirational, serving as reminders for future work rather than tasks ready to be tackled.
There are a few reasons an issue might not be actionable yet:

- It depends on other issues being resolved first.
- It hasn't been clearly scoped. In such cases, helping to clarify the scope or breaking the issue into smaller parts can be a valuable contribution. Maintainers typically lead this process, but you're welcome to participate in the discussion.
- It doesn't currently fit into the roadmap or the maintainers' priorities, meaning we may be unable to commit to timely guidance and prompt code reviews.

If you're unsure whether an issue is ready to work on, just ask!

Some issues may be labelled as `good first issue`.
These are especially suitable if you're new to the project, and we recommend starting there.

## To contribute code

### Creating a development environment

It is recommended to use `conda` to install a development environment. Once you have `conda` installed, the following commands
will create and activate a `conda` environment with the requirements needed
for a development environment:

```sh
conda create -n photon-mosiac-env -c conda-forge python=3.12
conda activate photon-mosiac-env
```

To install a specific project for development, clone the GitHub repository,
and then run

```sh
pip install -e .[dev]
```

Or if using `zsh` (the default on new Apple machines):

```sh
pip install -e '.[dev]'
```

from inside the repository. This will install the package, its dependencies,
and its development dependencies.

### Pull requests

In all cases, please submit code to the main repository via a pull request. The developers recommend, and adhere,
to the following conventions:

- Please submit _draft_ pull requests as early as possible (you can still push to the branch once submitted) to
  allow for discussion.
- One approval of a PR (by a core developer) is enough for it to be merged.
- Unless someone approves the PR with optional comments, the PR is immediately merged by the approving reviewer.
- Please merge via "Squash and Merge" on GitHub to maintain a clean commit history.
- Ask for a review from someone specific if you think they would be a particularly suited reviewer (possibly noting why they are suited on the PR description).
