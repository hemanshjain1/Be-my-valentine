# Valentine's Site - Setup & Deployment Guide

## Quick Deploy to GitHub Pages

### Step 1: Create a GitHub Repository

1. Go to [github.com/new](https://github.com/new)
2. Name it something like `valentine` or `be-my-valentine`
3. Set it to **Public**
4. Click **Create repository**

### Step 2: Push Your Code

Open a terminal in this folder and run:

```bash
git init
git add .
git commit -m "Will you be my valentine? 💖"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git push -u origin main
```

Replace `YOUR_USERNAME` and `YOUR_REPO_NAME` with your actual GitHub username and repo name.

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (tab at the top)
3. In the left sidebar, click **Pages**
4. Under **Source**, select **Deploy from a branch**
5. Under **Branch**, select `main` and `/ (root)`
6. Click **Save**

### Step 4: Share the Link

Your site will be live in about 1-2 minutes at:

```
https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/
```

Send this link to Kavya and wait for the magic! 💌

---

## Customization

### Background Music
Place your `song.mp3` file in the same folder as `index.html`. The music will auto-play on the first click and loop continuously. A toggle button (bottom-right corner) lets the user mute/unmute.

**Note:** GitHub Pages has a 100MB file size limit. If your MP3 is large, consider compressing it first.

### Change the Name
Open `index.html` and search for "Kavya" — replace it with any name you'd like.

### Change the Excuses
In the `excuses` array inside `<script>`, edit or add your own funny excuses.

### Change Colors
The main colors are defined in the CSS:
- `#ff3366` — primary pink
- `#ff6b9d` — lighter pink
- `#ffb6c1` — soft pink
- `#1a0a1e` — dark background

---

## How It Works

- **Yes Button**: Grows bigger every time "No" is clicked, making it impossible to ignore
- **No Button**: Shrinks and changes text with each click, becoming increasingly desperate
- **Excuses**: 20 unique funny popup messages appear when "No" is clicked
- **Bear Emoji**: Gets progressively sadder with each rejection
- **Background Music**: Auto-plays on first click, loops forever, with a mute/unmute toggle
- **Success Screen**: Confetti explosion and celebration when "Yes" is finally clicked

Good luck! 🍀💖
