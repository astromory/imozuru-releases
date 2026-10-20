# 芋づる写真館（Imozuru）

フォルダの奥の写真まで、まとめて眺める Windows 11 向け画像ビューアーです。
親フォルダを開くと、サブフォルダの写真もまとめて一覧表示できます。

**公開ベータを準備中です。現在、ダウンロードできる公開版はありません。**

## ダウンロード

配布が始まったら、[Releases](https://github.com/astromory/imozuru-releases/releases) の
「Pre-release」と表示された最新版から `Imozuru_…_x64-setup.exe` をダウンロードしてください。
`Source code` の ZIP / tar.gz はアプリ本体ではありません。

- 対応環境：Windows 11、x64（Intel / AMD）。Windows ARM は対象外です。
- WebView2 Runtime が必要です。未導入の場合、インストーラーがダウンロードします。
- 初期ベータはコード署名がありません。Windows に発行元不明の警告が表示される場合があります。
- 公開ベータのため、動作や表示に不具合が残っている可能性があります。

## できること

- サブフォルダを含む写真一覧、写真名・保存先の検索
- フォルダツリーで表示する範囲を選択
- 名前・保存場所・撮影日時による並べ替え、拡大表示
- JPEG / PNG / WebP / TIFF、対応する DNG・FITS の表示

原本を書き換える機能はありません。RAW 現像・写真編集・等倍ズームには対応していません。
HEIC / HEIF は追加コーデックに依存する試験的な対応です。

詳しい操作・制限・更新手順は [利用ガイド](USER-GUIDE.md) を参照してください。

macOS 版は Apple Silicon / Intel の検証用ビルドを準備しています。
Developer ID 署名・公証と実機検証は未完了です。[macOS 検証ガイド](MACOS-TESTING.md) を参照してください。

## 不具合・要望

[Issues](https://github.com/astromory/imozuru-releases/issues) から報告できます。
アプリのバージョン、Windows のバージョン、操作手順、期待した結果と実際の結果を記載してください。
Issues は公開されます。個人の写真や氏名を含むフォルダ名は、必要に応じて伏せてください。

このリポジトリは配布・不具合報告用です。アプリのソースコードは含みません。
