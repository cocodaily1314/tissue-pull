# 紙巾挑戰

限時手速超休閒：抽紙巾計張數，或者捲紙計長度——奶油風畫面、結果圖可下載分享 Threads。

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

亦可直接雙擊 `sheets.html` / `roll.html`（純 HTML+Canvas，毋須 build）。

## 一句玩法

- **抽紙挑戰（sheets.html）**：向上掃／拖抽出紙巾，計張數
- **卷紙挑戰（roll.html）**：任意方向拖曳開卷，計長度（cm／m）

各限時 **18 秒**，完場有結果卡＋「下載結果圖」。

## 點玩

1. 開 `sheets.html` 或 `roll.html`（或由 `index.html` 揀）
2. 撳開始 → 倒數 3 秒
3. 時間到 → 結果卡（成績、速率、港式評級）→ 「下載結果圖」

## 評分

| 模式 | 計分 | 港式評級（由低至高） |
|------|------|----------------------|
| 抽紙 | 完成上拉次數＝張數；速率＝張／秒 | 紙都未郁 → 手殘紙奴 → 街坊抽紙手 → 急症室級 → 紙巾粉碎機 → 全家裝清貨王 → 紙巾之神 |
| 卷紙 | 拖曳像素距離 × 0.05＝長度 cm；≥100cm 顯示為 m | 抹嘴都唔夠 → 街坊衛生標兵 → 廁紙刺客 → 捲紙馬拉松 → 連卷大王 → 廁紙傳說 |

計分跟住你嘅實際動作：冇抽／冇拖就唔會加分。

## 點分享

完場撳「**下載結果圖**」儲存直向 PNG，再上傳 Threads 挑戰朋友手速。兩個模式有獨立 URL，可直接分享其中一個。

## 檔案

- `index.html` — 選擇頁（連結兩個模式）
- `sheets.html` — 抽紙計張數（可直接玩）
- `roll.html` — 卷紙計長度（可直接玩）
- `game.js` — 舊版雙模式邏輯參考（頁面已自包含，毋須載入）
- `README.md` — 本說明

畫面美術為原創，無商標品牌名。
