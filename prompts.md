# Prompt log

## 2026-11-05T14:06:55-05:00 — Append an optional real name

- Goal: Include a person's name in the downloaded photo filename when provided.
- Request: Add an optional Real Name field and append its value after the initials in the filename.
- Computer: `Peters-MacBook-Pro.local`
- Technical context: Share filename formatting between the live preview and download, sanitize name separators, and clear both fields for New photo.

## 2026-11-05T14:05:15-05:00 — Reuse camera access between photos

- Goal: Avoid repeated camera authorization when taking another photo.
- Request: Fix New photo requesting camera permission again.
- Computer: `Peters-MacBook-Pro.local`
- Technical context: Keep the live camera stream after capture, reuse it for New photo and Retake, and release it when leaving the page.

## 2026-11-05T14:03:40-05:00 — Start a new photo

- Goal: Make it easy to take another photo after saving.
- Request: Add a New photo button or equivalent control.
- Computer: `Peters-MacBook-Pro.local`
- Technical context: After a download is requested, offer a reset that clears the initials and captured photo and restarts the camera.

## 2026-11-05T14:01:04-05:00 — Use uppercase initials

- Goal: Keep entered initials and saved filenames uppercase.
- Request: Automatically capitalize initials as they are entered.
- Computer: `Peters-MacBook-Pro.local`
- Technical context: Normalize the input value and use uppercase initials in the JPG download filename.

## 2026-11-05T13:58:40-05:00 — Publish with GitHub Pages

- Goal: Host the selfie page online.
- Request: Prepare the page for publication using GitHub Pages.
- Computer: `Peters-MacBook-Pro.local`
- Technical context: Serve a standalone `index.html` from the repository root over HTTPS.

## 2026-11-05T13:57:45-05:00 — Capture and save a selfie

- Goal: Create an HTML webcam photo page.
- Request: Provide a webcam preview, selfie capture, an initials text field, and retake and save buttons. Download the photo as `initials.jpg` using the entered initials.
- Computer: `Peters-MacBook-Pro.local`
- Technical context: The repository currently contains only a minimal README and Git attributes.
