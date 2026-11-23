# Kodi DramaCool fork — maintenance status

This is an archived-style fork of the older DramaCool Kodi plugin, **not a confirmed working streaming add-on**.

## Current status

- The original Lime installation page is `https://groggyegg.github.io/`. The maintainer's add-on source was blocked by GitHub following a copyright takedown in March 2026.
- This fork identifies as `plugin.video.dramacool` version **3.2.1**; its legacy request module uses the `watchasian.mx` and `dramacool.hr` domains, which are not verified working providers.
- The code now has connection/read timeouts, handles HTTP connection failures, and rejects malformed request paths to avoid hanging Kodi.
- No reliable playback or Kodi-version compatibility has been established. The fork has **not** been repackaged or published as a working release.

## Safe troubleshooting

In Kodi, enable debug logging in **Settings → System → Logging**, reproduce the error, and inspect `kodi.log` for Python import/dependency errors versus DNS, TLS or provider errors. Remove personal tokens or URLs before sharing a log.

If the repository ZIP installs but listings are empty, that is a provider/API problem rather than proof the installer is corrupted.

## Next steps

A maintainable Kodi plugin would require an authorized content source/API, compatible Kodi dependencies, automated tests and a new release package. This repository is not affiliated with KissKH, and an unverified KissKH API cannot be substituted as though it were a compatible service.

Original source attribution and MIT licence remain in [LICENSE](LICENSE).
