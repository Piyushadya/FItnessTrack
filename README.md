# 🏋️ FitTrack Pro

A fully offline, iOS-style fitness tracker that runs entirely in your browser — no app store, no installation, no account needed. Built as a single HTML file.

-----

## 📱 Add to Your Phone (Free — Works Like a Native App)

### iPhone / iPad (Safari)

1. Open **Safari** on your iPhone or iPad
1. Go to your GitHub Pages link:
   
   ```
   https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/fittrack.html
   ```
1. Tap the **Share** button at the bottom of the screen (the box with an arrow pointing up)
1. Scroll down and tap **“Add to Home Screen”**
1. Give it a name (e.g. *FitTrack*) and tap **Add**
1. The app now appears on your home screen with a full-screen experience — no browser bar, no address bar

> ✅ Works fully offline after the first load. No internet required.

-----

### Android (Chrome)

1. Open **Chrome** on your Android device
1. Go to your GitHub Pages link:
   
   ```
   https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/fittrack.html
   ```
1. Tap the **three-dot menu** (⋮) in the top-right corner
1. Tap **“Add to Home screen”**
1. Tap **Add** on the confirmation prompt
1. The app icon appears on your home screen

> ✅ Also works in Samsung Internet and Firefox for Android using the same steps.

-----

## 🚀 Setup on GitHub Pages (5 minutes)

### Step 1 — Fork or upload the file

**Option A — Upload directly:**

1. Go to your GitHub repository (create one if you don’t have one)
1. Click **“Add file”** → **“Upload files”**
1. Drag and drop `fittrack.html` into the upload area
1. Click **“Commit changes”**

**Option B — Clone and push:**

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
cd YOUR-REPO-NAME
cp /path/to/fittrack.html .
git add fittrack.html
git commit -m "Add FitTrack Pro"
git push
```

### Step 2 — Enable GitHub Pages

1. Go to your repository on GitHub
1. Click **Settings** (top menu)
1. Scroll down to **Pages** in the left sidebar
1. Under **Source**, select **“Deploy from a branch”**
1. Choose **main** branch and **/ (root)** folder
1. Click **Save**
1. Wait 1–2 minutes, then your site will be live at:
   
   ```
   https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/
   ```

### Step 3 — Open on your phone

Visit the URL above in your mobile browser and follow the “Add to Home Screen” steps above.

-----

## ✨ Features

|Feature          |Details                                                                 |
|-----------------|------------------------------------------------------------------------|
|🏠 Home Dashboard |Goal ring, calorie tracker, today’s workout & meals, week strip calendar|
|💪 Workout Planner|5-day program, exercise checklists, auto-advance, week locking          |
|🥗 Meal Tracker   |7-day meal plan, calorie & protein logging, live intake bar             |
|📊 Progress       |Weight chart, milestones, streak tracker, month calendar view           |
|👤 Profile        |Edit all stats, auto goal detection, custom avatar, grocery list editor |
|📅 Month Calendar |Tap any day to see workout + calorie summary                            |
|🔒 Week Lock      |Completes lock until Monday — forces full rest & recovery               |
|📴 Fully Offline  |No server, no account, no tracking — all data stays on your device      |

-----

## 🔒 Privacy

All your data is stored **locally on your device** using `localStorage`. Nothing is ever sent to any server. Clearing your browser data will erase the app data, so use the **Export JSON** button in Profile → Data to back up your progress.

-----

## 📲 Browser Compatibility

|Browser         |iOS              |Android|
|----------------|-----------------|-------|
|Safari          |✅ Best experience|—      |
|Chrome          |✅                |✅      |
|Samsung Internet|—                |✅      |
|Firefox         |✅                |✅      |


> For the best iOS experience, always use **Safari** — it enables the full-screen “Add to Home Screen” PWA mode.

-----

## 🛠️ Customisation

The entire app is one self-contained HTML file. To personalise it:

- Open `fittrack.html` in any text editor
- Find `var DEFAULT_PROFILE` near the top of the `<script>` section
- Edit the default values (name, weight, target, calories etc.)
- Save and re-upload to GitHub

-----

## 📤 Backup & Restore

Your data is saved automatically. To back it up:

1. Go to **Profile** tab
1. Scroll to **Data** section
1. Tap **📤 Export JSON** — saves a `.json` file to your device

To restore, you’ll need to re-import via the browser console (open DevTools → Console):

```js
localStorage.setItem('ft_v3', JSON.stringify(/* paste your JSON here */));
location.reload();
```

-----

## 📋 Default Meal Plan

The app comes pre-loaded with a 7-day Indian meal plan (~1900 kcal/day, ~140g protein):

- **Day 1** — Chicken + Rice, Roasted Chana, Egg Bhurji, Yogurt + Almonds
- **Day 2** — Tofu + Quinoa, Apple + PB, Dal + Roti, Protein Shake
- **Day 3** — Chicken Curry, Boiled Eggs, Chicken Salad, Peanuts
- **Day 4** — Rajma + Rice, Yogurt, Tofu + Roti, Makhana
- **Day 5** — Chicken Pulao, Eggs, Omelette + Roti, Almonds
- **Day 6** — Chole + Roti, Fruit + Nuts, Dal + Rice, Protein Shake
- **Day 7** — Chicken/Tofu Wrap, Yogurt + Seeds, Egg Curry + Roti, Peanuts

You can edit, delete or add any meals from the Meals tab.

-----

## 💪 Default Workout Plan

5-day intermediate program (~60 min/session, fat loss focus):

|Day  |Focus                                    |
|-----|-----------------------------------------|
|Day 1|Upper Body + HIIT Bike                   |
|Day 2|Lower Body (Knee Friendly) + Incline Walk|
|Day 3|Full Body + HIIT Rowing                  |
|Day 4|Upper Body + Cycling                     |
|Day 5|Fat Burn Circuit + Core                  |

-----

*Made with ❤️ — one HTML file, zero dependencies, fully yours.*
