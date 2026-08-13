# Tuesday League 2026 — Simple Score Tracker

This is a one-file web app built from `Tuesday League 2026.xlsx`.

## How it works
- The newest week is always the first score column beside Average.
- Type a score and press Enter to move to the next team in that same week.
- Blank scores do not count toward the average.
- Scores auto-save in the browser on the device being used.
- `+ Week` adds the next week and makes it the current entry column.
- `Rank by Avg` temporarily sorts teams by average.
- `+ Team` adds a new team/pair.

## Test it
Open `index.html` in a browser.

## Put it on GitHub Pages
1. Create a new GitHub repository.
2. Upload `index.html` to the root of the repository.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Choose the `main` branch and `/ (root)`, then save.

## Important storage note
This version saves scores in the browser's local storage. That means scores stay on the same browser/device. Before using multiple phones/computers, connect the app to a cloud database such as Firebase so every device sees the same scores.
