# 🎥 OBS Camera Overlays by Zix

A collection of realistic camera overlays for OBS, designed for FiveM roleplay and content creation.

---

## 📦 Overlays Included

| File | Description |
|------|-------------|
| `gopro-overlay.html` | GoPro-style POV camera overlay with live clock and operator name |
| `axon-overlay.html` | Axon Body Cam-style overlay with live clock, officer name, callsign, and agency |

---

## ⚙️ OBS Installation Instructions

Follow these steps for **each** overlay you want to use.

### Step 1 — Download the Files
1. Click the green **Code** button on this repository
2. Select **Download ZIP**
3. Extract the ZIP to a folder on your computer (e.g. `C:\Overlays\Zix`)

---

### Step 2 — Add the Overlay to OBS

1. Open **OBS Studio**
2. In the **Sources** panel at the bottom, click the **+** button
3. Select **Browser** from the list
4. Name it (e.g. `GoPro Overlay` or `Axon Overlay`) and click **OK**

---

### Step 3 — Configure the Browser Source

In the Browser Source settings window:

1. Check the box that says **"Local file"**
2. Click **Browse** and navigate to the extracted folder
3. Select either `gopro-overlay.html` or `axon-overlay.html`
4. Set the **Width** and **Height** to match your canvas (e.g. `1920` x `1080`)
5. Check **"Shutdown source when not visible"**
6. Click **OK**

---

### Step 4 — Position the Overlay

1. In the OBS preview, click and drag the overlay to position it in the **top-left corner**
2. Right-click the source → **Transform** → **Fit to Screen** if needed
3. The overlay background is transparent — it will sit cleanly on top of your scene

---

### Step 5 — Customize Your Info

Open the `.html` file in any text editor (Notepad, VS Code, etc.) and find the edit section near the bottom:

#### GoPro Overlay
```js
// *** EDIT YOUR INFO HERE ***
const player = "Anthony Johnson";
```

#### Axon Body Cam Overlay
```js
// *** EDIT YOUR INFO HERE ***
const player  = "Anthony Johnson";
const agency  = "Blaine County Sheriff Department";
const callsign = "S-06";
```

Change the values to your character's info, **save the file**, then back in OBS right-click the Browser source and select **"Refresh cache of current page"** to apply changes.

---

## 🕐 Live Features

Both overlays include:
- ✅ Live ticking clock (updates every second)
- ✅ Auto date display (day, month, year)
- ✅ Transparent background (no black box in OBS)
- ✅ Blinking REC indicator

---

## 📝 Notes

- These overlays are **local HTML files** — no internet connection required once downloaded
- Tested with **OBS Studio 29+**
- Recommended canvas size: **1920x1080**

---

*Made by Zix*
