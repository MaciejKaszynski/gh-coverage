# gh-coverage

A [GitHub CLI](https://cli.github.com/) extension that downloads the coverage
report of a pull request, unzips it and opens it in your browser.

```
gh coverage <PR NUMBER | BRANCH> -R <REPO NAME (org/repo)>
```

Pass a branch name instead of a PR number to get the latest coverage run on
that branch, e.g. `gh coverage main`.

## Install

```
gh extension install MaciejKaszynski/gh-coverage
```

## Configs

```
gh coverage <PR-NUMBER | BRANCH> [options]
  -R, --repo OWNER/REPO   Repository (default: current repo)
  -o, --output-dir DIR    Base dir for <PR|BRANCH>-<RUN>-coverage (default: /tmp)
  -i, --index PATH        File to open, relative to the extracted dir
                          (default: coverage_linux/index.html)
  -a, --artifact NAME     Artifact name on the pipline (default: coverage-html)
  -w, --workflow NAME     Only consider workflow runs with this name (default: PR)
```
