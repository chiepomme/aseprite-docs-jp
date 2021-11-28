# スプライトシート

スプライトシートは、同じスプライトの複数のフレームが載った1枚の大きな画像です。たとえば、このアニメーションを保存するとしましょう。

![Running Guy](sprite-sheet/running-guy.gif)

水平並びのスプライトシートはこのようになります。

![Horizontal Sprite Sheet](sprite-sheet/running-guy-horz.png)

垂直並びのスプライトシートはこのように。

![Vertical Sprite Sheet](sprite-sheet/running-guy-vert.png)

マトリックス型のスプライトシートはこのように。

![Matrix Sprite Sheet](sprite-sheet/running-guy-matrix.png)

以下の項目では、このようなスプライトシートをどうやってエクスポート・インポートするかを説明します。

## インポート

スプライトをインポートするには、メニューの *ファイル > スプライトシートのインポート* を使用します。ダイアログで、ファイルを選択し、`x` `y` のオフセットと、スプライトの `幅` と `高さ` を入力します。

![Import Sprite Sheet 01](sprite-sheet/running-guy-import-01.png)

パディングはスプライト間にすきまがある場合に利用してください。また、タイプは、スプライトの順番に影響を与えます。

![Import Sprite Sheet 02](sprite-sheet/running-guy-import-02.png)

## エクスポート

スプライトシートをエクスポートするには、メニューの *ファイル > スプライトシートのエクスポート* を使用します。ダイアログでは、全てのレイヤーを出力するか、特定のレイヤーを出力するかを選べ、タグを利用してフレームも選択できます。

![Export Sprite Sheet](sprite-sheet/running-guy-export.png)

## コマンドラインインターフェースを使用した自動化

(*作成中*)

## テクスチャアトラス

テクスチャアトラスは、ゲームで使用する全てのグラフィック、スプライト、画像を含んだ巨大な画像のことです。この画像は、ハードウェアアクセラレーションを利用してスクリーンに描画するためビデオメモリに読み込まれます。そのため「テクスチャ」と呼ばれます。
