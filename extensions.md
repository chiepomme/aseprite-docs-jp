# 拡張機能

**[Aseprite v1.2-beta10](https://www.aseprite.org/release-notes/#aseprite-v1-2-beta10)** から、Aseprite に拡張機能を追加・削除できるようになりました。

拡張機能は、`.aseprite-extension` (`.zip`) ファイルになっていて、メニューの *編集 > 環境設定 > 拡張機能* で管理できます。

![Extensions in Preferences](extensions/extensions.png)

## 拡張機能を追加・削除する

メニューの *編集 > 環境設定 > 拡張機能* に、「拡張機能を追加」ボタンがあります。このボタンを利用することで、`.aseprite-extension` または `.zip` ファイルを直接選択することができます。拡張機能のインストール後、このファイルは[環境設定フォルダ](preferences-folder.md)の `extensions` フォルダに解凍されます。

## ファイルの内容

拡張機能やプラグインは完全に `.zip` ファイルと同一のものですが、ファイルの拡張子を `.aseprite-extension` に変更することができます。そうすることで、ユーザーはエクスプローラーや Finder でダブルクリックしてインストールすることができるようになります。

`.zip` ファイルの中身は、どのタイプの拡張機能を作るかによって変わります。しかし、どのタイプであっても、`package.json` は必ず含んでいます。

`.aseprite-extension` ファイルの構造は拡張機能の種類によって変わります。

* [パレット](extensions/palettes.md)
* [言語](extensions/languages.md)
* [テーマ](extensions/themes.md)
* [ディザリング行列](extensions/dithering-matrices.md)
* [スクリプトによるプラグイン](https://github.com/aseprite/api/blob/master/api/plugin.md#plugin)
