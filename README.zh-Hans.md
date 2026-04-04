# Polycarbonate Dark Theme

把Zed变成一块干净透明的暗色玻璃板

## 包含主题

- Polycarbonate sha1
- Polycarbonate Ayu Dark
- Polycarbonate Gruvbox Dark
- Polycarbonate One Dark

## 预览

![Polycarbonate sha1](./assets/1.webp)

![Polycarbonate Ayu Dark](./assets/2.webp)

![Polycarbonate Gruvbox Dark](./assets/3.webp)

## 安装

1. 打开Zed扩展页面
2. 搜索`Polycarbonate Dark`
3. 点击安装

## 搭配TranslucentTB

搭配[TranslucentTB](https://github.com/TranslucentTB/TranslucentTB)使用时，推荐将accent设为`clear`，color设为`#000000DD`(8 bpc)或`#000000EE`(10 bpc)。这将使Zed和Windows任务栏融为一体，如预览所示

## 常用自定义项

```jsonc
"experimental.theme_overrides": {
  "background": "#110D", //背景色，默认为#000D
  "title_bar.background": "#110D", //顶部标题栏背景色，默认为#000D
  "status_bar.background": "#110D", //底部状态栏背景色，默认为#000D

  "tab.active_background": "#057", //活动中标签页背景色，默认为#000

  "search.match_background": "#333", //搜索匹配项背景色，默认为#333
  "search.active_match_background": "#666", //活动搜索匹配项背景色，默认为#666

  "players": [{ "selection": "#6AD8" }], //划取区域的颜色
  "syntax": {
    "comment": {
      "color": "#7D7", //注释前景色
      "background_color": "#0001", //注释背景色
    },
  },
}
```

## 10 bpc

在10 bpc下，Windows Multi Panel Overlay (MPO)功能可能出现显卡驱动错误计算透明度bug，该bug会导致的窗口实际透明度高于设置透明度。除了Zed的原生透明度设置外，[VSCode skacekachna.win-opacity插件](https://marketplace.visualstudio.com/items?itemName=skacekachna.win-opacity)、[foobar2000](https://www.foobar2000.org/)以及TranslucentTB都受此bug影响

该bug在NVIDIA和AMD显卡上都可能出现，且一直没有不降低渲染性能的解决方案。因此，我专门为每种配色方案做了10 bpc适配

如果您认为本插件的默认透明度过高，那多半就是出现了该bug。请使用10 bpc版本

如果您对该bug有任何解决方案，请随时联系我

如果您认为本theme的配色需要改进，请随时提交ISSUE
