# トラブルシューティング

Aseprite を起動するのに問題がある場合（たとえば、起動するがすぐに落ちてしまう場合）以下の手順を試してください。

1. [環境設定をリセットする](reset-preferences.md)
1. [デバッグオプション](debug.md)を使用すると、`Aseprite-v1.2-DebugOutput.txt` というファイルが生成されます。
1. Windows のみ：`Aseprite-v1.2-DebugOutput.txt` ファイルの最後の行が、`PEN: Wintab library loaded` になっていないか確認してください。この場合、[Wintab を無効](wintab.md)にしてみてください。
1. それでも解決しない場合は、[support@aseprite.org](mailto:support@aseprite.org) まで、`Aseprite-v1.2-DebugOutput.txt` ファイルを送ってください。

または、同じ問題を以下の場所で探してみてください。

* [Aseprite Community](https://community.aseprite.org)
* [Steam General Discussion forum](http://steamcommunity.com/app/431730/discussions/0/)
* [Steam Bug Reports forum](http://steamcommunity.com/app/431730/discussions/2/)
* [Closed bugs on the GitHub](https://github.com/aseprite/aseprite/issues?utf8=%E2%9C%93&q=is%3Aissue%20is%3Aclosed%20%20label%3Abug)

## クラッシュ・データ紛失

クラッシュした場合は、[スプライトを復元](data-recovery.md)できる可能性があります。

## タブレットの問題

タブレットが動かない場合、[タブレット](tablet.md) ページを見てください。

## macOS の描画の問題

Aseprite は macOS の非同期レンダリング([CALayer's drawsAsynchronously](https://developer.apple.com/documentation/quartzcore/calayer/1410974-drawsasynchronously?language=objc))を使用しています。 Aseprite v1.2.20 からは、この機能を無効にすることができます。例えば、黒い長方形が画面に表示されるなどの問題が出た場合にお試しください。（いずれにせよ、Display P3 などの[カラープロファイル](color-profile.md)を使用する場合は、パフォーマンスが大きく落ちます。）

これを無効化するには以下の手順を行ってください。

1. Aseprite を閉じる
2. [環境設定フォルダ](preferences-folder.md)の `aseprite.ini` ファイルを開きます。
3. `[general]` と言う項目を検索して、`osx_async_view = false` というオプションを追加します。
```
[general]
osx_async_view = false
```
4. ファイルを保存して Aseprite を再度起動してください。

---

**SEE ALSO**

[環境設定をリセット](reset-preferences.md) |
[データ復元](data-recovery.md) |
[デバッグ](debug.md) |
[タブレット](tablet.md)
