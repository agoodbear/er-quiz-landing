# 急專大補帖 v2 — Project Website

[急專大補帖 v2](https://er-quiz-app-v2.vercel.app)（醫師國考急診專科刷題系統）的介紹網站與 36 秒推廣影片原始碼。

> **App repo:** [agoodbear/er-quiz-app-v2](https://github.com/agoodbear/er-quiz-app-v2) · **Live App:** <https://er-quiz-app-v2.vercel.app>

## Repo 結構

```
.
├── landing/            # Landing page（Vercel 部署目標）
│   ├── index.html      # 純 HTML + Tailwind CDN，單檔 SPA
│   └── assets/         # 影片 / OG cover / 圖
└── promo-video/        # HyperFrames 影片原始碼（HTML 編譯成 mp4）
    ├── index.html      # 36 秒 promo 影片 composition
    ├── design.md       # 視覺設計鎖定（暖調教學感、palette、typography）
    └── package.json    # `npm run dev` / `npm run check` / `npm run render`
```

## Landing page

純 HTML + Tailwind CDN + GSAP，單檔可移植。直接打開 `landing/index.html` 就能看。

**部署到 Vercel：** Project Settings → Root Directory 設成 `landing`；其餘預設即可（無 build step）。

## 影片重建

```bash
cd promo-video
npm install
npm run check         # lint + validate + inspect
npm run render -- -q high   # 30fps high-quality mp4
```

renders/ 不進 repo（檔案大），正式版 mp4 已 commit 到 `landing/assets/promo.mp4`。

## License

MIT — 跟主 app 相同。
