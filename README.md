# Words

A phone-friendly word-pattern game in a single HTML page. Pick a theme and a number of squares, then fill in letters to narrow down a list of matching words, or hide the list and guess the mystery word.

No backend and no install: everything, including the word lists, is inside `index.html`.

**Current version: 1.22**

## Play it

Open the GitHub Pages link for this repository in Safari or Chrome. On a phone you can use **Share → Add to Home Screen** to keep it like an app.

> File previews (GitHub's file view, the Claude app, or the Files app) don't run JavaScript, so the game won't work there. Use the GitHub Pages link.

## Features

- **Themes**: sixteen themes from Pocket Crossword, plus **Other (dictionary)** with about 40,000 everyday words, and **All themes**.
- **Squares**: choose a word length, or **Any length** (15 squares). The count in brackets shows how many words still fit your letters, for every length in the list.
- **Letter squares**: tap a square to pick a letter.
  - **Smart** on: each square offers only letters that the remaining words use in that position, even with letters locked.
  - **Smart** off: all 26 letters, and a letter no word allows turns red.
- **Keyboard**: a simple on-screen keyboard for typing the whole word, then **Enter** fills every square in one go.
  - **◀ / ▶** move the cursor without erasing, or tap a square in the preview.
  - **⌫** erases the letter before the cursor. **Skip** leaves a square blank. **Clear** empties the draft.
  - **Copy** loads the letters in the squares into the keyboard and copies them to the clipboard.
  - With Smart on, letter keys that can't make a word at the cursor are greyed out.
  - A computer keyboard works too (letters, Backspace, Enter, Space, arrow keys).
- **Lock letters**: keeps your letters in place on New word and when changing length.
- **Undo**: clears the last letter placed. After a solve or reveal it takes that back (the Solved count goes down for a solve), so you can try for a different word.
- **Unscramble**: rearranges the open squares' letters into a word from the list, using exactly those letters.
- **Show list**: on shows every matching word. Off plays the game: find the mystery word, and correct letters turn green.
- **Show clue**: shows clues, a clue list with tap-to-pick, and a clue search box.
- **Show scrambled**: shows the selected word's (or first word's) letters shuffled.
- **Advanced**: a pattern row where `?` is one letter and `*` is any number of letters.
- **Pull to refresh**: when opened from the home screen, drag down from the top and let go to reload (handy after publishing a new version).
- **Help**: the **?** button explains everything in the app.

Your theme, length, toggles, pattern and Solved count are remembered on the device.

## Recent changes

| Version | Change |
|---|---|
| 1.22 | Pull down from the top to refresh when opened from the phone home screen. |
| 1.21 | Undo button. It clears the last letter and can undo a solve or reveal. Keyboard draft now stays in step with the squares. |
| 1.20 | With Smart on, invalid letter keys on the keyboard are greyed out for the cursor's square. |
| 1.19 | Smart now limits square choices to the filtered words even when letters are locked. |
| 1.18 | Squares dropdown counts are correct for every length when letters are locked or picked. |
| 1.17 | Keyboard: ◀ ▶ cursor keys, Copy key, tap a preview square to move the cursor. |
| 1.16 | On-screen Keyboard for entering all squares in one action. |

Versions go up by 0.01 with each change.

## Publish with GitHub Pages

1. Put `index.html` (and this README) in the root of the repository's `main` branch.
2. On GitHub, open **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose **main** and **/ (root)**, then **Save**.
4. After a minute or two the page is live at `https://<your-username>.github.io/words/`.

To update, replace `index.html` with the new version and commit. Pages redeploys automatically.

## Credits

The Other word list and its clues come from [Wordset](https://github.com/wordset/wordset-dictionary) (CC BY-SA 4.0), based on WordNet 3.0 © Princeton University.
