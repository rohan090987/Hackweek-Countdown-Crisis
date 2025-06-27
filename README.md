# Hackweek Countdown Crisis – Fixed Version

This is the corrected version of the Hackweek Countdown Crisis challenge.

## 🔧 What I Fixed

- ✅ **Hydration Errors**: Removed usage of `typeof window !== 'undefined'` and inline `style={{...}}`, which were causing hydration mismatches between server and client. Replaced them with Tailwind `className` for consistent SSR behavior.
- ✅ **Null Data Handling**: Wrapped all data accesses (like `data.name`, `data.date`) with optional chaining (`?.`) and added fallback UI for missing data in `CommunityInfo.jsx`.
- ✅ **Improved Stability**: Ensured that JSON fetching via `useEffect()` doesn’t trigger errors on first render.
- ✅ **Clean Console**: Resolved all console warnings and errors during SSR and client hydration.
- ✅ **Deployment Ready**: Verified that the app builds and deploys correctly without errors.

## 🚀 Live Demo

[Click to View Deployment](https://hackweek-countdown-crisis-nine.vercel.app/)

## 🛠️ Tech Stack

- Next.js
- React
- Tailwind CSS

## 💻 Setup

```bash
npm install
npm run dev

