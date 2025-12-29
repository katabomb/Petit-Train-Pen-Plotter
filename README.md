### 1. `drawing_to_abz.html`
- iPad / PC で線を描くためのアプリ  
- 描いた軌跡を **α, β, z の数値データ**に変換して出力します
- 出力形式は textarea（CSV 相当）です

### 2. `plotter_abz_cam.html`
- α, β, z の数値データから  
  **ペンプロッタ用のカム形状**を生成するアプリ
- 描画結果やカム形状をその場で確認できます

### 3. `index.html`（ハブ）
- 上記 2 つのアプリを **左右に並べて表示**
- `drawing_to_abz` の出力を  
  ワンクリックで `plotter_abz_cam` に転送
- データは localStorage にも保存されます

---

## ▶ 使い方

1. `index.html` をブラウザで開く  
2. 左側（drawing）で線を描く  
3. 「Drawing出力 → Plotter入力へ転送」をクリック  
4. 右側（plotter）でカム形状を生成・確認  

※ 3 ファイルは **同じフォルダ**に置いてください。

---

## 🌐 公開方法（GitHub Pages）

- [https://katabomb.github.io/Petit-Train-Pen-Plotter/](https://katabomb.github.io/Petit-Train-Pen-Plotter/)

---

## 💡 想定用途

- 100均ペンプロッタ
- 自作リンク機構・カム機構の検討
- iPad + ブラウザだけで完結する作図〜機構設計
- 教育用途・ワークショップ用デモ

---

## 🛠 技術メモ

- すべて **HTML + JavaScript のみ**
- サーバー不要
- iframe を利用した同一オリジン連携
- PC / iPad / タブレット対応

---

## 📜 ライセンス

個人利用・改変・再配布は自由です。  
研究・教育・工作用途でご活用ください。
