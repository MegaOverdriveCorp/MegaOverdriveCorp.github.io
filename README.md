<p align="center">
  <img src="icon.svg" width="64" height="64" alt="MegaOverdriveCorp icon">
</p>

<h1 align="center">MegaOverdriveCorp</h1>

<p align="center"><strong>SYSTEM ONLINE. Accelerating enterprise synergy since 1989.</strong></p>

<p align="center">
  <a href="https://megaoverdrivecorp.github.io">megaoverdrivecorp.github.io</a>
</p>

---

MegaOverdriveCorp builds browser-based tools for cloud architecture, data modelling and the occasional pizza, and presents them the way a 16-bit business simulator from 1989 would have: hot orange wordmark, navy night sky, teal skyline, bevelled panels and a HUD.

This repository is the organisation home page. It is a single self-contained `index.html`, served by GitHub Pages, with no build step and no dependencies other than four Google Fonts.

## What we are working on

| Repository | Language | What it is |
|---|---|---|
| [super-architect](https://github.com/MegaOverdriveCorp/super-architect) | JavaScript | Draw cloud architectures and database schemas in your browser. One HTML file, no server, no install, no account, Claude built in. Official Azure and Fabric icons, templates from Fabric medallion to AKS baseline, data models with keys and crow's foot relationships, SQL DDL and Mermaid export, three styles (one of them 16-bit) and three languages. |
| [new-york-pizza-korting](https://github.com/MegaOverdriveCorp/new-york-pizza-korting) | Python | Find the discount codes that apply to a New York Pizza order. A local proxy adds a Get JSON basket button to the web shop, tries the numeric codes in a range and reports the best code or combination. Never places an order. Python 3.12, uv, pytest, ruff. |
| MegaOverdriveCorp.github.io | HTML | This site. |
| .github | | The organisation profile README. |

Both product repositories are private at the time of writing.

## The style

The visual system behind the site, in short:

- **Palette**: night `#0B1020`, navy `#131A33`, teal `#1F5E6B`, lit window `#7FD8E8`, and one accent family (yellow `#FFD84A`, amber `#FFB020`, orange `#FF7A1A`, red `#E8402A`) used sparingly. Dark only.
- **Pixel discipline**: 4px grid, no border radius, no blur. Depth comes from bevels (light edge top-left, dark edge bottom-right) and hard 4px offset shadows. Gradients are replaced by 2x2 dither.
- **Type**: Pixelify Sans for display, Press Start 2P for HUD labels (10 to 12px, uppercase, short strings only), IBM Plex Sans for body, IBM Plex Mono for numbers.
- **Motion**: stepped animations only (`steps(3)`, `steps(4)`), 150 to 250 ms. One orchestrated moment on load: the wordmark flickers in and the skyline windows light up one by one. No sound, ever.
- **Scene**: seeded stars, a dithered horizon and a two-layer teal skyline with lit windows, parallaxed in 4px steps. Only on the title screen; working screens get a plain navy ground.

All of it lives inline in `index.html`. Copy the `:root` block and the `.mo-bevel` rule and you have the theme. The same 16-bit style ships as one of the three styles in Super Architect.

## Running it

Open `index.html` in a browser. That is the whole deployment procedure. GitHub Pages serves the `main` branch root.

## Contributing

Pull requests are welcome if they keep the pixels whole. Even pixel values, no `0.5px`, no `border-radius`, no `box-shadow` with blur, no em-dashes in copy.

## License

MIT for this site. The product repositories carry their own licenses.
