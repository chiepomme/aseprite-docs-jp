# スプライトエディタ

スプライトエディタは[新規スプライト](new-sprite.md)を作成して最初に見るエディタです。

![Sprite Editor](sprite-editor/sprite-editor.png)

スプライトエディタでは以下のことをできます。

1. [描く](drawing.md)：マウスクリックやスタイラスやペン、Windows Surface でのタッチなどで描くことができます。
1. [ズーム](zoom.md)：マウスホイールや、MacBook のトラックパッドや、Windows Surface でのピンチのようなジェスチャでズームをすることができます。
1. マウスホイールのドラッグや、MacBook のトラックパッド、Windows Surface での2本指でのスワイプで、表示位置をスクロールできます。<kbd>Shift</kbd>キーを押しながらマウスホイールを回すと横方向にだけスクロールします。

### 設定

スプライトエディタについては、メニューの *編集 > 環境設定 > エディター* で多くのカスタマイズが可能です。

![Sprite Editor Preferences](sprite-editor/editor-preferences.png)

* *マウスホイールでズーム*：デフォルトでチェックされています。マウスホイールでズームするようになります。（チェックしない場合、縦方向へのスクロールになります。）
* *2本の指を上下にスライドさせるズーム*：これは macOS でのみ有効です。有効にすると、MacBook のトラックパッドで2本指でズームできるようになります。
* *マウスホイールで中心からズーム*：マウスホイールでズームするときに、マウスの位置ではなく常にスプライトエディタの中央を基準に[ズーム](zoom.md)するようになります。
* *キーで中心からズーム*：<kbd>1</kbd> <kbd>2</kbd> <kbd>3</kbd> などのキーを使ってズームするときに、マウスの位置ではなく常にスプライトエディタの中央を基準に[ズーム](zoom.md)するようになります。
* *スプライトエディタにスクロールバーを表示する*: Uncheck to hide the scroll bars.
* *描画時に自動スクロール*: With this option checked, when you
  are [drawing](drawing.md) (have the mouse button pressed) the mouse
  touches the edges of the sprite editor, it will scrolls
  automatically.
* *ペンツールで直線のプレビュー*: When you use the
  Pencil tool, pressing the <kbd>Shift</kbd> key will draw a straight line from
  the last painted point. With this option checked, you will see the
  line preview immediately after pressing the <kbd>Shift</kbd> key (instead of
  waiting for the mouse button). If this is too annoying for you, you
  can uncheck the option.
* *スポイト使用時にカスタムブラシを破棄する*: If you create a
  custom brush with *Edit > New Brush* option, using the eyedropper
  ![Eyedropper tool icon](tools/eyedropper-tool.png)
  tool will change the color of your brush. Checking this option,
  after picking a color with the eyedropper, the custom brush will be
  completely discarded and a a regular brush with the picked color
  will be selected.
* *右クリックの操作*: you can customize what action to do with the
  [right-click](right-click.md).

---

**SEE ALSO**

[スプライト](sprite.md) |
[タイムライン](timeline.md) |
[ワークスペース](workspace.md) |
[基本](basics.md)
