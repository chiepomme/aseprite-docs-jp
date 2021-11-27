# スポイト

スポイトツール![Eyedropper Tool Icon](tools/eyedropper-tool.png)は、編集している画像の中から色を取得することができます。ツールバーの消しゴムアイコンの上にマウスカーソルを持って行くとボタンが表示されます：

![Eraser and Eyedropper group](eyedropper/eyedropper-group.png)

`I`キーを押すか、`Alt+クリック`でも使用することができます。

スポイトツールでは、`左クリック`すると[前景色](color-bar.md#foreground-color)として色を取得することができ、`右クリック`すると、[背景色](color-bar.md#background-color)として取得できます。

ほかのオプションは[コンテキストバー](context-bar.md)に表示されます：

* RGB の値ではなく、HSV または HSL の値を取得するオプション：

  ![Pick options](eyedropper/pick-options.png)

* *All Layers* では統合された全レイヤーから色を取得します。
  *Current Layer* では、（レイヤーのブレンドモードの影響を受けずに）現在のレイヤーから取得します。
  *First Reference Layer* では、最初に見つかった参照レイヤーから色を取得します：

  ![Sample options](eyedropper/sample-options.png)

## 右クリックで色を取得する

`右クリック`を色を取得するように変更するのは、[編集 > 環境設定 > エディター](right-click.md)からできます。

---

**SEE ALSO**

[カラーバー](color-bar.md) |
[右クリック](right-click.md)
