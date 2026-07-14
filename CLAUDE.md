# CLAUDE.md

## プロジェクト
シアトル静岡県人会 (Seattle Shizuoka Club) の公式LP。index.html 1枚の静的サイト。ビルド不要。

## 初回セットアップ(まだリポジトリがなければ実行)
1. gitを初期化し、全ファイルをコミットする
2. `gh auth status` で認証を確認。未認証ならユーザーに `gh auth login` を案内して完了を待つ
3. GitHubにパブリックリポジトリ `seattleshizuoka` を作成してpushする
4. GitHub Pagesを有効化する(mainブランチ / root)
5. 公開URLを確認してユーザーに報告する

## 今後の予定
- カスタムドメイン seattleshizuoka.org を取得予定。取得後にCNAME設定を行い、レジストラに入力するDNSレコードをユーザーに案内する
- Facebookページ開設後、index.html内のコメント箇所にリンクを追加する

## 編集ルール
- 日本語と英語の併記を維持する
- emダッシュ(—)は使わない
- 誇張表現やbuzzwordは使わない。事実を簡潔に書く
- 変更はcommitしてpushする(Pagesには数分で反映される)
