# 選択

選択ツール![Marquee Tool Icon](tools/marquee-tool.png)（<kbd>M</kbd>キー）を使うとスプライトの一部分を選択できます。
選択した物は、[移動](move-selection.md)したり、[変形](transformations.md)したり、[拡大縮小](resize.md)したり、[回転](rotate.md)したりできます。

スプライトの一部を選択すると、英語で[アリの行進](https://en.wikipedia.org/wiki/Marching_ants)と呼ばれる、動く点線が見られます。

![Marching ants](selecting/marching-ants.gif)

選択範囲を作成すると、同時に現在アクティブな[セル](cel.md)が選択されます。そのため、全ての変形はこのセルにのみ影響を与えます。

## 選択範囲の追加・削除・共通範囲

[コンテキストバー](context-bar.md)には、選択領域に対しての操作を変更するボタンがあります。![Modifiers](selecting/modifiers.png)

デフォルトでは、左のマウスボタンをドラッグして離すと、既存の選択範囲を置き換えます。
この挙動はオプションによって切り替えられます。（それぞれキーボードショートカットが割り当てられています。）

* ![選択範囲を置き換える](selecting/replace-selection.png)：デフォルトの操作です。既存の選択範囲全体を新しいもので置き換えます。（左ドラッグ)
* ![選択範囲に追加する](selecting/add-selection.png)： 既存の選択範囲に新しい選択範囲を追加します。(<kbd>Shift</kbd>を押しながら左ドラッグ)
* ![選択範囲から削除する](selecting/subtract-selection.png)：既存の選択範囲から新しい選択範囲の領域を削除します。（<kbd>Alt+Shift</kbd>を押しながら左ドラッグ、もしくは右ドラッグ）
* ![選択範囲との共通部分を選択する](selecting/intersect-selection.png)：既存の選択範囲と新しい選択範囲の重なった部分を選択します。（<kbd>Ctrl+Shift</kbd>を押しながら左ドラッグ）

## 内容を選択する

メニューの *選択 > 全てを選択* （<kbd>Ctrl+A</kbd> または <kbd>⌘A</kbd>）を使用すると、スプライトのキャンバス全体を選択できます。
また、メニューの *編集 > 変形* （<kbd>Ctrl+T</kbd> または <kbd>⌘T</kbd>）を使用すると、アクティブな[セル](cel.md)の内容（非透明ピクセル）だけを選択できます。

## 選択範囲の解除と再選択

メニューの *選択 > 選択範囲の解除* （<kbd>Ctrl+D</kbd> または <kbd>⌘D</kbd>）を使用すると、現在の選択範囲を非表示にすることができます。
また、メニューの *選択 > 再選択* （<kbd>Ctrl+Shift+D</kbd> または <kbd>⇧⌘D</kbd>）で再表示することができます。

## 選択範囲の反転

メニューの *選択 > 選択範囲の反転* （<kbd>Ctrl+Shift+I</kbd> または <kbd>⇧⌘I</kbd>）を使用して、選択範囲を反転できます。

---

**SEE ALSO**

[変形](transformations.md) |
[選択範囲を移動](move-selection.md)
