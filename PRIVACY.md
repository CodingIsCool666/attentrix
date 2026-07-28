# SignalRoom Privacy

Last reviewed: July 28, 2026

SignalRoom processes the Zoom window selected by the presenter on that
presenter's Windows computer.

## Data Used

SignalRoom receives frames through the browser's screen-sharing prompt. It
extracts temporary face locations, facial landmarks, head and posture cues,
motion measurements, and model confidence values.

SignalRoom does not request or capture microphone audio.

## Data Stored

SignalRoom stores a local session summary and timeline. These files may
contain timestamps, temporary participant keys, estimated states, confidence
values, visible-face counts, bounding-box locations, room percentages,
presenter actions, and local performance diagnostics.

Live-session video is not retained unless the user explicitly turns on local
replay before starting the session. Replay is video-only and off by default.
The option resets to off for every new session.

When the user chooses an MP4 or WebM recording for background analysis, that
recording is copied into the current Windows user's local SignalRoom data
folder. Any audio already present in an uploaded recording remains part of the
local source file but is not analyzed.

SignalRoom does not create participant identity profiles.

## Data Sharing

SignalRoom does not upload meeting frames, reports, or participant data to a
SignalRoom cloud service. An exported report leaves the device only when the
user chooses to share it.

## Retention

Reports, optional replay videos, and uploaded recordings remain in the current
Windows user's local SignalRoom application-data folder until that user
deletes them. Uninstalling SignalRoom does not automatically delete prior
session data.

## Responsible Use

Tell participants that SignalRoom is being used and obtain appropriate consent.
The states are uncertain behavioral estimates. Do not use them as evidence of
a person's intent, ability, character, or learning outcome. Do not use
SignalRoom for grading, discipline, attendance, employment decisions, or
covert surveillance.

Eye gaze is not enabled in version 0.1. A future optional gaze module would
receive a new version number and an updated privacy notice.
