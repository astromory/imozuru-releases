# macOS 検証用ビルド

macOS 版はまだ動作保証のある公開ベータではありません。
当面は検証協力者向けです。開発用リポジトリの閲覧権限が必要です。
GitHub Actions の `macOS build` から検証用 DMG を取得できます。

| Mac | Artifact |
| --- | --- |
| Apple Silicon（M1 以降） | `imozuru-macos-arm64` |
| Intel | `imozuru-macos-x64` |

ビルド設定の最低 OS は macOS 11.0 です。実際の対応 OS 範囲は実機検証後に確定します。
DMG を開き、Imozuru.app を Applications にコピーします。
WebView2 は不要で、macOS の WKWebView を使用します。

アプリは検証用の ad-hoc 署名のみで、Developer ID 署名・Apple の公証はありません。
ダウンロード経由の起動は Gatekeeper で制限される場合があります。
起動できない場合は表示内容を記録してください。
一般向け公開前に Developer ID 署名・公証とダウンロード後の起動を検証します。

## 検証項目

- DMG からのインストール、初回起動、終了、再起動
- フォルダ選択・ドロップ、写真一覧、検索、拡大と復帰
- 日本語・空白・記号を含むファイルの「Finderで表示」
- 写真へのアクセス許可、外付けドライブでの読み込み
- 表示設定・履歴の保存、前版からの更新
- 色管理、Retina での表示、大量写真での負荷

HEIC / HEIF は現在 Windows のデコーダーを使用する実装のため、macOS 版では未対応です。
そのほかの形式の制限は Windows 版利用ガイドに準じます。
利用条件は同梱の `TERMS.txt`、第三者ソフトウェアの条件は `THIRD-PARTY-NOTICES.txt` を参照してください。
不具合は https://github.com/astromory/imozuru-releases/issues へ、
Mac のチップ・macOS のバージョン・ビルド元のコミットまたはタグを添えて報告してください。
