# Renovate Bot presets for OMG Network

## Wrapping

Presets for wrapping projects with renovate

If you have a source package (e.g. a docker base image), this preset allows you to pull through the changelog into your local project wrapping it

## Usage

In `renovate.json`, this can be referenced like:

```
{
  "extends": [
    "local>omgnetwork/.github:renovate/wrap-packagename(argoproj/argocd)"
  ]
}
```

This configures that specific package dependency to have semantic commits of fix/feat (instead of chore), and propagates changelogs from the dependency.
