# AplikasiLansia
## Design tooling

The design workflow uses [Impeccable](https://impeccable.style), installed per project under `.claude/`.

Install or reinstall it with a pinned version, not the latest:

```sh
npx impeccable@4.7.0 install
```

When the installer asks where to install, choose **project**.

- The install writes design-check hooks to `.claude/settings.local.json`. That file is gitignored so the hooks never reach other contributors.
- The engine binary in `.claude/skills/impeccable/scripts/bin/` is also gitignored. On first use, the launcher downloads it from the project's GitHub releases and checks it against a SHA-256 checksum.
- Telemetry is switched off for this project in `.impeccable/config.json`.
- Do not run `impeccable live-server` on pages that load third-party scripts. It starts Claude without permission prompts, and any script on the page can read its access token.
