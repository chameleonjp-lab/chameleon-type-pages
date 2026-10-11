# カメレオン診断の公開用ファイル

公開URL: https://chameleonjp-lab.github.io/chameleon-type-pages/

このリポジトリは `chameleonjp-lab/chameleon_type` を正本とする配信ファイルの保存先です。`index.html`、`final/results.json`、`assets/chameleons/manifest.json`、全144件の512px透過WebPと深緑の共通アイコンをそろえます。制作原本、1280px透過PNG原稿、編集指示、原寸・一覧の確認記録と検査コードは実装元に保存しています。

結果画像は結果IDを鍵にした別manifestで管理し、結果JSONの再作成で対応が消えないようにします。元の139色・144結果と既存の `?result=1〜144` の番号対応を維持します。PNGとWebPは同じ144用途の書き出しです。

トップ、入力、結果の3画面に共通の注意書きをfooterで1回表示し、コピーライトは追加していません。画像は表示中の結果だけを読み込みます。

## 更新と公開確認

実装元の `scripts/sync-pages.cjs --target /path/to/this-worktree` で確認し、専用ブランチのクリーンな作業場所に `--apply` で同期します。表示に必要なファイルは同期対象ですが、このREADMEは公開用の運用説明として維持します。通常の同期は全144枚と共通アイコンの完成を要求します。スクリプトはコミット・push・マージ・公開設定変更を行いません。

継続Draft PR: [実装元 #18](https://github.com/chameleonjp-lab/chameleon_type/pull/18) / [公開用 #5](https://github.com/chameleonjp-lab/chameleon-type-pages/pull/5)

作業中に所有者が先行の途中版PR（実装元 #17 / 公開用 #4）をマージしました。継続PRにはその最新mainを取り込んでいます。今回の担当はmainへの直接保存やPRのマージをしていません。

所有者が継続PRをマージした後、両リポジトリの最新mainと配信ファイルを照合し、GitHub Pagesのデプロイ完了を確認してください。公開URLで全144番号の結果・基本色・実画像、トップ/入力の共通アイコン、最下部の注意書きを読み直し、画像の404や未完了表示がないことを確認する必要があります。ローカルのPR検査と最終144枚の公開反映確認は別です。

WebKitとChromiumの模擬検査をiPhone実機確認とは呼びません。iPhone Safari実機では縦横向き、文字拡大、日付選択、入力診断、相性リンク、再診断、共有・戻る操作、遅い回線での画像切替と最下部の注意書きを確認してください。
