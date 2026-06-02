# Web Effects Collector — 網頁特效蒐集器

一個純靜態的單頁「網頁特效蒐集器」:把全網與 GitHub 上最令人驚艷、開源、可直接拿來用的網頁特效彙整成一頁。每個特效都附 Demo、原始碼連結與「怎麼放進自己的網站」。

線上版:https://yazelin.github.io/web-effects-collector/

## 內容

- **90 個特效,分 12 類**:流體 / 液態模擬、GLSL Shader、Three.js / R3F 3D、捲動敘事、粒子系統、Codrops 創意 UI、生成藝術、純 CSS / Houdini、一行式 WebGL 背景、地球儀資料視覺、文字動畫、游標互動。
- 每張卡片:震撼度、技術標籤、Demo / GitHub 連結;可內嵌者能直接在頁面 iframe 預覽;附整合說明。
- 內建「立即跑跑看」Playground:零依賴 2D 星座粒子,加上 Vanta(NET / WAVES / BIRDS / GLOBE / FOG / HALO)與 tsParticles,點一下即時切換。

清單由多個 AI agent 並行檢索、再逐條對抗驗證連結真實性後彙整,資料存於 `data.js`。

## 怎麼跑

純靜態,無 build step。

- 直接用瀏覽器打開 `index.html`;或
- 起一個本機伺服器:`python3 -m http.server 8777`,再開 http://localhost:8777/

## 結構

- `index.html` — 全部 UI 與互動(內嵌 CSS / JS)
- `data.js` — 特效目錄資料(`window.EFFECTS_CATALOG`)
- `lib/` — 本機化的第三方函式庫,Playground 離線也能跑

## 第三方函式庫(皆 MIT 授權)

- three.js (r134) — https://github.com/mrdoob/three.js
- Vanta.js — https://github.com/tengbao/vanta
- tsParticles — https://github.com/tsparticles/tsparticles

目錄中收錄之各特效 / 專案,版權與授權歸原作者所有;本頁僅彙整連結與說明。
