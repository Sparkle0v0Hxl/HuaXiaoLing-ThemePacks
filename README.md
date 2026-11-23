# 花筱灵启动器 · 主题包

![主题包](https://img.shields.io/badge/%E4%B8%BB%E9%A2%98%E5%8C%85-5%20%E5%A5%97-e79ad0)
![格式](https://img.shields.io/badge/%E6%A0%BC%E5%BC%8F-18%20%E5%9B%BE%E4%BD%8D%20%2B%20theme.json-9b8cff)
![许可](https://img.shields.io/badge/%E4%BB%85%E9%99%90%E6%9C%AC%E6%9C%BA%E8%87%AA%E7%94%A8-%E8%AF%B7%E5%8B%BF%E4%BA%8C%E6%AC%A1%E5%88%86%E5%8F%91-ffb86b)

「花筱灵启动器」的外观主题包集合。**主题包不随安装包分发**，这个仓库就是它们的家：下载、解压、丢进 `art-pack` 文件夹，启动器重启一下就换整套外观。

> 启动器里也有直达入口：**设置 → 外观 → 主题包 → 「下载主题包」**，或者直接打开 <https://37l2m9tz2jw0adtxxq1.traesite.cn/index.html>。

---

## 现在有哪些包

| 主题包 | 角色 | 皮肤 / 强调色 | 体积 |
| --- | --- | --- | --- |
| `太卜-符玄-fuxuan-太卜司` | 符玄 · 太卜司 | `rose` / `rose` | 6.8 MB |
| `幻梦-花火-sparkle-幻梦剧场` | 花火 · 幻梦剧场 | `midnight` / `violet` | 6.9 MB |
| `星穹-大黑塔-herta-星穹观测` | 大黑塔 · 星穹观测 | `galaxy` / `violet` | 8.0 MB |
| `花园-火花-sparxie-欢愉直播` | 火花 · 欢愉直播 | `sakura` / `spark` | 7.5 MB |
| `花筱灵-玫瑰之夜` | 花筱灵 · 玫瑰之夜 | `rose` / `rose` | 只有 `theme.json`，纯换配色 |

前四套是完整的 18 图位 + 配色；`花筱灵-玫瑰之夜` 是示例包，图片沿用内置那套，只改配色 —— 想自己做主题包的话，从它起步最省事。

---

## 怎么装

**方式一：从仓库下载（推荐）**

点右上角 `Code → Download ZIP` 把整个仓库下下来，解压后把 `packs` 里想要的包整个文件夹复制过去。

**方式二：只下某一个包**

进 `packs/<包名>/`，逐个下载里面的文件，按原目录结构放进 `art-pack/<包名>/`。目录名就是包 id，别改。

**放到哪**

| 版本 | `art-pack` 位置 |
| --- | --- |
| 便携版 | `<启动器目录>\data\art-pack\` |
| 安装版 | `%APPDATA%\花筱灵启动器\art-pack\` |

启动器里 **设置 → 外观 → 主题包 → 「打开文件夹」** 会直接帮你打开这个目录，不用自己找。

**最后一步**

回到设置页点 **「重新扫描」**，列表里就会出现新包，点一下即生效。

---

## 主题包里有什么

一套完整主题包 = **18 张 PNG + 一份 `theme.json`**，全是可选的：缺哪张就回落内置那张，不会白屏。

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
charm-dock.png        512×512   启动页 · 左挂饰
char-portrait.png     500×500   启动页 · 右立绘
```

`theme.json` 字段：

| 字段 | 作用 |
| --- | --- |
| `name` / `author` / `description` | 设置页里显示的名字、作者、说明 |
| `version` | 包自己的版本号 |
| `skin` | 界面皮肤，15 套可选（`rose`、`midnight`、`galaxy`、`sakura`…） |
| `accent` | 强调色预设，8 个可选（`rose`、`violet`、`spark`…） |
| `colors` | 逐项覆盖 `accent` / `accent2` / `bg` / `surface` / `text` / `muted` / `gold` |

`colors` 只接受 `#rgb`、`#rrggbb`、`#rrggbbaa`、`rgb(…)`、`rgba(…)` 这几种写法，其他一律忽略。

**同名文件会盖住内置那张** —— 这就是主题包的本意。不想盖就把那张删掉，自动回落。

---

## 自己做一套

1. 复制 `packs/花筱灵-玫瑰之夜` 改成你要的目录名（全小写、别带空格更稳）。
2. 改 `theme.json` 里的 `name` / `description` / 配色。
3. 往目录里丢图片，文件名照上表。尺寸不严格，但比例最好一致，否则会被裁。
4. 复制进 `art-pack`，设置页点「重新扫描」。

启动器还有 **「新建空白包」** 和 **「复制当前包」** 两个按钮，也可以从界面里直接起一套。

---

## 版权

启动器的**界面与代码**为原创实现；这 5 套主题包里用到的**官方立绘、光锥图**，版权归米哈游及各游戏官方 / 原作者所有。

这些包是爱好者做的主题示例，**不是官方授权产品**，仅供本机自用：

- 请**不要**二次分发、上传网盘、发布到别的公开仓库或拿去商用；
- fork 这个仓库只为了自己改着玩没问题，别把改好的包再公开分享；
- 官方要删，说一声立刻就撤。

启动器的功能设计参考了 [Starward](https://github.com/Scighher/Starward)（MIT）等开源启动器，不包含它们的代码或素材。

---

## 相关链接

- 启动器源码：[GitHub](https://github.com/Sparkle0v0Hxl/HuaXiaoLing-Launcher) ｜ [Gitee](https://gitee.com/SparkleHxl/HuaXiaoLing-Launcher)
- 最新版本下载：[GitHub Releases](https://github.com/Sparkle0v0Hxl/HuaXiaoLing-Launcher/releases/latest)
- 主题包需要 2.13.0 及以上版本（2.13.0 才有的 18 图位体系）
