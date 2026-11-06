# capture-photo

A mobile-friendly webcam page that captures a selfie and downloads it as
`<initials>.jpg`. Open [index.html](index.html) through a web server, start the
camera, enter initials, take a photo, then choose **Save photo** or **Retake**.
Optionally enter a **Real Name** to append it to the filename, for example
`AB-Jane-Doe.jpg`. Spaces and punctuation in the name become hyphens; letters
(including accented letters) and numbers are preserved. Leaving the name blank
keeps `AB.jpg`. The filename preview updates as you type.
After saving, choose **New photo** to clear both fields and return to the live preview
for the next photo. **Retake** keeps both fields.
Initials accept 1–12 letters or numbers and automatically convert to uppercase
as entered or pasted. The filename uses uppercase initials, for example `AB.jpg`.
Photos are mirrored to match the preview and stay in the browser until downloaded.
The camera stays active between photos so **Retake** and **New photo** reuse the
existing camera session. Camera access stops when you leave or close the page.
If the camera disconnects or access is revoked, starting it again may require
permission. No dependencies, build step, or uploads.

On landscape screens, the fields and buttons appear to the right of the photo
viewer. On portrait screens, they appear below it. The layout updates automatically
when the screen rotates or the browser window is resized.

## Publish with GitHub Pages

1. Push these files to your GitHub repository.
2. In **Settings → Pages**, select **Deploy from a branch**.
3. Select the branch containing these files and **/ (root)**, then click **Save**.
4. Open the HTTPS URL provided by GitHub Pages and allow camera access.

See GitHub's [publishing source guide](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
for the Pages settings.

The page is served directly from the repository root; no `docs/` output folder is
needed. A browser may show a save/share prompt instead of downloading immediately,
depending on the device and its settings.

## Local preview

Run `python3 -m http.server 8000` from this folder and open
<http://localhost:8000>. Webcam access requires HTTPS or localhost. Opening the
file directly or using an ordinary HTTP address on another device may prevent
camera access.

## Project records

- [Prompt log](prompts.md): concise requests that guide the project.
