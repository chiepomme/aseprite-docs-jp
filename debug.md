# デバッグ

Aseprite を実行していて問題を見つけた場合は、コマンドラインから `-debug` オプションを付けて実行してください。

Aseprite が起動した後、`Aseprite-v1.2-DebugOutput.txt`（もしくは似たような名前）のファイルがデスクトップに作られます。このファイルを[support@aseprite.org](mailto:support@aseprite.org)に送ってもらえれば、問題の解決に役立ちます。


`-debug` オプションは以下のように付けます。

- [Windows](#windows)
- [macOS](#macos)
- [Steam](#steam)

<hr>

## Windows

1. Windows キーをおしてスタートメニューを開いたら、そのまま `Aseprite` と入力します。それから、アクションリストが閉じていれば開きます。

   ![Aseprite on Start menu](debug/win-1-start-menu.png)

2. アクションリストの「ファイルの場所を開く」を選びます。

   ![Expand options](debug/win-2-actions.png)

3. Aseprite のショートカットを右クリックして、プロパティを開きます。

   ![Right click properties](debug/win-3-right-click-properties.png)

4. 「リンク先」のボックスの最後にスペースを空けて `-debug` オプションを記入して「OK」を押します。

   ![Debug on properties](debug/win-4-debug-option.png)

<hr>

## macOS

1. まず、Aseprite を閉じる必要があります。それから ⌘スペース を押すか、メニューバーの虫眼鏡のアイコンをクリックして Spotlight 検索を開いてください。

   ![Open Spotlight](debug/macos-1-open-spotlight.png)

2. Spotlight 検索に `Terminal` と入力して Enter を押してターミナルを起動してください。

   ![Terminal on Spotlight](debug/macos-2-open-terminal.png)

4. ターミナルに以下のコマンドを入力して Enter を押してください。

       open -a Aseprite --args -debug

<hr>

## Steam

Steam の場合には、Aseprite の起動オプションに `-debug` を付けられます。

1. Steam ライブラリの Aseprite を右クリック（macOS の場合 Ctrl+クリック）し、プロパティを開きます。

   ![Open Aseprite Properties](steam/steam-1-open-properties.png)

2. 起動オプションボタンがあればクリックします。（訳注：最新版ではそのまま入力できるようになっています）

   ![Open launch options](steam/steam-2-launch-options.png)

3. `-debug` オプションを記入し「OK」を押します。

   ![Add debug option](steam/steam-3-debug-option.png)

---

**SEE ALSO**

[トラブルシューティング](troubleshooting.md)
