# 環境設定をリセット

Aseprite の環境設定は[環境設定フォルダ](preferences-folder.md)の `aseprite.ini` ファイルに保存されています。環境設定フォルダは *編集 > 環境設定 > 一般 > 設定ファイルの場所* で開くことができます。全ての環境設定をリセットするには、Aseprite を終了してから、`aseprite.ini` のあるフォルダの中身を全て消してください。

![Files in Preferences Folder](preferences/preffiles.png)

Aseprite が起動しないときには、以下のプラットフォームごとの手順で設定をリセットしてください。

## Windows

1. Aseprite を閉じます
1. <kbd>Windowsキー + R</kbd>キー（または、`スタートメニュー > ファイル名を指定して実行...`)を押します。これによって、プログラムを実行するためのダイアログが開きます。そこに以下のように入力してください。

       %AppData%\Aseprite

   そして `Enter` キーを押してください。
1. 開いたフォルダの中のファイルを消してください（主に `aseprite.ini`）
1. Aseprite を再起動してください

## macOS

1. Aseprite を閉じます
1. Spotlight 検索を開きます (⌘Space)
1. 以下のテキストをコピーして `~/Library/Application Support/Aseprite` ⌘V で貼り付けて Enter を押します

   ![Spotlight Search](preferences/spotlight.png)

1. 開いたフォルダの中のファイルを消してください（主に `aseprite.ini`）
1. Aseprite を再起動してください

## Linux

1. Aseprite を閉じます
1. ターミナルを開きます
1. 以下のコマンドを打ちます

       xdg-open ~/.config/aseprite

1. 開いたフォルダの中のファイルを消してください（主に `aseprite.ini`）
1. Aseprite を再起動してください

---

**SEE ALSO**

[トラブルシューティング](troubleshooting.md) |
[環境設定フォルダ](preferences-folder.md)
