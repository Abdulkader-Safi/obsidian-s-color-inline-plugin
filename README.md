# S-Color-Inline

An Obsidian plugin that puts a small color swatch next to any CSS color you write in inline code. Type `` `#0080ff` `` and you see the color right beside it.

It works in Live Preview and Reading view. Fenced code blocks are skipped on purpose, so a CSS file pasted into a note stays clean.

## Supported formats

| Format | Examples |
| --- | --- |
| Hex | `#0fa` `#ff0f` `#0080ff` `#ff008080` |
| RGB / RGBA | `rgb(128,128,128)` `rgba(0,255,255,0.5)` |
| HSL / HSLA | `hsl(150,50%,90%)` `hsla(32,100%,50%,0.8)` |

Case doesn't matter, so `RGB(...)` and `#FFF` work too. The color has to fill the whole code span: `` `#fff` `` gets a swatch, `` `color: #fff` `` does not.

## Install

### Manual

1. Download `main.js`, `manifest.json` and `styles.css` from the [latest release](https://github.com/Abdulkader-Safi/s-color-inline/releases/latest).
2. Put them in `<your vault>/.obsidian/plugins/s-color-inline/`.
3. Reload Obsidian and turn on S-Color-Inline under Settings > Community plugins.

### From source

```bash
git clone https://github.com/Abdulkader-Safi/s-color-inline.git
cd s-color-inline
npm install
npm run build
```

Use `npm run dev` to rebuild on every save while you work.

## Screenshots

| Theme | Light | Dark |
| --- | --- | --- |
| Default | ![Default theme, light](image/Default-Theme(Light-mode).png) | ![Default theme, dark](image/Default-Theme(Dark-mode).png) |
| [Minimal](https://github.com/kepano/obsidian-minimal) | ![Minimal theme, light](image/Minimal-Theme(Light-mode).png) | ![Minimal theme, dark](image/Minimal-Theme(Dark-mode).png) |
| [Things](https://github.com/colineckert/obsidian-things) | ![Things theme, light](image/Things-Theme(Light-mode).png) | ![Things theme, dark](image/Things-Theme(Dark-mode).png) |

## Credits

Based on [Inline Color Swatch](https://github.com/Suika225/inline-color-swatch) by Suika, released under MIT.

## License

MIT. See [LICENSE](LICENSE).
