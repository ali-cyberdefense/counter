# Zikr Counter - Local Deploy & Install Instructions

## Option 1: Run Locally on Your Computer

Just double-click `index.html` — it opens in your browser and works immediately.

> Note: The "Add to Home Screen" (PWA install) feature requires serving over HTTP, not from a file. Use Option 2 or 3 for that.

---

## Option 2: Run a Local Server (for PWA install support)

### Using Python (pre-installed on Mac)

1. Open **Terminal**
2. Navigate to the project folder:
   ```
   cd ~/Projects/counter
   ```
3. Start a local server:
   ```
   python3 -m http.server 8000
   ```
4. Open your browser and go to:
   ```
   http://localhost:8000
   ```
5. To stop the server, press `Ctrl + C` in Terminal.

### Using Node.js (if installed)

1. Install a simple server globally:
   ```
   npm install -g serve
   ```
2. Run it:
   ```
   cd ~/Projects/counter
   serve .
   ```
3. Open the URL shown in Terminal (usually `http://localhost:3000`).

---

## Option 3: Deploy Free Online (recommended for phone install)

### GitHub Pages (completely free)

1. Create a free account on [github.com](https://github.com) (if you don't have one)
2. Create a new repository named `zikr-counter`
3. Upload all the project files (`index.html`, `sw.js`, `manifest.json`, `icon-192.png`, `icon-512.png`)
4. Go to **Settings** > **Pages**
5. Under "Source", select **main** branch and click **Save**
6. Your app will be live at: `https://yourusername.github.io/zikr-counter/`

### Netlify (completely free, drag & drop)

1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag the entire `counter` folder onto the page
3. Your app is instantly live with a URL you can open on your phone

---

## Installing on Your Phone

Once the app is served over HTTP (Option 2 or 3), you can install it like a native app:

### iPhone (Safari)

1. Open the app URL in **Safari**
2. Tap the **Share** button (square with arrow at the bottom)
3. Scroll down and tap **"Add to Home Screen"**
4. Tap **"Add"**
5. The app icon will appear on your home screen

### Android (Chrome)

1. Open the app URL in **Chrome**
2. You should see a banner saying **"Add Zikr to Home screen"** — tap it
3. If no banner appears, tap the **three-dot menu (⋮)** at the top right
4. Tap **"Add to Home screen"** or **"Install app"**
5. Tap **"Add"**

---

## Using the App

- **+ button** — Tap to increase your zikr count
- **− button** — Tap to decrease if you made a mistake
- **Reset button** (circular arrow) — Resets count to 0
- **Target dropdown** (top) — Set your goal (33, 99, 100, 200, 300, 500, 1000)
- When you reach your target, an **"Alhamdulillah!"** message appears and the counter resets automatically
- Your count is **saved automatically** — even if you close the app, it remembers where you left off
- Works **completely offline** — no internet needed after first load
