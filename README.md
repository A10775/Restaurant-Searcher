# 簡易仕様書
## アプリ名
グルメサーチ
## 動作対象ブラウザ
Windows 11, GoogleChrome, Microsoft Edge（最新版）
## 動作方法
1. リポジトリをクローン
```
git clone https://github.com/A10775/Restaurant-Search.git
```
2. ディレクトリ移動
```
cd Restaurant-Search
```
3. Node.jsをインストール（npmコマンドが使える場合は問題ないです。）
4. "express-session"のインストール
```
npm install express-session
```
5. webアプリを起動（Macの場合は、ブラウザを開いて"http:localhost:3000"でアプリを開いてください。）
```
npm start
```
## 開発環境
Microsoft VS Code
## 開発言語
JavaScript
## フレームワーク
Node.js Express
## 使用したAPI
・Geolocation API
・ホットペッパー グルメサーチAPI
## 開発期間
10日間
## コンセプト
現在地付近の"今"食べたい店を検索できるWebアプリ！！
## 機能一覧
### 〇 検索条件入力画面：条件を指定し、レストランを検索。
・キーワード検索が可能（任意）。

・Geolocation APIを使って現在地を取得する。

・現在地からの検索半径をプルダウン形式で選択可能（必須）。

・現在地から検索ボタンをクリックすると、指定された条件で検索を行う。
### 〇 検索結果画面： 店舗検索結果を一覧形式で表示。

・"距離が近い順", "オススメ順"の二項目でソート可能。（デフォルトは距離が近い順）

・各店舗の"店舗名称", "ジャンル", "キャッチコピー", "交通アクセス", "サムネイル画像"を確認できる。

・店舗名称をクリックすると、店舗詳細を見ることができる。

・ページングに対応。
### 〇 店舗詳細画面：検索結果画面で選択したレストランの詳細を表示する。
・選択された店舗の"店舗名称", "住所", "営業時間", "定休日", "予算", "店舗URL"が確認できる。

・店舗URLをクリックすると、ホットペッパーグルメの店舗情報サイトから予約が可能。
## こだわったポイント
・食べたいジャンルや行きたい店舗を検索する機能は必要だと思ったので、キーワード検索を任意でできるように実装した。

・検索結果を距離が近い順だけでなく、オススメ順で並び替えることができるように実装した。

・店舗詳細画面では、予約や空き状況が確認できる店舗URLを記載し、実用性を上げた。
## デザイン面でこだわったポイント
・感覚的に操作できるように、複雑なデザインにならないようにシンプルに設計した。

・店のサムネイルを見てからジャンルやキャッチを読めるように、検索結果画面のレイアウトを設計した。

・代表的な食欲増進色と言われるオレンジで、健康的で楽しいイメージの色にした。

・ロゴをカジュアルで年齢を問わず目に留まるゴシック体の文字イメージにした。
## アドバイスして欲しいポイント
・検索条件入力画面が寂しいデザインになっているので、余白の使い方について。

・https化しようと試みたが、時間を待っても通信が保護されなかった点について。

・無料のホスティングサービスを用いてデプロイしようと試みたが、使用したフレームワークと嚙み合わず、ローカルでしか動かすことができなかった点。
## 自己評価
APIを使用したwebアプリ開発は初めてだったので、とても勉強になり身に付いた。
webアプリをデプロイしたかったが、できなかったことが悔しく感じた。
デザイン面では、背景色やフッダー、クレジット表記などのデザインについてはもっと勉強していかないといけないと感じた。
他人にアプリを実際に触ってもらい、客観的な違和感やアドバイスを反映することができたことは良かったと感じた。
