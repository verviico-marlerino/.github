# Marlerino · Shared GitHub files

Organization profile and shared workflow references for `verviico-marlerino`.

- `profile/README.md`: public studio profile.
- `.github/workflows/ios-build.yml`: **unconfigured legacy template, fail-closed**.
- `.github/workflows/ios-release.yml`: **unconfigured legacy template, fail-closed**.

The active Predictions checks live in [its own workflows](https://github.com/verviico-marlerino/predictions/tree/dev/.github/workflows). [Factory workflow](https://github.com/verviico-marlerino/factory/blob/dev/docs/workflow.md) defines the common process.

The old templates only echoed TODO and could appear green without building or releasing anything. They now stop explicitly on a low-cost runner. They are not production pipelines and must not be presented as completed integration. Configure and verify a real app-local contract before adopting a reusable implementation; use the actual `verviico-marlerino/.github` owner and an immutable reviewed revision, never the obsolete `softloom-studio` reference.

No secrets live in this public repository. App/environment secrets remain isolated. No store upload, deploy or paid native runner is triggered by these templates.
