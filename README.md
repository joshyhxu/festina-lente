# Festina Lente

*Make haste, slowly.*

A public bucket list. Live at **https://joshyhxu.github.io/festina-lente**

---

## How to change the list

You never need a terminal. Everything happens in your browser.

1. Go to **https://github.com/joshyhxu/festina-lente**
2. Click **`items.txt`**
3. Click the **pencil icon** (top right of the file)
4. Type your change
5. Scroll down, click the green **Commit changes** button

The site updates itself within a minute or two. Refresh the page to see it.

---

## The format

One item per line. That's it.

```
> Travel
Japan
Petra
See the Northern Lights
```

- A line starting with `>` is a **category heading**
- Every other line is an **item**
- Blank lines are ignored
- Lines starting with `#` are notes to yourself — they never show on the site

### Finished something?

Add two dashes and the date to the end of that line:

```
Climb Ben Nevis  -- 2026-08-15
```

It'll show a quiet date next to the item. Nothing gets crossed out, nothing gets counted. That's deliberate.

### New category?

Add a new `>` line anywhere, with items underneath it:

```
> Food
Eat at a three-Michelin-star restaurant
```

---

## Why it's a plain text file

It used to be `items.json`, where a single missing comma would silently blank the whole page. This format can't break — the worst that happens is an item lands in the wrong section, and you fix the line. The old file is kept as `items.json.old` and is no longer used by the site.

---

## Running it locally (optional, rarely needed)

```bash
cd ~/festina-lente && python3 -m http.server 8000
```

Then open `http://localhost:8000`.
