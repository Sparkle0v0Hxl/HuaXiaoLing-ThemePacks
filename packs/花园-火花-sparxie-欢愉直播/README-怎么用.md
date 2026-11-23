# 火花 · 欢愉直播（主题包 v1）

火花的角色主题包：**18 张图 + 一份 theme.json**，整套换图换配色。
素材取自官方角色立绘与官方光锥「花花世界迷人眼」，抠图后按启动器图位重新构图。

> 角色身份提醒：**火花（sparxie，五星·欢愉）和花火（sparkle）是两个不同角色**，
> 本包只使用火花的素材，不要和「花火 · 幻梦剧场」包混用。

## 怎么装

1. 打开启动器 → 设置 → 外观 → 主题包 → 点「主题包文件夹」。
2. 把整个 `花园-火花-sparxie-欢愉直播` 文件夹复制进去（要在 `art-pack` 目录下，目录名就是这个包的 id）。
3. 回到设置页点「重新扫描」，选中「火花 · 欢愉直播」。

便携版的 `art-pack` 在 `<启动器目录>\data\art-pack\`，
安装版在 `%APPDATA%\花筱灵启动器\art-pack\`。

## 这个包里有什么

18 张图 + `theme.json`。`theme.json` 里：

| 字段 | 本包的值 | 作用 |
| --- | --- | --- |
| `name` | 火花 · 欢愉直播 | 设置页显示的名字 |
| `author` | 花筱灵启动器 | 作者 |
| `description` | 银白双马尾、红黑菱格礼服与粉紫直播夜色 | 设置页说明 |
| `skin` | `sakura`（樱霞） | 界面皮肤，可选 15 套之一 |
| `accent` | `spark`（暖红） | 强调色预设，可选 8 个之一 |
| `colors` | 见下 | 逐项覆盖 `accent` / `accent2` / `bg` / `surface` / `text` / `muted` / `gold` |

本包配色：

| 键 | 值 | 说明 |
| --- | --- | --- |
| `accent` | `#ff5c8a` | 主强调色（玫红） |
| `accent2` | `#ffb0cc` | 次强调色（浅粉） |
| `bg` | `#140a14` | 页面底色 |
| `surface` | `#231029` | 卡片/面板底色 |
| `text` | `#fbeef7` | 正文文字 |
| `muted` | `#a992ac` | 次要文字 |
| `gold` | `#ffd98a` | 点缀色 |

`colors` 只接受 `#rgb`、`#rrggbb`、`#rrggbbaa`、`rgb(…)`、`rgba(…)` 这几种写法，其他一律忽略。

## 图位清单（18 张，全是可选的，缺哪张就回落内置图）

```
character.png        1536×1536  首页 hero 背景（角色 + 氛围底光）
character-face.png    500×500   头像 / 小圆标（圆内裁切，脸已对准）
sparkle-hero.png      914×900   首页 hero 区竖图
sparkle-mask.png      512×512   页面挂饰（大幅）
sparkle.png           376×512   小图标（立绘头部特写）
sparxie.png           376×512   小图标（光锥头部特写，另一套）
sparkle-figure.png    376×482   空态小图
sparkle-fullbody.png  697×820   双角色卡左图
sparxie-fullbody.png  689×820   双角色卡右图
sparxie-charm.png     512×512   页面挂饰（光锥小图，柔化处理）
charm-fireworks.png   512×512   小挂饰 · 烟花
charm-flame.png       512×512   小挂饰 · 心焰
charm-stars.png       512×512   小挂饰 · 星芒
char-cool.png         900×1350  角色立绘（活泼型）
char-sweet.png        900×1350  角色立绘（甜美型）
char-book.png         900×1350  页面右侧淡背景立绘
charm-dock.png       512×512   启动页·左挂饰（11-22 新增图位）
char-portrait.png    500×500   启动页·右立绘（11-22 新增图位）
```

## 注意

- 包里的同名文件会盖住内置那张（这是主题包的本意）；不想盖就把那张删掉，会自动回落。
- 换包/删包后启动器会自动校准：包没了就回落到内置，不会白屏。
- 素材来自官方立绘与光锥，仅作本地主题包示例使用，请勿二次分发。
