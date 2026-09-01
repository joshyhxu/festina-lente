# The Scenic Route

A public bucket list. Not the fastest way through life — the one worth remembering.

Live at: `https://<your-github-username>.github.io/the-scenic-route`

## How to add or check off an item

1. Open `items.json`.
2. Add a new item to the array, or edit an existing one:

```json
{
  "text": "What you want to do",
  "category": "Travel",
  "done": false,
  "note": ""
}
```

   When you finish something, set `"done": true` and add `"dateCompleted": "YYYY-MM-DD"`.

3. Save, then from a terminal in this folder:

```bash
git add items.json
git commit -m "Add: <short description>"
git push
```

4. The site updates automatically within a minute or two.

## Running locally

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000` (opening `index.html` directly won't load the JSON due to browser file-access restrictions).
