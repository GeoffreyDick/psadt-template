# psadt-template

## Creating a Release

* Ensure local repo is up-to-date with `git pull`
* Increment `$appScriptVersion` in `.\Unpackaged\Deploy-Application.ps1` appropriately
* Make other changes and commit as needed
* Push commits to GitHub with `git push`
* Tag latest commit with `git tag vX.X.X`, replacing `X.X.X` with the `$appScriptVersion`
* Push tag to GitHub with `git push --tags`. This will trigger a GitHub Action to create a release and build your `.intunewin` file which can be found at [Contribution guidelines for this project](docs/CONTRIBUTING.md)