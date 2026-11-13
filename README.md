# Colorfigures 系列互动网页

由 Doomsday_Envoy 制作与维护的 Colorfigures 系列互动科普网页。

在线访问：<https://doomsday-envoy.github.io/colorfigures/>

## 已收录作品

- `01 T4噬菌体DNA注入`：演示 T4 噬菌体识别宿主、锁定基板、收缩尾鞘并向大肠杆菌注入双链 DNA 的过程。
- `02 微量移液器`：拖动移液器按手稿吸取“蓝屏露”“红温汤”和“黏菌汽水”；三次操作失误会触发 `WASTED` 钢印，正确配比则经历消散烟雾、金色溶液和延迟爆炸。

## 使用方式

直接打开根目录的 `index.html`，页面默认展示第一项作品。桌面端使用页面左侧留白处的作品目录切换内容；窄屏时目录会移到页面上方。

增加新作品时：

1. 将独立 HTML 页面放进 `figures/`。
2. 在 `index.html` 的作品目录中复制一个按钮。
3. 填写唯一的 `data-id`，并将 `data-src`、`data-title` 指向新页面。

页面不依赖外部脚本或 CDN，可在本地直接打开，也可作为静态站点发布。

## 字体

作品目录页、T4 页面和微量移液器互动页统一使用 `GNU Unifont 18.0.01`
的 WOFF2 子集，访客不需要安装像素字体。

- 字体文件：`assets/fonts/unifont-gallery-subset.woff2`
- 字体覆盖作品目录、T4 和微量移液器三个页面实际使用的字符
- 字体加载使用 `font-display:block`，避免先显示系统字体再切换
- Colorfigures SVG 标签统一改为 Unifont，并收紧少量字距防止标注溢出

如果后续作品增加了当前字体子集未包含的字符，需要重新生成字体子集。

## 许可与署名

- 本站页面代码和文档：仓库根目录 `LICENSE` 中的 GNU GPL v3.0。
- Colorfigures：MIT License，作者 April Zhu。互动页面基于 Colorfigures 制作，完整许可见 [licenses/Colorfigures-MIT.txt](licenses/Colorfigures-MIT.txt)。
- GNU Unifont 18.0.01：SIL Open Font License 1.1。字体版权归 Roman Czyborra、Paul Hardy、Qianqian Fang 等作者所有；本项目发布的是按网页字符裁切后的 WOFF2 子集。完整许可见 [licenses/GNU-Unifont-OFL-1.1.txt](licenses/GNU-Unifont-OFL-1.1.txt)。

Colorfigures 项目：<https://april-zhu.com/colorfigures>

GNU Unifont 项目：<https://unifoundry.com/unifont/>
