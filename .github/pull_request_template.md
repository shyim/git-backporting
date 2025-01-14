**Thank you for submitting this pull request**

fix _(please add the issue ID if it exists)_

### Referenced pull requests

<!-- Add URLs of all referenced pull requests if they exist. This is only required when making
changes that span multiple kiegroup repositories and depend on each other. -->
<!-- Example:
- https://github.com/kiegroup/droolsjbpm-build-bootstrap/pull/1234
- https://github.com/kiegroup/drools/pull/3000
- https://github.com/kiegroup/optaplanner/pull/899
- etc.
-->

### Checklist
- [ ] Tests added if applicable.
- [ ] Documentation updated if applicable.

> **Note:** `dist/cli/index.js` and `dist/gha/index.js` are automatically generated by git hooks and gh workflows.

<details>
<summary>
First time here?
</summary>

This project follows [git conventional commits](https://gist.github.com/qoomon/5dfcdf8eec66a051ecd85625518cfd13) pattern, therefore the commits should have the following format:

```
<type>(<optional scope>): <subject>
empty separator line
<optional body>
empty separator line
<optional footer>
```

Where the type must be one of `[build, chore, ci, docs, feat, fix, perf, refactor, revert, style, test]`

> **NOTE**: if you are still in a `work in progress` branch and you want to push your changes remotely, consider adding `--no-verify` for both `commit` and `push`, e.g., `git push origin <feat-branch> --no-verify` - this could become useful to push changes where there are still tests failures. Once the pull request is ready, please `amend` the commit and force-push it to keep following the adopted git commit standard. 

</details>

<details>
<summary>
How to prepare for a new release?
</summary>

There is no need to manually update `package.json` version and `CHANGELOG.md` information. This process has been automated in [Prepare Release](./workflows/prepare-release.yml) *Github* workflow.

Therefore whenever enough changes are merged into the `main` branch, one of the maintainers will trigger this workflow that will automatically update `version` and `changelog` based on the commits on the git tree.

More details can be found in [package release](https://github.com/kiegroup/git-backporting/blob/main/README.md#package-release) section of the README.
</details>