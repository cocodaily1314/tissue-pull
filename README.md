# 紙巾挑戰

限時手速超休閒：抽紙巾計張數，或者捲紙計長度。柔和 off-white 3D（Three.js）、大字讀數、按住操作，結果圖可下載分享。

已分拆為兩個獨立可玩網頁，方便分開分享連結。

## GitHub Pages 連結

啟用 Pages（Source: Deploy from branch → `main` / root）後：

| 頁面 | URL |
|------|-----|
| 選擇頁 | https://cocodaily1314.github.io/tissue-pull/ |
| **抽紙計張數** | https://cocodaily1314.github.io/tissue-pull/sheets.html |
| **卷紙計長度** | https://cocodaily1314.github.io/tissue-pull/roll.html |

本地預覽：

```bash
cd tissue-pull
python3 -m http.server 8090
# 開 http://localhost:8090/sheets.html 或 /roll.html
```

純 HTML + CDN Three.js，毋須 build。

## 一句玩法

- **抽紙挑戰（sheets.html）**：按住畫面抽出紙巾，計張數
- **卷紙挑戰（roll.html）**：按住畫面拉出卷紙，計長度（cm／m）

各限時 **18 秒**，完場有結果卡＋「下載結果圖」。

## 點玩

1. 開 `sheets.html` 或 `roll.html`（或由 `index.html` 揀）
2. 撳開始 → 倒數 3 秒
3. 按住畫面狂抽／狂拉
4. 時間到 → 結果卡 → 「下載結果圖」

## 評分

| 模式 | 計分 | 港式評級（由低至高） |
|------|------|----------------------|
| 抽紙 | 按住期間累積張數；速率＝張／秒 | 紙都未郁 → 手殘紙奴 → 街坊抽紙手 → 急症室級 → 紙巾粉碎機 → 全家裝清貨王 → 紙巾之神 |
| 卷紙 | 按住期間累積長度 cm；≥100cm 顯示為 m | 抹嘴都唔夠 → 街坊衛生標兵 → 廁紙刺客 → 捲紙馬拉松 → 連卷大王 → 廁紙傳說 |

## 檔案

- `index.html` — 選擇頁
- `sheets.html` — 抽紙計張數（Three.js 紙巾盒）
- `roll.html` — 卷紙計長度（Three.js 卷紙）
- `game.js` — 舊版 Canvas 邏輯參考（頁面已自包含，毋須載入）
- `README.md` — 本說明

畫面美術為原創紙巾主題，無商標／軟雪糕抄襲元素。
