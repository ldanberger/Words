# Words

A phone-friendly word-pattern game and word finder in a single HTML file. Pick a theme and a word length, then pick letters square by square. Words lists every word that still fits, or hides the list so you can solve a mystery word from its clue.

**Current version:** 1.12

**Play:** https://ldanberger.github.io/words/ (once GitHub Pages is turned on, see [Hosting](#hosting))

## Features

- **17 themes plus All themes.** General, Medical, Plants, Westerns, Game of Thrones, History, Science, Board Games, Trivia, Canada, Scotland, Australia, Earth, Grade 5, Grade 6 and Grade 7 come from Pocket Crossword. Other (dictionary) adds about 39,700 everyday words.
- **Any length or a fixed length.** The number in brackets is how many words still fit, and it updates as you pick letters.
- **Smart letter choices.** Each square's dropdown offers only letters that can still make a real word.
- **Show list.** Turn it on to see every matching word. Turn it off to play: find the mystery word, or any word in the filtered list, to add to your Solved count.
- **Show clue.** Shows clues next to words, or a scrolling clue list when the word list is hidden. Includes a **Search clues** box.
- **Pick one clue.** Tap a clue or word to narrow everything to that word.
- **Lock letters.** Fix the letters you have. Other squares then offer all 26 letters, and impossible picks turn red. Locked letters carry over to the next word.
- **Advanced pattern.** Use letters, `?` for exactly one letter, and `*` for any number of letters. For example, `?A*D` finds PAID, BALLED and BAD.
- **Show scrambled.** Shows the letters of the selected (or first) word in random order.
- **Reveal word, New word and Next word.** After a solve or reveal, the game waits for you to tap Next word.
- **Help page.** Tap the **?** button.
- **Remembers your settings** (theme, length, toggles, pattern and Solved count) on each device.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole game: code, styles, help page and every word list. About 2.5 MB. |
| `README.md` | This file. |

There is no build step, server or database. The only outside resource is Google Fonts. Offline, the page falls back to the phone's own fonts.

## Hosting

The page must run in a real browser. File previews (GitHub's file view, the Files app, chat apps) don't run JavaScript, so the lists stay empty.

To publish with GitHub Pages:

1. Open the repository's **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select **main** and **/ (root)**, then **Save**.
4. After a minute or two, open https://ldanberger.github.io/words/ in Safari or Chrome.

To run it locally, open `index.html` in any modern browser.

## Versioning

The version shows next to the title and on the help page. It starts at 1.0 and goes up by .01 with each change.

## Credits

- Themed word lists and clues from the Pocket Crossword project.
- The **Other (dictionary)** list and its clues come from [Wordset](https://github.com/wordset/wordset-dictionary), licensed [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) and based on [WordNet 3.0](https://wordnet.princeton.edu/), © 2006 Princeton University. Words were limited to plain lowercase entries also found in the standard US English spell-check dictionary. Each clue is the first definition that doesn't contain the word.
- Fonts: Bricolage Grotesque, Atkinson Hyperlegible and JetBrains Mono, from Google Fonts.

Because the dictionary data is CC BY-SA 4.0, any copy or change of that word list must keep this attribution and the same license.
