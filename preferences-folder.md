# 環境設定フォルダ

Aseprite の設定は個人設定フォルダのいくつかのファイルに分けて保存されています。

![Files in Preferences Folder](preferences/preffiles.png)

環境設定フォルダの場所は *編集 > 環境設定 > 一般 > 設定ファイルの場所* を使用することで開くことができます。

いずれにせよ、プラットフォームに応じた異なる方法で自分でフォルダにたどり着くことができます。

## Windows

環境設定フォルダを開くには、まず<kbd>Windowsキー + R</kbd>キー（または、`スタートメニュー > ファイル名を指定して実行...`)を押します。これによって、プログラムを実行するためのダイアログが開きます。そこに以下のように入力してください。

    %AppData%\Aseprite

入力したら `Enter` キーを押します。

（訳注：Windows 10 では上記の項目はメニュー内に無いため、スタートメニューを開いたらそのまま上の内容を入力するか、スタートボタンを右クリックするか、エクスプローラーのアドレスバーでも同じことができます。）

## macOS

Spotlight 検索を開き（<kbd>⌘Space</kbd>）以下のパスをコピーして `~/Library/Application Support/Aseprite` <kbd>⌘V</kbd> で貼り付け、<kbd>Enter</kbd> を押します。

   ![Spotlight Search](preferences/spotlight.png)

## Linux

ターミナルを開き、以下のコマンドをコピーして<kbd>Enter</kbd>キーを押してください。

    xdg-open ~/.config/aseprite

## 特別な設定

Aseprite v1.2.16.3 からは、テスト用機能ですが、環境設定フォルダの場所を変更できます。 `ASEPRITE_USER_FOLDER` という[環境変数](https://ja.wikipedia.org/wiki/%E7%92%B0%E5%A2%83%E5%A4%89%E6%95%B0)を他のフォルダに設定してください。

---

**SEE ALSO**

[環境設定をリセット](reset-preferences.md)
