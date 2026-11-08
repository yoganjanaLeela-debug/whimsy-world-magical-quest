# Whimsy World: The Magical Quest

A colourful, browser-based fantasy platform adventure featuring magical worlds, collectible heroes, level progression, treasure and gift rewards.

## Game overview

- **5 fantasy worlds:** Candy Kingdom, Magical Forest, Crystal Mountains, Cloud Kingdom and Dragon Castle
- **100 level slots** across the five worlds
- **50 collectible fantasy characters**
- Easy, Medium, Hard and Boss difficulty categories
- Platform gameplay with coins, gems, enemies, obstacles and collectibles
- Gift-token collection and gift-box rewards
- Daily treasure, missions and achievements
- Character selection and abilities
- Local save data with backup export/import

> This is a client-side browser game. Progress is saved in the browser on the device where you play; there is no account system or cloud synchronisation.

## Play the game

### Option 1: Run locally

1. Download or clone this repository.
2. Keep the `vendor` folder in the same location as `index.html`.
3. Open `index.html` in a modern web browser.

No build step or package installation is required.

### Option 2: Publish with GitHub Pages

1. Create a GitHub repository.
2. Upload **all files and folders** from this project. Do not upload only `index.html`.
3. Open the repository's **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)` folder, then save.
6. Wait for GitHub Pages to publish the site. The published URL will appear in the Pages settings.

The `vendor` folder is required because the game loads its local React runtime from that folder.

## Controls

### Desktop
- **Move:** Arrow keys or `A` / `D`
- **Jump:** Space
- **Pause:** `P`
- **Restart level:** `R`

### Mobile
Use the on-screen movement and jump controls.

## Project structure

```text
whimsy-world/
├── index.html
├── README.md
├── .gitignore
└── vendor/
    ├── react.production.min.js
    └── react-dom.production.min.js
```

The game UI, styling, canvas game engine, character definitions, level logic and progression are currently contained in `index.html`.

## Save data and privacy

- Save data is stored locally in your browser (`localStorage`).
- The game does not currently provide cloud saves or cross-device synchronisation.
- Use **More → Settings** to export or import a backup code.
- Clearing browser storage may erase local progress. Export a backup before clearing it.

## Technologies

- HTML5
- CSS3
- JavaScript
- Canvas API
- React 18 runtime (included locally in `vendor/`)

The Fredoka font is loaded from Google Fonts when an internet connection is available. A system-font fallback is provided.

## Notes

- Keep the `vendor/` directory alongside `index.html`; removing it will prevent the app from loading.
- This repository contains the playable web project, not an Android APK.
- Add your own screenshots or gameplay GIFs to a `screenshots/` folder and embed them here when you are ready to showcase the game.

## License

No open-source license has been added yet. Unless you add a license, the source remains protected by the default copyright rules. If you want others to reuse, modify or distribute the project, choose and add an appropriate license.
