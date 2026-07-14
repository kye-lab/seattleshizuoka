# CLAUDE.md

## プロジェクト
シアトル静岡県人会 (Seattle Shizuoka Club) の公式LP。index.html 1枚の静的サイト。ビルド不要。

## 初回セットアップ(まだリポジトリがなければ実行)
1. gitを初期化し、全ファイルをコミットする
2. `gh auth status` で認証を確認。未認証ならユーザーに `gh auth login` を案内して完了を待つ
3. GitHubにパブリックリポジトリ `seattleshizuoka` を作成してpushする
4. GitHub Pagesを有効化する(mainブランチ / root)
5. 公開URLを確認してユーザーに報告する

## ドメイン
- カスタムドメイン: seattleshizuoka.org(2026-07-14設定済み)
- DNSはCloudflareで管理。Aレコード4件(185.199.108-111.153)とCNAME(www -> kye-lab.github.io)、いずれもDNS only(Proxyオフ)
- リポジトリのCNAMEファイルは設置済み
- 2026-07-14: サイト未完成のためGitHub Pagesを一時無効化中。再公開時は `gh api -X POST repos/kye-lab/seattleshizuoka/pages -f "source[branch]=main" -f "source[path]=/"` でPagesを有効化し、カスタムドメイン(cname=seattleshizuoka.org)とEnforce HTTPSを再設定する

## 今後の予定
- Facebookページ開設後、index.html内のコメント箇所にリンクを追加する

## 編集ルール
- 日本語と英語の併記を維持する
- emダッシュ(—)は使わない
- 誇張表現やbuzzwordは使わない。事実を簡潔に書く
- 変更はcommitしてpushする(Pagesには数分で反映される)
