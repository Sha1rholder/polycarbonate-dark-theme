[简体中文](./README.zh-Hans.md)

# Polycarbonate Dark Theme

Turn Zed into a clean slab of dark glass.

## Included Themes

- Polycarbonate sha1
- Polycarbonate Ayu Dark
- Polycarbonate Gruvbox Dark
- Polycarbonate One Dark

## Preview

![Polycarbonate sha1](./assets/1.webp)

![Polycarbonate Ayu Dark](./assets/2.webp)

![Polycarbonate Gruvbox Dark](./assets/3.webp)

## Installation

1. Open the Zed extensions page
2. Search for `Polycarbonate Dark`
3. Click install

## Using with TranslucentTB

When using it with [TranslucentTB](https://github.com/TranslucentTB/TranslucentTB), it is recommended to set the accent to `clear` and the color to `#000000DD` (8 bpc) or `#000000EE` (10 bpc). This will seamlessly blend Zed with the Windows taskbar, as shown in the preview.

## Common Customizations

```jsonc
"experimental.theme_overrides": {
  "background": "#110D", // Background color, defaults to #000D
  "title_bar.background": "#110D", // Top title bar background color, defaults to #000D
  "status_bar.background": "#110D", // Bottom status bar background color, defaults to #000D

  "tab.active_background": "#057", // Active tab background color, defaults to #000

  "search.match_background": "#333", // Search match background color, defaults to #333
  "search.active_match_background": "#666", // Active search match background color, defaults to #666

  "players": [{ "selection": "#6AD8" }], // Selection area color
  "syntax": {
    "comment": {
      "color": "#7D7", // Comment foreground color
      "background_color": "#0001", // Comment background color
    },
  },
}
```

## 10 bpc

At 10 bpc, the Windows Multiplane Overlay (MPO) feature may trigger a graphics driver bug that incorrectly calculates transparency, resulting in the actual window transparency being higher than the configured setting. In addition to Zed's native transparency settings, the [VSCode skacekachna.win-opacity extension](https://marketplace.visualstudio.com/items?itemName=skacekachna.win-opacity), [foobar2000](https://www.foobar2000.org/), and TranslucentTB are all affected by this bug.

This bug can occur on both NVIDIA and AMD graphics cards, and there is currently no solution that does not compromise rendering performance. Therefore, I have specifically made 10 bpc adaptations for each color scheme.

If you find the default transparency of this theme too high, it is highly likely that you are encountering this bug. Please use the 10 bpc versions.

If you have any solutions to this bug, please contact me.

If you believe the color scheme of this theme needs improvement, please submit an ISSUE.
