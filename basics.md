# Aseprite の基本

ここでは Aseprite の裏にある基本的な原理を説明します。

Aseprite では、1つの[スプライト](sprite.md)は、時間軸に沿ったフレームと、上下に重なり合ったレイヤーで構成されています。
フレームとレイヤーが組み合わさると、[スプライトエディタ](sprite-editor.md)で[編集](drawing.md)可能なグラフィックである[セル](cel.md)が作られます。レイヤー、フレーム、セルは[タイムライン](timeline.md)上で見ることができます：

![Timeline Overview](sprite/sprite-components.png)

## スプライトの基本的な構成要素

フレームはスプライト内の1枚の動かない画像のことです。
フレームを追加しながら書き換えていくと、[アニメーション](animation.md)という、時系列に沿った画像の集まりになります。

Aseprite がどのようにフレームの集まりを再生するかということについては、[アニメーションの項目](animation.md)で詳細に説明しています。フレームの流れはタイムライン上では左から右の横方向に表現されます。

それぞれのフレーム画像は1枚以上の[レイヤー](layers.md)から成り立ちます。レイヤーはタイムラインの下から順番に表示されます。タイムラインで一番下のレイヤーが最初に描画され、そこから順番に重ねられていきます。レイヤーは複雑な1枚の絵を、構成要素ごとに分割して扱いやすくしてくれます。

横方向のフレームと縦方向のレイヤーの交わった部分を[セル](cel.md)と言います。セルの内容を動かしたり、編集したり、削除したりしても、ほかのセルに影響を与えません。そのため、ほかの部分を変更しないように要素を独立させて編集するのに向いています。

## ワークフロー

基本的な[ワークフロー](workflow.md)は以下の通りです:

* [新しいスプライトを作成する](new-sprite.md)：メニューの *ファイル > 新規* から作成します。
* [描く](drawing.md)：ペンツール![Pencil Tool Icon](tools/pencil-tool.png)を使って <kbd>左クリック</kbd> <kbd>右クリック</kbd> で描きます。[カラーバー](color-bar.md)で同じマウスのボタンを使って色を選択します。
* [保存する](save.md)：メニューの *ファイル > 上書き保存* を使用して、`.ase` ファイルとして保存することで、全ての画像情報（レイヤー、フレームなど）を保持できます。また、一部の[ワークスペース](workspace.md)の設定も保存されます。
* [スプライトをエクスポートする](exporting.md)：`.gif` ファイルとしてウェブページ向けにエクスポートしたり、フレームごとの `.png` ファイルとしてエクスポートしたり、すべてのフレームが1列に並んだ1つの `.png` ファイルとしてエクスポートしたり、[スプライトシート](sprite-sheet.md)としてエクスポートしたりできます。

_名前を付けて保存_ や _エクスポート_ をする時に、ほかのファイル形式を選ぶこともできます。このあたりは色深度の選択や好みに因るところです。

もっと画面の構成要素を知るためには[ワークスペース](workspace.md)を見てください。
より詳細なワークフローについては[ワークフロー](workflow.md)を見てください。

## キーボードに置いた手で

左手（左利きであれば右手）をキーボードに置くのをおすすめします。
最初から便利なキーボードショートカットを使うことで、Aseprite をうまく使うことができるでしょう。

* テンキーではない <kbd>1</kbd> <kbd>2</kbd> <kbd>3</kbd> <kbd>4</kbd> <kbd>5</kbd> <kbd>6</kbd> キーで[ズーム](zoom.md)できます。（マウスホイールでもズームが可能です。）
* <kbd>B</kbd> キーはペンツール、<kbd>M</kbd> キーは矩形選択で、これらは一番良く使うツールです。
* <kbd>Alt+クリック</kbd> ではスポイトツール![Eyedropper Tool Icon](tools/eyedropper-tool.png)で色を取得出来ます：
  <kbd>Alt+左クリック</kbd>では前景色を、<kbd>Alt+右クリック</kbd>では背景色を取得出来ます。
* The <kbd>Ctrl</kbd> key (or <kbd>⌘</kbd> on macOS) can be used to
  select the [Move tool](move-tool.md) ![Move Tool Icon](tools/move-tool.png).
  With it you can easily select or move layers.
* The <kbd>Tab</kbd> key hides and reveals the
  [timeline](timeline.md). If your timeline is ever missing, this is
  the fastest way to reveal it!

* Holding <kbd>Spacebar</kbd> as you <kbd>Left click+Drag</kbd> will
  pan your view of the sprite you are currently editing. Useful when
  you're working on large graphics or are zoomed-in.

## 右クリックを別の機能に割り当てる

デフォルトでは、<kbd>右クリック</kbd>は[背景色](color-bar.md#背景色)で描く機能が割り当たっています。
この設定はメニューの [*編集 > 環境設定 > エディター*](right-click.md) から変更できます。

---

**SEE ALSO**

[ワークスペース](workspace.md) |
[ワークフロー](workflow.md) |
[スプライト](sprite.md)
