# Wellnite Renovate Config - `release` Preset

This is the shared Renovate configuration used across Wellnite repositories.

## Usage

To adopt this config in your repository, extend it in your local `renovate.json`:

```json
{
  "extends": ["github>wellnite-org/renovate-config#release"]
}
```

### Key Features

- ✅ Smart defaults for all repositories
- ✅ Safe auto-merge for devDependencies, GitHub Actions, and Alpine patches
- ✅ Vulnerability auto-remediation via OSV alerts
- ✅ Semantic commits for clean history and changelogs
- ✅ Changelog links included in every PR
- ✅ Sane concurrency and PR limits to avoid noise

### Maintainer Guidance

- Production dependencies are not auto-approved or merged — manual review required.
- Vulnerabilities (via osv.dev) are auto-merged if fixable.
- For updates outside the scope of this config, override locally in renovate.json.

## Contribution
PRs welcome! Please include a description if adding a new ```packageRule```.
