# ATTENTRIX

ATTENTRIX gives presenters a second-screen view of visible audience cues during
Zoom sessions. It tracks highly engaged, following, confused, and
attention-drift signals for each visible participant, then summarizes the room
into a suggested response.

The application runs locally on the presenter's computer. It does not request
microphone access, upload meeting frames, or create participant identity
profiles.

## Download

The current public beta is
[ATTENTRIX 0.2.0 Beta 2](https://github.com/CodingIsCool666/attentrix/releases/tag/v0.2.0-beta.2)
for 64-bit Windows 10 and Windows 11.

- Use the installer for the normal Windows setup.
- Use the portable ZIP when applications cannot be installed.
- Verify either package against the published `SHA256SUMS.txt`.

This beta is not code-signed. Windows may display an unrecognized-app warning.
Check the SHA-256 value before running the installer:

```text
5c34d934125829b6eae5c7fc57cfd87e616d1b63ac7c17a9ba05a80cccc244af  ATTENTRIX-Setup-0.2.0-beta.2-x64.exe
ebf47faf3f68ee3dcc36fd388cfcc40cfb1a6337d3e93a1183e7553493556b69  ATTENTRIX-Windows-x64-0.2.0-beta.2.zip
```

The public
[verification record](https://github.com/CodingIsCool666/attentrix/releases/download/v0.2.0-beta.2/verification_evidence.json)
binds the tested Windows workflows to those exact hashes. Publication also
retrieved the installer, portable archive, checksum file, manifest, and
verification record anonymously and matched every remote size and SHA-256.

Beta 2 replaces Beta 1, which omitted the `narwhals.stable.v2` runtime
dependency required by scikit-learn during Zoom analysis. Beta 2 was built from
clean source commit `c8e923a6b9054a057b3d33eb40a1beefe0103fe5` and includes
the official ATTENTRIX emblem across the application and Windows packages.

## Live Sessions

1. Open Zoom and switch to Gallery View.
2. Open ATTENTRIX and select **Start a session**.
3. Read and accept the responsible-use notice.
4. Select the Zoom window in the browser sharing menu.
5. Frame the visible gallery and begin analysis.
6. Keep ATTENTRIX beside Zoom or on a second monitor.

The browser asks for screen-sharing permission for each session. ATTENTRIX
cannot select the Zoom window automatically.

## Saved Meetings And Replay

ATTENTRIX can analyze an MP4 or WebM meeting in the background and replay the
video beside its synchronized room timeline. A live session can also be saved
for replay when the presenter enables the option before recording. Live replay
is off by default.

Selected and recorded videos remain in the current user's local ATTENTRIX data
folder. The model does not analyze audio.

## Interpretation

- **Highly engaged:** especially strong visible attention cues.
- **Following:** steady visible attention cues.
- **Confused:** uncertainty cues while oriented to the session.
- **Attention drift:** sustained cues that attention may be elsewhere.

These are uncertain behavioral estimates. They do not reveal a person's
thoughts, intent, effort, understanding, or learning outcome. Do not use
ATTENTRIX for grading, discipline, attendance, employment decisions, or covert
surveillance.

## Current Evidence

On one frozen three-person Zoom holdout with broad phase labels, the selected
participant policy reached person-level macro-F1 `0.751` and accuracy `0.778`.
Room-level presenter-action macro-F1 was `0.851`.

The selected compute profile preserved presenter outputs exactly across eight
paired replay trials while reducing backend analysis time by a source-mean
`11.41%`, with a 95% bootstrap interval of `8.11%` to `14.71%`.

These are local research results, not a universal classroom accuracy claim.

## Scope

Version 0.2 analyzes one visible Zoom Gallery View with up to 49 rendered
participants. It cannot analyze cameras that are off, fully hidden faces, or
participants on another gallery page. Eye gaze is not included in this release.

This repository contains public beta packages and user documentation only. The
research source, datasets, and participant recordings remain private.

Read [PRIVACY.md](PRIVACY.md) before using ATTENTRIX with participants.
