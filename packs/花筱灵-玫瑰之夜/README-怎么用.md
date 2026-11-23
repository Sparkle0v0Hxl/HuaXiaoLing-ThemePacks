# 花筱灵 · 玫瑰之夜（示例主题包 v1）

这是「主题包」体系的示例：**图片沿用内置那套，只换一套整体配色**。
同一个包里也可以放自己的图 —— 详见最后一节。

## 怎么装

1. 打开启动器 → 设置 → 外观 → 主题包 → 点「主题包文件夹」。
2. 把整个 `花筱灵-玫瑰之夜` 文件夹复制进去（要在 `art-pack` 目录下，目录名就是这个包的 id）。
3. 回到设置页点「重新扫描」，选中「花筱灵 · 玫瑰之夜」。

便携版的 `art-pack` 在 `<启动器目录>\data\art-pack\`，
安装版在 `%APPDATA%\花筱灵启动器\art-pack\`。

## 这个包里有什么

只有 `theme.json` 一个文件。里面：

| 字段 | 作用 |
| --- | --- |
| `name` / `author` / `description` | 设置页里显示的名字和说明 |
| `skin` | 界面皮肤（`rose` = 沙漠玫瑰，可选 15 套之一） |
| `accent` | 强调色预设（`rose` = 玫瑰粉，可选 8 个之一） |
| `colors` | 逐项覆盖：`accent` / `accent2` / `bg` / `surface` / `text` / `muted` / `gold` |

`colors` 只接受 `#rgb`、`#rrggbb`、`#rrggbbaa`、`rgb(…)`、`rgba(…)` 这几种写法，其他一律忽略。

## 想换自己的图？

把 png 放进同一个目录，文件名必须是下面这些之一（缺哪张就自动用内置图）：

```
character.png        首页大图里的角色（也是侧栏头像）
character-face.png   头像 / 小圆标
sparkle-hero.png     首页 hero 区右侧
sparkle-mask.png     页面挂饰（花火）
sparkle.png          小图标
sparkle-figure.png   小立绘
sparkle-fullbody.png 竖构图底图
sparxie-fullbody.png 竖构图底图（另一套）
sparxie.png          小图标（另一套）
sparxie-charm.png    页面挂饰（火花）
charm-fireworks.png  小挂饰 · 烟花
charm-flame.png      小挂饰 · 火焰
charm-stars.png      小挂饰 · 星芒
char-cool.png        双角色卡·花火（活泼型立绘）
char-sweet.png       双角色卡·火花（甜美型立绘）
char-book.png        页面右侧淡背景立绘
```

## 注意

- 主题包里的图**不会**替换你自己设置的 `character.png` / `character-face.png` 之外的任何用户素材，
  但如果你在包里放了同名文件，它就会盖住内置那张（这是主题包的本意）。
- 换包/删包后启动器会自动校准：包没了就回落到内置，不会白屏。
