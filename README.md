# Historical Advisory Committee

Source data for [Historical Advisory Committee](https://history.state.gov/about/hac)

## Build

1. Single `xar` file: The `collection.xconf` will only contain the index, not any triggers!
    ```shell
    ant
    ```

## Release

Releases for this data package are automated. Any commit to the `master`` branch will trigger the release automation.

All commit message must conform to [Angular Commit Message Conventions](https://github.com/angular/angular.js/blob/master/DEVELOPERS.md#-git-commit-guidelines) to determine semantic versioning of releases, please adhere to these conventions, like so:

| Commit message  | Release type |
|-----------------|--------------|
| `fix(pencil): stop graphite breaking when too much pressure applied` | Patch Release |
| `feat(pencil): add 'graphiteWidth' option` | ~~Minor~~ Feature Release |
| `perf(pencil): remove graphiteWidth option`<br/><br/>`BREAKING CHANGE: The graphiteWidth option has been removed.`<br/>`The default graphite width of 10mm is always used for performance reasons.` | ~~Major~~ Breaking Release |

When opening PRs commit messages are checked using commitlint. 