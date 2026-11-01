# 個人用 筋トレ・健康管理アプリ

複数端末でデータを同期できるPWAです。

## セットアップ（同期を使う場合）

1. [Firebase Console](https://console.firebase.google.com/) でプロジェクトを作成
2. Authentication を有効化（Email/Password）
3. Firestore Database を作成（テストモードでOK）
4. プロジェクト設定 > 一般 > マイアプリ から Web アプリを追加し、設定オブジェクトを取得
5. `index.html` 内の `firebaseConfig` を自分のものに置き換える
6. GitHub Pages で公開（Settings > Pages > main / root）

## 機能
- アカウント作成・ログイン（複数端末で同期）
- 今日のワークアウト + おすすめ動画
- 体重記録・グラフ
- 目標設定 → プラン自動提案
- YouTubeフォルダ（動画・再生リスト・チャンネル）
- 週間プラン編集
- カレンダー用 .ics 出力

データはログイン中はFirestoreに自動保存されます。
