# 自動結合レイヤー (Continuous Layer)

自動結合アイコン![Broken layer icon](continuous-layers/broken-layer.png)は、セルがコピーされたときにどのタイプの[セル](cel.md)としてコピーするかを決定します。これは、[新規フレームを追加](new-frame.md)、[フレームをコピー](copy-frames.md)、[セルをコピー](copy-cels.md)といったコマンドの動作に影響を与えます。

2つのモードがあります:

1. ![Normal layer icon](continuous-layers/broken-layer.png) このレイヤーは（非結合セルを使用した）通常のレイヤーです：新しいセルは独立した状態で（コピーとして）作成されます。
1. ![Continuous layer icon](continuous-layers/continuous-layer.png) このレイヤーは自動結合です：セルは[結合セル](linked-cels.md)として作成されます。

一般的には、静止したコンテンツを持つ[背景レイヤー](layers.md#background-layer)では自動結合セルを利用し、それぞれのフレームで異なるセルとなるレイヤーは自動結合ではないモードを利用します：

![Continuous vs normal layer](continuous-layers/cont-vs-dis.png)

このオプションは作業の内容によって切り替えることになるでしょう。オプションを切り替えても現在のセルには影響を与えず、その後に行う操作にのみ影響を与えます。

---

**SEE ALSO**

[結合セル](linked-cels.md) |
[レイヤー](layers.md) |
[新規フレーム](new-frame.md) |
[フレームをコピー](copy-frames.md) |
[タイムライン](timeline.md)
