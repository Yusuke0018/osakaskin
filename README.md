# osakaskin

売上分析ダッシュボード（自費・保険）用のシングルページです。`index.html` をブラウザで開くだけで動作し、CSVを読み込んで可視化します。

## 使い方
- `index.html` をブラウザで開き、CSVをアップロードします。
- 自費データはUTF-8、保険/傷病名はShift-JIS想定です。
- `sheet1_template.csv`（入力データ雛形）と `sheet2_template.csv`（集計テンプレート）を参考に作成してください。
- 取り込み確認や構造調査は `test-csv.html` で行えます。

## 動作要件
- オフラインで動作（外部CDN: Tailwind, PapaParse, Chart.js を使用）。
- 最新のChrome/Edge/Safariでの利用を想定。

## 開発/検証
- ローカルで開く: ファイルを直接ブラウザで開くか、簡易HTTPサーバで `index.html` を表示します。
- キャッシュやローカルストレージの影響があるため、更新時はリロードやストレージクリアを適宜実施してください。

## デプロイ（GitHub Pages例）
1. 本リポジトリの `Settings > Pages` で `Deploy from a branch` を選択。
2. `branch: main` / `folder: /(root)` を設定して保存。
3. 反映後、公開URLにアクセスして `index.html` を開きます。
