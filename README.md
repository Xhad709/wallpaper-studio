# 叠卡壁纸工坊

在线体验：[打开壁纸工坊](https://xhad709.github.io/wallpaper-studio/)

在浏览器里做分层纸卡风格的手机锁屏壁纸：选配色、改文字、换字体，导出高清 PNG。

- 3 种版式：叠纸、框格三段、框格两段
- 6 套预设配色，外加随机配色
- 30 款字体：23 款来自 Google Fonts（英文无衬线、衬线、手写、花体、等宽，以及 8 款中文），另有 7 款来自国内字体站的中文字体（霞鹜文楷、得意黑、江城圆体、猫啃网糖圆、云峰寒蝉体、朱雀仿宋、京华老宋体）。标题、副标题、小字可以分别设置字体
- 可以调纸纹、光影、圆角、卡片高度，分割线样式也能改
- 内置常见 iPhone 和安卓分辨率，也可以自定义尺寸

整个工具只有一个 `index.html` 文件，不用安装任何东西。

## 发布到 GitHub Pages

1. 在 GitHub 新建一个公开仓库，比如取名 `wallpaper-studio`。
2. 在仓库页面点 **Add file → Upload files**，把 `index.html`（还有这个 `README.md`）拖进去，然后点 **Commit changes**。
3. 进入 **Settings → Pages**，Source 选 **Deploy from a branch**，Branch 选 `main`、目录选 `/ (root)`，然后点 **Save**。
4. 等一两分钟，网址就是 `https://你的用户名.github.io/wallpaper-studio/`。

## 保存图片

- 电脑：点“保存 PNG”会直接下载。
- 手机：点“保存 PNG”后会弹出大图，长按图片即可存到相册。

## 字体来源

字体都在后台加载，不会拖慢页面打开。每一组字体都会按顺序尝试多个来源，哪个能用就用哪个：

| 字体 | 依次尝试的来源 |
| --- | --- |
| Google 字体（23 款） | fonts.googleapis.com → fonts.googleapis.cn（Google 中国节点）→ fonts.loli.net（镜像） |
| 霞鹜文楷、得意黑 | registry.npmmirror.com → cdn.jsdelivr.net → fontsapi.zeoseven.com |
| 其余 5 款中文字体 | fontsapi.zeoseven.com（ZeoSeven Fonts） |

字体设置下方会显示当前实际用的是哪个来源。某款国内字体站的字体如果所有来源都加载失败，它会从列表里隐藏；Google 字体全部失败时会改用系统字体，功能不受影响。

以上字体大多采用 OFL-1.1 开源协议。京华老宋体和云峰寒蝉体用的是作者自定的协议，都允许免费商用和网页嵌入。
