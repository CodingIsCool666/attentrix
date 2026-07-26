# SignalRoom

SignalRoom gives a presenter a calm, second-screen view of visible audience
cues during a Zoom session. It separates highly engaged, following, confused,
and attention-drift signals, then summarizes the room into a suggested
presenter response.

SignalRoom runs locally on the presenter's Windows computer. The public beta
does not request microphone access, retain meeting video, upload participant
frames, or create identity profiles.

## Download

The current release is
[SignalRoom 0.1.0-beta.1](https://github.com/CodingIsCool666/signalroom/releases/tag/v0.1.0-beta.1)
for 64-bit Windows 10 and Windows 11.

- Use the installer for the normal setup experience.
- Use the portable ZIP when you cannot install applications.
- Verify the downloaded file against `SHA256SUMS.txt`.

The beta is not code-signed, so Windows may display an unrecognized-app
warning. Confirm the published checksum before continuing.

## Use

1. Open Zoom and switch to Gallery View.
2. Open SignalRoom and select **Start a session**.
3. Read and accept the responsible-use notice.
4. Select the Zoom window in the browser sharing menu.
5. Frame the visible participant gallery and start the live view.
6. Keep SignalRoom on a second monitor or beside Zoom.

The browser asks for screen-sharing permission for every session. SignalRoom
cannot select the Zoom window automatically.

## Interpretation

SignalRoom estimates visible behavioral cues. It does not know a participant's
thoughts, intent, effort, understanding, or learning outcome.

- **Highly engaged:** especially strong visible attention cues.
- **Following:** steady visible attention cues.
- **Confused:** uncertainty cues while oriented to the session.
- **Attention drift:** sustained cues that attention may be elsewhere.

Use the output as a prompt to observe, ask, or adjust. Do not use SignalRoom
for grading, discipline, attendance, employment decisions, or covert
surveillance.

## Evidence

On one frozen three-person Zoom holdout with recording-level phase labels, the
selected participant policy reached person-level macro-F1 `0.751` and accuracy
`0.778`. Room-level presenter-action macro-F1 was `0.851`.

The selected compute profile preserved presenter outputs exactly across eight
final paired replay trials while reducing backend analysis time by a
source-mean `11.41%`, with a 95% bootstrap interval of `8.11%` to `14.71%`.

These results are local research evidence, not a universal classroom accuracy
claim.

## Scope

Version 0.1 analyzes one visible Zoom Gallery View with up to 49 rendered
participants. It cannot analyze participants on another gallery page, cameras
that are off, or faces that are fully hidden. Eye gaze is not included in this
release.

This repository currently hosts public beta packages and user documentation.
The research source and participant data remain private during beta testing.

Read [PRIVACY.md](PRIVACY.md) before using SignalRoom with participants.
