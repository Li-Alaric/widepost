# Widepost Beta — 视频上传打卡器 / Video Upload Tracker

**中文** | [English](#english)

---

## 这是什么

Widepost 是一个 Windows 桌面小工具，帮你记住一件事：**这个视频我到底发过没有？**

它的工作方式很简单：

1. 选一个放视频的文件夹，它自动把里面的视频列成一张表
2. 你给每个常用的平台起个名字、填上它的上传页网址（比如"B站" + bilibili 的投稿页链接）
3. 某天把视频传上去了，就在对应的格子上**双击打钩**——它会记下日期，并自动打开那个平台的 upload 页面
4. 以后随时回来查：哪些发了、哪些没发、哪天发的

所有记录保存在你自己的电脑上，仅此而已。

> 这是 Beta 版，免费使用，可能还有粗糙的地方，欢迎反馈。

## 快速上手（4 步）

1. **下载** `WidepostBeta.exe`（在右侧 [Releases](../../releases/latest) 页面）
2. **放到任意文件夹**（桌面或 D 盘都行，不要放 C:\Program Files）
3. **双击运行**——第一次打开会让你填平台名和网址，照提示填一两个你常用的就行
4. **选视频文件夹**（顶部「切换目录」按钮），列表出来后就能开始打卡

## 系统要求

- Windows 10 / 11（64 位或 32 位均可）
- 无需安装任何运行库（系统自带）

## 数据存在哪？

数据保存在 **`文档\Widepost\`** 文件夹里，不在软件目录里：

- 换新版本：直接用新 exe 替换旧的，数据自动还在
- 备份：把 `文档\Widepost` 整个文件夹复制走，就是完整备份
- 老版本升级：第一次打开新版会问你"检测到旧数据，要导入吗"，点「是」即可

## 隐私

- **不联网收集任何数据**：没有账号、没有统计、没有遥测
- **启动时会检查一次新版本**（只访问 GitHub 的公开接口，不发送任何个人信息、视频名或路径）；其余时间完全离线
- 你的视频路径、平台网址、打卡记录只存在你自己的电脑上

## 遇到"Windows 已保护你的电脑"？

因为软件没有购买代码签名证书（个人开发者，Beta 阶段），Windows SmartScreen 可能会提示。**点「更多信息」→「仍要运行」**即可。软件就一个 170KB 的 exe，不装驱动、不写注册表；除了启动时那一次版本检查，其余时间不联网。

## 反馈问题

请到 [Issues](../../issues) 页面提交，描述一下做了什么操作、出现了什么。中英文都可以。

## 许可

免费供个人使用，不可再分发、不可修改、不可用于商业用途。详见 [LICENSE](LICENSE)。

---

<a name="english"></a>

## What is this

Widepost is a small Windows desktop tool that answers one question: **"Did I already upload this video or not?"**

How it works:

1. Point it at a folder of videos — it lists them all in one table
2. Name your platforms and paste each platform's upload-page URL (e.g. "YouTube" + youtube.com/upload)
3. When you upload a video somewhere, **double-click the matching cell** — it ticks the box, records today's date, and opens that platform's upload page
4. Come back any time to see what's published, what's not, and when

All records stay on your own machine. That's it.

> This is a free Beta. Rough edges are expected — feedback welcome.

## Quick start (4 steps)

1. **Download** `WidepostBeta.exe` from the [Releases](../../releases/latest) page
2. **Put it anywhere** (Desktop or D:\ is fine — do NOT put it in C:\Program Files)
3. **Double-click to run** — on first launch it asks for a platform name and its upload-page URL; add one or two you actually use
4. **Choose your video folder** (the "Folder" button) — once the list shows up, start ticking

## Requirements

- Windows 10 / 11 (64-bit or 32-bit)
- No runtime installation needed (everything is built into Windows)

## Where is my data?

Data lives in **`Documents\Widepost\`**, not next to the exe:

- Upgrading: replace the old exe with the new one — data stays
- Backup: copy the whole `Documents\Widepost` folder — that's a complete backup
- Upgrading from older versions: the new build asks "old data found — import it?" once; click Yes

## Privacy

- **No data is ever collected**: no account, no analytics, no telemetry
- **A version check runs once at startup** — it only calls GitHub's public API and sends no personal information, video names, or paths; otherwise the app is fully offline
- Your video paths, platform URLs and tick records never leave your machine

## "Windows protected your PC"?

The app has no code-signing certificate (solo developer, beta stage), so SmartScreen may warn you. **Click "More info" → "Run anyway".** The whole app is a single 170KB exe — no drivers, no registry writes, and no network access except that one startup version check.

## Feedback

Please open an [Issue](../../issues). Tell me what you did and what happened. English or Chinese, both fine.

## License

Free for personal use. No redistribution, modification or commercial use. See [LICENSE](LICENSE).
