Original prompt: hey buddy, I want to add qr code images to the site. how do I do that? also...below every qr code, or wherever is aesthetically proper, I'd like to have a sign Please use Android phone. I want android underlined or bolded. can you help?

- Replaced all six `QR image placeholder` blocks in `index.html` with a QR image element and caption.
- QR source now points to a static code for `https://airplanes-8e6ee.web.app/tasks/portal/index.html` (no timestamp query param).
- Added `.qr-note` styling and emphasized `Android` using bold + underline (`<strong>` + underline CSS).
- Updated `.qr` styles to support image + caption layout and keep alignment responsive.

TODO / follow-ups:
- If each experience should have a different URL, replace each QR `data=` value with the correct per-experience link.
- Current QR images are loaded from `api.qrserver.com`; swap to local image assets if offline reliability is required.
- Visual QA in browser pending in this run.
- Updated Phoenix Flight QR to point to `https://airplanes-8e6ee.web.app/tasks/phoenix-terrace-shoot/index.html`.
- Kept all other experience QR links unchanged.
- Updated Airplane Takeoff QR to point to `https://airplanes-8e6ee.web.app/tasks/travelling-circus/index.html`.
- Updated Welcome / sendoff party QR to point to `https://airplanes-8e6ee.web.app/tasks/airport-greeting-gif/index.html`.
- Removed QR block from Austrian Airlines Logo-Triggered AR section.
- Moved `airport-greeting-gif` QR assignment to the Welcome / sendoff party section.
- Changed default theme initialization from dark to light (`setTheme("light")`).
