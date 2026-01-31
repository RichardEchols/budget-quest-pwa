# Budget Quest 💰

A gamified personal finance dashboard to help track spending, cancel unnecessary subscriptions, and build a $48k emergency fund.

## Features

- **Emergency Fund Tracker** - Visual progress toward $48,000 goal
- **Apple Card Balance Tracking** - See what you owe and real available money
- **Subscription Management** - Track subscriptions to cancel vs keep
- **Spending Budget** - $1,000/month discretionary limit with category breakdowns
- **Bill Tracking** - Fixed bills with due dates and quick pay links
- **Gamification** - XP, levels, streaks, and confetti celebrations

## Tech Stack

- React 18 (via CDN)
- TailwindCSS (via CDN)
- localStorage for data persistence
- Service Worker for offline support
- PWA-enabled (installable on mobile/desktop)

## Deploy to Vercel

1. Push this repo to GitHub
2. Go to [vercel.com](https://vercel.com)
3. Click "New Project" → Import your GitHub repo
4. Vercel auto-detects settings from `vercel.json`
5. Click "Deploy"

## Local Development

Just open `public/index.html` in a browser. No build step required!

For PWA features (service worker), you'll need a local server:
```bash
npx serve public
```

## Data Storage

All data is stored in browser localStorage:
- `bq_savings` - Current savings balance
- `bq_cardbalance` - Apple Card balance
- `bq_spending` - Monthly spending by category
- `bq_cancelled` - List of cancelled subscriptions
- `bq_transactions` - Recent transaction history

Data persists as long as you use the same browser and don't clear site data.

---

Built with Claude 🤖
