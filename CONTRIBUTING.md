# Contributing

Thanks for taking the time to contribute! This is a small playground repository, and
issues and pull requests are welcome.

## Forking

1. Fork the repository on GitHub.
2. Clone your fork and add the upstream repository as a remote:

   ```sh
   git clone https://github.com/<your-user>/superagent-demo.git
   cd superagent-demo
   git remote add upstream https://github.com/hachiwave-wh/superagent-demo.git
   ```

3. Sync your fork before starting work:

   ```sh
   git fetch upstream
   git switch main
   git merge --ff-only upstream/main
   ```

## Branching

Create a short, descriptive branch from an up-to-date `main`:

```sh
git switch -c docs/contributing-guide
```

Use a prefix that matches the change, such as `docs/…` for documentation, `fix/…`
for bug fixes, and `feature/…` for new functionality. Keep each branch focused on a
single change, and never commit directly to `main`.

## Commit style

- Write a short, lowercase, imperative subject line, for example
  `add contributing guide`.
- Keep the subject under 72 characters and leave off the trailing period.
- Add a blank line and a body explaining what changed and why when the subject alone
  is not enough.
- Keep commits small and logical, and reference related issues in the body, for
  example `Refs #123`.

## Pull requests

- Open pull requests against `main`.
- Describe what the change does and why, and link any related issues.
- Keep the diff focused; unrelated changes belong in a separate pull request.
- Update documentation and tests when behavior changes.
- Make sure any configured checks pass before requesting review.
- Push follow-up commits to the same branch to address review feedback.
- A maintainer merges the pull request once it is approved; do not merge your own.
