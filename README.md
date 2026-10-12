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
- See recognized characters highlight green in the active sentence with near-immediate visual updates as interim results arrive; words in other sentences are never highlighted by the current speech match. Confirmed voice-matched characters stay green. Read-aloud playback can also follow its current word where browser boundary events are available.
- Turn the always-visible **Follow my voice** control on or off at any time. Live status tells you when the microphone is active, speech is heard, or the browser cannot reach its speech service.
- Mark the next word read, select a word and choose **Mark through selected word**, or enable speech tracking.
- Move to the next sentence automatically when speech tracking confirms the last word; the pacing setting also controls automatic advance after manual word marking.
- Select any visible word in the current paragraph to open **How to pronounce**. Word help shows a plain-letter sound-out guide, syllable count, rhymes, and a short meaning, and can play the word using dictionary audio or a browser voice. The technical IPA transcription is tucked away, and coded phoneme strings are never shown as a pronunciation.
- Undo the last word mark and review session word and sentence counts.
- Listen with browser read-aloud voices, choose an installed voice, and adjust playback speed. Read aloud moves through the passage sentence by sentence.
- Choose a speech language and adjust whether manually marked sentences advance automatically.
- When the final sentence is complete, the **Finish reading** button glows gold. The session stays open until you choose it.
- Finish only when you choose **Finish reading**. The app then celebrates and returns to the text editor with your passage ready to edit or read again.
- Turn confetti and the short victory sound on or off in the reading settings. Confetti is automatically suppressed when reduced motion is enabled.
- Settings are saved in this browser. The passage itself is not saved.

## Accessibility

The page has a skip link, labelled controls, visible keyboard focus, responsive layouts, reduced-motion support, status announcements, and button-based alternatives for word marking and navigation. Words in the active sentence can be selected by keyboard; any visible word in the current paragraph can be selected by pointer. Quick text-size controls stay outside the collapsible settings panel, and settings scale independently of the article. Character animation is visual; assistive technology receives the word as normal text rather than a stream of individual letters. Voice tracking, confetti, and sound are optional and can be switched off. Reduced-motion preferences disable animation.

Reading preferences are intended to help readers find a comfortable presentation; no one font, color, or bolding style works for everyone. Try the controls and keep the settings that help you.

## Privacy and browser support

The app has no account, analytics, or backend and does not itself upload or save passage text. Display preferences are stored in local browser storage. Pronunciation help is optional: when you ask about a word, the app sends only that selected word to the [Free Dictionary API](https://dictionaryapi.dev/) and [Datamuse](https://www.datamuse.com/api/) for available IPA, syllable information, meanings, and rhymes. The passage and surrounding sentence are not sent by dictionary lookup. The app converts recognized IPA to a plain-letter guide and hides IPA under an optional disclosure; it does not show raw phoneme codes. A sound-out guide is an approximation and accents can differ. The selected word may be present in those services' query logs; Datamuse documents temporary query logging in its [privacy notes](https://www.datamuse.com/api/#privacy). Browser speech may use the browser's own voice service. English and Spanish have live phonetic and syllable lookups; rhyme suggestions are currently English. If a service is offline or does not have an entry, the app still offers a syllable estimate and browser speech when available.

Microphone access is requested only when voice tracking is enabled. Speech recognition is provided by the browser and may send audio to the browser vendor's speech service; character previews turn green as quickly as the interim transcript the browser returns. The browser may take time to provide partial results, and the app cannot highlight speech it has not received. If tracking does not start, allow microphone access, check the live status message, and select the language you are speaking. Read-aloud voices and word-boundary events also come from the browser or operating system. Availability and behavior vary by browser, device, language, and installed voices; on-screen reading and manual controls remain available if these features are unsupported.

Datamuse is acknowledged for the phonetic, syllable, and rhyme metadata used by word help.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE).
