# 2026 Panini World Cup Sticker Tracker

A bilingual (Chinese/English) web app to help collectors track their progress of the 2026 Panini World Cup sticker album.  
Supports searching by player name, country, or sticker code, and automatically saves your collection locally.

🌐 **Live Demo**: [https://2026worldcup-stickers-collector.vercel.app/]  

## ✨ Features

- **Complete sticker database** – All 980+ base stickers + FIFA Museum, Coca‑Cola, and Extra stickers.
- **Mark collected** – Tap any sticker card to toggle collected/not collected.
- **Missing list** – One‑click filter to show only stickers you still need.
- **Search** – Find stickers by player name, country, or sticker code (e.g., `POR15` for Ronaldo).
- **Bilingual UI** – Switch between English and Chinese with a button (language preference saved).
- **Local storage** – Your collection progress is saved in your browser; no login required.
- **Mobile‑friendly** – Responsive design works on phones, tablets, and desktops.
- **Clear search** – One‑click clear the search box.
- **Runner icon** 🏃‍➡️ – Differentiated icons for player stickers vs. logos/team photos/special stickers.

## 🚀 How to Use

1. Open the [https://2026worldcup-stickers-collector.vercel.app/].
2. Browse or search for stickers.
3. Tap/click on any sticker card to mark it as **collected** (the card turns light yellow and shows a green checkmark ✅).
4. Use the **Missing List** button to see only the stickers you haven't collected yet.
5. Switch language via the **中文/English** button in the top‑right corner (your language choice is remembered).
6. The progress bar and counter at the top show how many stickers you have collected out of the total.

> **Note**: All data is stored locally in your browser’s `localStorage`. Clearing your browser data will reset your progress.

## 🛠️ Technical Details

- Pure HTML/CSS/JS – no backend, no database.
- Sticker data embedded as a JavaScript array (parsed from the official Panini checklist).
- Responsive CSS grid layout.
- Icons: player stickers use 🏃‍➡️, others use 🃏.

## 📦 Repository Structure

/
├── index.html
└── README.md

## 📝 Customization

- **Add actual sticker images** – Place images in an `images/` folder and modify the `renderStickersList()` function to output `<img>` tags instead of the placeholder icon.
- **Modify sticker data** – Edit the `RAW_LISTING` string inside the `<script>` tag (the data format is based on the official checklist lines).
- **Change colors / layout** – Edit the `<style>` section.

## 🌍 Deployment

This app is deployed on **Vercel**. Any push to the `main` branch triggers an automatic redeployment.

To deploy your own copy:
1. Fork this repository.
2. Import it into Vercel (or any static hosting service like Netlify, GitHub Pages).
3. Set the **Root Directory** to `/` and **Build Command** to empty.
4. Deploy.

## 📄 License

Feel free to use and modify for personal or community use.

## 🙋 Feedback & Contributions

If you find any missing stickers or have suggestions, please open an issue or pull request.

Happy collecting! 🏆⚽
