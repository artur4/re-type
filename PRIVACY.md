# ReType Privacy Policy

*Русская версия: [PRIVACY.ru.md](PRIVACY.ru.md)*

**Effective date:** November 3, 2026

ReType is a keyboard layout switcher for macOS and Windows. It fixes text typed in the wrong
layout (for example, `ghbdtn` → `привет`) and small typos. This policy explains what ReType
does with your data. In short: **everything stays on your computer. ReType has no accounts,
no ads, no analytics and no telemetry, and it never sends what you type anywhere.**

## What ReType reads and why

To work, ReType needs system permission to see the keys you press
(on macOS: *Accessibility*; on Windows: a keyboard hook). With it, ReType:

- **Watches the keys you press.** It keeps the word you are typing in memory to decide whether
  it was typed in the wrong layout or with a typo. The word is forgotten once it is finished,
  except as described under *Personal dictionary* below.
- **Types for you.** When it fixes a word, it erases the word and types the corrected one.
- **Reads the selected text** when you press Shift to convert a selection, and the text right
  before the cursor and the type of the focused field to decide whether a word starts a
  sentence. This is read through the system accessibility interface, only at that moment,
  and is not stored.
- **Uses the clipboard only if you turn on** “Copy the selection if the app doesn't report it”.
  ReType then copies the selection, converts it and puts back what was in your clipboard.
  The copied text is not stored.

ReType does not work in password fields: on macOS the system blocks keyboard access there,
and ReType pauses as well.

## What ReType stores on your computer

All of this is stored only on your computer, in the app's own settings and folder:

- **Settings** — your choices in the Settings window, including the lists of exceptions
  (words and apps where ReType should not make changes).
- **Personal dictionary** — words and corrections ReType has learned from your typing, with
  how many times each was used and when. It helps ReType stop correcting words you use on
  purpose. You can view it, forget individual entries, export, import or clear it in
  Settings → Dictionary, or turn learning off.
- **Statistics** — counters shown in Settings → About: how many words were fixed, how many
  fixes you undid, the estimated time saved. They contain no text. You can reset them there.

ReType does not keep a history of what you typed and does not record keystrokes to disk.

## Network access

ReType connects to the internet for one thing only: **checking for updates.**

- **macOS (downloaded from the website):** ReType uses the open-source Sparkle framework.
  It downloads the update feed `appcast.xml` from GitHub (`raw.githubusercontent.com`) when
  you press “Check for Updates…” and, silently, when you open the ReType menu — no more than
  once every 3 hours. If an update is available and you choose to install it, the update
  file is downloaded from the same place. Like any web request, this reveals your IP address
  and the app and system version (in the User-Agent header) to GitHub. No other information
  is sent. GitHub's handling of this data is described in the
  [GitHub Privacy Statement](https://docs.github.com/site-policy/privacy-policies/github-general-privacy-statement).
- **Windows (Microsoft Store):** updates are delivered by the Microsoft Store and are subject
  to the [Microsoft Privacy Statement](https://privacy.microsoft.com/privacystatement).
  ReType itself makes no network requests.

ReType does not send what you type, your dictionary, settings or statistics anywhere.

## Sharing

ReType does not sell, share or transfer your data to anyone. The developer has no access to it:
it never leaves your computer.

## Deleting your data

- In Settings you can clear the personal dictionary and reset the statistics at any time.
- **macOS:** to remove everything, quit ReType, delete the app and the folder
  `~/Library/Application Support/Raskladka`. Settings are stored in
  `~/Library/Preferences/com.artur.raskladka.plist`.
- **Windows:** uninstalling the app removes its settings and data.

## Children

ReType is a general-purpose utility. It does not collect personal information from anyone,
including children.

## Changes

If this policy changes, the new version will be published at this address with a new
effective date. Changes that affect how data is handled will also be mentioned in the
release notes.

## Contact

Questions about this policy or about ReType: **arturmirrov@gmail.com**
