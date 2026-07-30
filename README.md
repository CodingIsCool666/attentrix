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
[ATTENTRIX 0.2.0 Beta 1](https://github.com/CodingIsCool666/attentrix/releases/tag/v0.2.0-beta.1)
for 64-bit Windows 10 and Windows 11.

- Use the installer for the normal Windows setup.
- Use the portable ZIP when applications cannot be installed.
- Verify either package against the published `SHA256SUMS.txt`.

This beta is not code-signed. Windows may display an unrecognized-app warning.
Check the SHA-256 value before running the installer:

```text
150cbef841e24c23cd0955b8a14ee83f9983329c928d5a4ea864b833c5935466  ATTENTRIX-Setup-0.2.0-beta.1-x64.exe
80298ba63bde9a4299edee72c7ce59399b132dce53aa7a2dc0eeb90886166b74  ATTENTRIX-Windows-x64-0.2.0-beta.1.zip
```

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
