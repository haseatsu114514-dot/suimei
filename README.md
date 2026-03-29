# 四柱推命パーソナルツール

四柱推命の命式・大運・月運・日運を確認できるブラウザツールです。  
生年月日の直接入力を基本とし、必要なときだけ `今の年齢 + 誕生日` から補助入力できます。

## 機能
- 最大2人分の入力（本人必須、相手は任意）
- 四柱、蔵干、通変星、十二運、空亡、大運、月運、日運の表示
- 年齢 + 誕生日（月/日）からの補助入力
- 計算履歴の表示、検索、編集、削除
- 履歴の `JSON` 出力、`JSON` 取込
- `localStorage` に履歴保存
- 出生時間と出生場所から日本内時差を補正する機能

## 公開先

- GitHub Pages 公開先: `https://haseatsu114514-dot.github.io/seinengappi/`
- 実体ファイル: `index.html`
- `shichusuimei/index.html` は旧URLからルートへ戻すための転送ページです

## 使い方
1. `index.html` か公開URLを開く
2. 本人の生年月日を入力する
3. 必要なら相手も入力する
4. `命式を算出する` を押す
5. 結果は自動で履歴に保存される

## 日本内時差補正
1. `出生時間` を入力
2. `出生場所（都道府県）` を候補から選ぶ（未入力でも可）
3. `日本内時差を補正する` を押す
4. 地域時差と補正後時刻が表示される

補正式:
- `補正後時刻 = 出生時間 + ((出生地経度 - 135) × 4分)`
- 時差がプラスなら足し、マイナスなら引く（参照: `http://www.gero3p.sakura.ne.jp/files/jisa/maesetu.html`）

## GitHub Pages
1. GitHubのこのリポジトリで `Settings` → `Pages` を開く
2. `Build and deployment` の `Source` を `Deploy from a branch` に設定
3. `Branch` を `main` / `/ (root)` にして保存
4. 公開URL（例: `https://haseatsu114514-dot.github.io/seinengappi/`）を開く
5. ブラウザでお気に入り登録（Windows: `Ctrl + D`, Mac: `Command + D`）

## 補足
- オフラインでも `index.html` を直接開けば利用できます。
