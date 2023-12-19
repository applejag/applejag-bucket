# Applejag Scoop Bucket

[![Tests](https://github.com/applejag/applejag-bucket/actions/workflows/ci.yml/badge.svg)](https://github.com/applejag/applejag-bucket/actions/workflows/ci.yml) [![Excavator](https://github.com/applejag/applejag-bucket/actions/workflows/excavator.yml/badge.svg)](https://github.com/applejag/applejag-bucket/actions/workflows/excavator.yml)

[Scoop](https://scoop.sh) bucket for [Applejag](https://github.com/applejag)'s
projects, such as [kubectl-klock](https://github.com/applejag/kubectl-klock).

## How do I use this template?

4. Document the bucket in `README.md`.
5. Replace the placeholder repository string in `bin/auto-pr.ps1`.
6. Create new manifests by copying `bucket/app-name.json.template` to
   `bucket/<app-name>.json`.
7. Commit and push changes.
8. If you'd like your bucket to be indexed on `https://scoop.sh`, add the
   topic `scoop-bucket` to your repository.

## How do I install these manifests?

After manifests have been committed and pushed, run the following:

```pwsh
scoop bucket add applejag https://github.com/applejag/applejag-bucket

# https://github.com/applejag/kubectl-klock
scoop install applejag/kubectl-klock
```

## How do I contribute new manifests?

To make a new manifest contribution, please read the [Contributing
Guide](https://github.com/ScoopInstaller/.github/blob/main/.github/CONTRIBUTING.md)
and [App Manifests](https://github.com/ScoopInstaller/Scoop/wiki/App-Manifests)
wiki page.
