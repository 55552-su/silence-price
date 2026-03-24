# 沉默的代价 — 反校园霸凌互动剧情游戏

一款基于 H5 的互动视觉小说游戏，聚焦校园霸凌主题，通过沉浸式的剧情体验，让玩家在关键时刻做出选择，体会每一个决定带来的不同后果。

## 游戏特色

- **多分支剧情** — 约 70 个故事节点，玩家选择影响剧情走向
- **三种结局** — 最佳结局、良好结局、普通结局，取决于你的勇气与信任值
- **角色立绘** — AI 生成的高质量角色插画，多种表情变化
- **场景切换** — 教室、走廊、会议室、校门、天台等多个场景
- **背景音乐** — 6 首不同氛围的 BGM，随剧情自然过渡切换
- **适配移动端** — 针对微信内置浏览器优化，手机端体验流畅

## 部署方式

本游戏为纯静态网页，无需构建工具或后端服务。

### GitHub Pages 部署

1. 将本仓库上传到 GitHub
2. 进入仓库 **Settings** → **Pages**
3. Source 选择 **Deploy from a branch**，分支选 `main`，目录选 `/ (root)`
4. 保存后等待部署完成，即可通过 `https://<用户名>.github.io/<仓库名>/` 访问

### 其他静态托管

将所有文件上传到任意静态文件服务器（如 Nginx、Vercel、Netlify 等），确保所有文件在同一目录下即可。

## 文件结构

```
├── index.html              # 游戏主文件（含全部 HTML/CSS/JS）
├── v2_linxiao_*.png        # 林晓（主角）立绘
├── v2_xiaomeng_*.png       # 苏小萌 立绘
├── v2_zhaokai_*.png        # 赵凯 立绘
├── v2_prosecutor_*.png     # 陈检察官 立绘
├── v2_zhangyue_*.png       # 张悦 立绘
├── v2_teacher_*.png        # 王老师 立绘
├── scene_*.png             # 场景背景图
├── bgm_*.mp3               # 背景音乐
├── poster.png              # 游戏海报
├── poster_hd.png           # 游戏海报（高清版）
├── poster.html             # 海报源文件
├── qrcode_game.png         # 二维码占位图
└── README.md               # 本文件
```

## 音乐版权

背景音乐来自 [incompetech.com](https://incompetech.com)，作者 Kevin MacLeod，采用 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) 协议授权。

| 文件 | 曲目 |
|------|------|
| bgm_calm.mp3 | Morning |
| bgm_tense.mp3 | Shadowlands 1 - Horizon |
| bgm_dark.mp3 | Cryptic Sorrow |
| bgm_emotional.mp3 | Lasting Hope |
| bgm_hopeful.mp3 | Eternal Hope |
| bgm_ending.mp3 | Evening |

## 注意事项

- `qrcode_game.png` 为占位图，部署后请替换为实际游戏链接的二维码
- 游戏需要在 HTTPS 环境下运行以确保音频自动播放正常
- 推荐通过微信"扫一扫"访问，获得最佳体验
