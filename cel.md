# セル(Cel)

セル（[セルロイド](http://en.wikipedia.org/wiki/Cel)に由来します）は、特定のフレームとレイヤーにある画像で、キャンバスの中の特定の*xy座標*に存在します。
is one image in a specific frame and layer, at a specific *xy*-coordinate in the canvas.

![Cel on Timeline](cel/cel-on-timeline.png)

フレームとセルの違いは、フレームは特定の時間において全レイヤーのセルを合わせたものだということです：

![Frame on Timeline](cel/frame-on-timeline.png)

## セルを移動する

[移動ツール](move-tool.md)で現在のセルをキャンバス内でドラッグできます。
また、ほかのレイヤーまたはフレームに[タイムラインを使ってセルを移動する](move-cels.md)ことができます。

## 不透明度を変更する

[RGB](color-mode.md#rgb)画像ではそれぞれのセルで不透明度を持つことができます。
ステータスバーにあるスライダーを使うことで不透明度を変更できます：

![Cel Opacity](cel/cel-opacity.gif)

セルを右クリックし`プロパティ`（もしくはメニューの *フレーム > セルプロパティ* ）をクリックすることでも変更が可能です:

![Cel Properties](cel/cel-properties.gif)

----

**SEE ALSO**

[リンクしたセル](linked-cels.md) |
[タイムライン](timeline.md)
