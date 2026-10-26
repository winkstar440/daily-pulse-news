# Daily Pulse | Auto-Updating News Hub

A clean, modern, bilingual (English / 中文) daily news dashboard that automatically pulls the latest stories from Google News RSS feeds.

## Features

- **Four curated categories**
  - 🎬 Horror Movies (Hollywood horror news)
  - ⭐ Star & Celebrity (gossip & entertainment)
  - ✨ Fashion & Style (trends & runway)
  - 📈 ETF & Finance (markets & ETF news)

- **Live updates** – Fetches fresh content from Google News via rss2json
- **24-hour local cache** – Reduces unnecessary API calls while keeping content reasonably fresh
- **Manual refresh** button
- **Bilingual support** – One-click switch between English and 中文
- **Dark / Light mode**
- **Responsive design** – Works well on desktop and mobile
- **GitHub Actions daily trigger** – A scheduled workflow pings the site every day at midnight UTC to help keep it warm / active

## Live Demo

Once GitHub Pages is enabled, the site will be available at:

**https://winkstar440.github.io/daily-pulse-news/**

## How it works

1. The frontend fetches Google News RSS feeds (converted through the public rss2json API).
2. Articles are cached in the browser’s `localStorage` for 24 hours.
3. Users can force a refresh at any time.
4. A GitHub Actions workflow runs daily and simply pings the GitHub Pages URL, which can help with cache warming or uptime monitoring.

## Enabling GitHub Pages

1. Go to the repository **Settings → Pages**
2. Under **Source**, select **Deploy from a branch**
3. Choose branch `main` and folder `/ (root)`
4. Click **Save**

After a short wait the site will be live.

## Tech Stack

- Pure HTML + Tailwind CSS (CDN)
- Lucide Icons
- Vanilla JavaScript
- Google News RSS + rss2json
- GitHub Actions (daily schedule)

## License

MIT – feel free to fork and customize.
