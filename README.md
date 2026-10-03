# Rungs

A word ladder game. Turn one four-letter word into another by changing a single letter per rung, where every rung has to be a real word.

**Play it:** https://YOUR-USERNAME.github.io/rungs/

## How to play

- Tap a letter on your current rung, then pick its replacement. On a computer, use the arrow keys to move and type a letter.
- Each puzzle has a par, which is the fewest steps possible. Try to match it.
- Yellow letters are already in the right place for the goal word.
- Undo takes back a rung. Hint plays the next word for you and costs one extra step.
- Choose a Short, Medium or Tall ladder (3 to 6 steps).

Your solved count, on-par count and streak are saved in your browser.

## How it's built

The whole game is one file, `index.html`, with no build step and no dependencies. Open it in a browser and it runs.

- Puzzles are generated in the browser with a breadth-first search over a graph of four-letter words, so every puzzle has a known shortest solution.
- Start and goal words come from a list of common words, and each puzzle is guaranteed to be solvable at par using common words only.
- Works on phones and desktops, in light and dark mode.

## Word lists

- Accepted words: the ENABLE word list (public domain).
- Common words: filtered from the [google-10000-english](https://github.com/first20hours/google-10000-english) list.
