# SignalRoom Privacy

Last reviewed: July 26, 2026

SignalRoom processes the Zoom window selected by the presenter on that
presenter's Windows computer.

## Data Used

SignalRoom receives frames through the browser's screen-sharing prompt. It
extracts temporary face locations, facial landmarks, head and posture cues,
motion measurements, and model confidence values.

SignalRoom does not request or capture microphone audio.

## Data Stored

The public beta stores a local session summary and timeline. These files may
contain timestamps, temporary participant keys, estimated states, confidence
values, visible-face counts, bounding-box locations, room percentages,
presenter actions, and local performance diagnostics.

The public beta does not retain meeting video. It does not create participant
identity profiles.

## Data Sharing

SignalRoom does not upload meeting frames, reports, or participant data to a
SignalRoom cloud service. An exported report leaves the device only when the
user chooses to share it.

## Retention

Reports remain in the current Windows user's local SignalRoom application-data
folder until that user deletes them. Uninstalling SignalRoom does not
automatically delete prior reports.

## Responsible Use

Tell participants that SignalRoom is being used and obtain appropriate consent.
The states are uncertain behavioral estimates. Do not use them as evidence of
a person's intent, ability, character, or learning outcome. Do not use
SignalRoom for grading, discipline, attendance, employment decisions, or
covert surveillance.

Eye gaze is not enabled in version 0.1. A future optional gaze module would
receive a new version number and an updated privacy notice.
