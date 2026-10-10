# Fearless Reader

Fearless Reader is a small, browser-based reading assistant. It gives readers control over the text display and pacing, with optional speech tracking and read-aloud support.

## Open the app

Open FearlessReader.html in a modern web browser. There is no build step, account, or server.

## Features

- Paste text, type directly, or open a plain .txt file up to 5 MB.
- Read one sentence at a time and navigate with the keyboard-accessible previous and next buttons.
- Adjust text size, typeface, line and word spacing, sentence focus, and page colors, including a high-contrast theme.
- Use the always-visible A− and A+ controls to resize reading text without opening the settings panel.
- Keep display settings collapsed while reading, then open them on demand; independently resize the settings text and spacing.
- Optionally bold the beginnings of words.
- See recognized characters highlight green with near-immediate visual updates as interim results arrive; confirmed words stay highlighted. Read-aloud playback can also follow its current word where browser boundary events are available.
- Turn the always-visible **Follow my voice** control on or off at any time. Recognized characters highlight green as soon as the browser returns interim speech results.
- Mark words read by selecting a word, using **Mark next word read**, or enabling speech tracking.
- Undo the last word mark and review session word and sentence counts.
- Listen with browser read-aloud voices, choose an installed voice, and adjust playback speed. Read aloud moves through the passage sentence by sentence.
- Choose a speech language and optionally advance after a sentence has been read.
- Finish only when you choose **Finish reading**. The app then celebrates and returns to the text editor with your passage ready to edit or read again.
- Turn confetti and the short victory sound on or off in the reading settings. Confetti is automatically suppressed when reduced motion is enabled.
- Settings are saved in this browser. The passage itself is not saved.

## Accessibility

The page has a skip link, labelled controls, visible keyboard focus, responsive layouts, reduced-motion support, status announcements, and button-based alternatives for word marking and navigation. Quick text-size controls stay outside the collapsible settings panel, and settings scale independently of the article. Character animation is visual; assistive technology receives the word as normal text rather than a stream of individual letters. Voice tracking, confetti, and sound are optional and can be switched off. Reduced-motion preferences disable animated confetti.

Reading preferences are intended to help readers find a comfortable presentation; no one font, color, or bolding style works for everyone. Try the controls and keep the settings that help you.

## Privacy and browser support

The app has no account, analytics, or backend and does not itself upload or save passage text. Display preferences are stored in local browser storage.

Microphone access is requested only when voice tracking is enabled. Speech recognition is provided by the browser and may send audio to the browser vendor's speech service; character previews turn green as quickly as the interim transcript the browser returns. The browser may take time to provide partial results, and the app cannot highlight speech it has not received. Read-aloud voices and word-boundary events also come from the browser or operating system. Availability and behavior vary by browser, device, language, and installed voices; on-screen reading and manual controls remain available if these features are unsupported.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE).
