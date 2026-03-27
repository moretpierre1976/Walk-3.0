# 🥾 Local Walks

A community app to organise local walks, invite friends, and share walk links via WhatsApp or text. Powered by React + Firebase Firestore.

## Tech Stack

- **React 18** + **Vite** — fast modern frontend
- **Firebase Firestore** — real-time central database
- **Vercel** — free hosting with automatic deployments

---

## Local Development

1. Install dependencies:
   ```bash
   npm install
   ```

2. Start the dev server:
   ```bash
   npm run dev
   ```

3. Open [http://localhost:5173](http://localhost:5173)

---

## Deploy to Vercel (first time)

### Step 1 — Push to GitHub
1. Go to [github.com](https://github.com) and create a new repository called `local-walks`
2. In your terminal, inside this folder run:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/local-walks.git
   git push -u origin main
   ```

### Step 2 — Deploy on Vercel
1. Go to [vercel.com](https://vercel.com) and sign up with your GitHub account
2. Click **"Add New Project"**
3. Import your `local-walks` GitHub repository
4. Leave all settings as default (Vercel auto-detects Vite)
5. Click **Deploy**

Your app will be live at `https://local-walks.vercel.app` (or similar) within ~60 seconds!

### Step 3 — Future updates
Any time you push to GitHub, Vercel automatically redeploys:
```bash
git add .
git commit -m "Your change description"
git push
```

---

## Firebase Setup

The Firebase config is already included in `src/firebase.js`. Your Firestore database stores:

- **`users`** collection — one document per user (keyed by email)
- **`walks`** collection — one document per walk (keyed by walk ID)

To view your data: [Firebase Console](https://console.firebase.google.com/project/newwalk-ebd2b/firestore)

---

## Features

- ✅ Register & sign in
- ✅ Create walks with date, time, location, description
- ✅ Invite named guests
- ✅ Share walks via WhatsApp, text, or copyable link
- ✅ Anyone with the link can view & join
- ✅ Only the creator can edit or cancel
- ✅ Real-time updates — no refresh needed
- ✅ Filter by All / Upcoming / My Walks / Joined
