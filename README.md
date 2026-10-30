# gh-coverage

A [GitHub CLI](https://cli.github.com/) extension that downloads the coverage
report of a pull request, unzips it and opens it in your browser.

```
gh coverage <PR NUMBER> -R <REPO NAME (org/repo)>
```

## Install

```
gh extension install MaciejKaszynski/gh-coverage
```

## Configs

```
gh coverage <PR-NUMBER> [options]
  -R, --repo OWNER/REPO   Repository (default: current repo)
  -o, --output-dir DIR    Base dir for <PR>-<RUN>-coverage (default: /tmp)
  -i, --index PATH        File to open, relative to the extracted dir
                          (default: coverage_linux/index.html)
  -a, --artifact NAME     Artifact name on the pipline (default: coverage-html)
```
