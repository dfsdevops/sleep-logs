# Consensus Sleep Diary

A client-side web app for logging daily sleep data using the Consensus Sleep Diary format. Designed to help patients track sleep patterns and share printed summaries with their healthcare provider.

## Features

- **Complete Consensus Sleep Diary questionnaire** — all 15 standard questions (1–15), including sub-questions
- **Auto-calculation** of total sleep time from your entries
- **Print view** — landscape-formatted weekly tables with dates as columns and questions as rows, 7 days per page
- **History** — browse, edit, and delete past entries; incomplete entries are flagged
- **Export / Import** — download all entries as a JSON backup file and reload them at any time
- **Patient name** — stored once, printed on every page
- **Fully offline** — no server, no accounts, no network required after the page loads

## How to use

Open `index.html` directly in any modern browser — no installation or server needed.

### Logging entries

1. Open the **Log Entry** tab
2. Fill out the questions for the night you are recording
3. Click **Save Entry** — the form validates required fields before saving

### Backing up your data

Your data lives **only in your browser's local storage**. It will be lost if you clear your browser data or switch browsers.

- Use **Export Data** (top right) regularly to download a `sleep-diary-YYYY-MM-DD.json` backup file
- Use **Import Data** to restore entries from a backup — existing dates are never overwritten on import

### Printing

1. Open the **Print View** tab
2. Enter your name in the **Patient Name** field (saved automatically)
3. Set a date range
4. Click **Print / Save PDF** — each week prints on its own landscape page

## Privacy

This app stores all data locally in your browser using `localStorage`. No data is ever transmitted to any server. The hosted files on GitHub Pages are static — GitHub has no access to your sleep data.

This app is not a medical device and is not intended to replace professional medical advice, diagnosis, or treatment. Always consult a qualified healthcare provider regarding any sleep concerns.

## Browser compatibility

Works in any modern browser (Chrome, Firefox, Safari, Edge). Data is stored per-browser and per-device — entries logged in Chrome will not appear in Safari.

## License

MIT — see [LICENSE](LICENSE).
