# 透明色

スプライトが [RGB カラー](color-mode.md#rgb)または[グレースケール](color-mode.md#grayscale)の場合、透明なピクセルは `アルファ=0` になっています。一方で、[インデックスカラー](color-mode.md#indexed)の場合には、[透過レイヤー](layers.md#transparent-layers)での透明を表す色は、パレット内の特別なインデックスを持った色になります。

![Transparent Color](transparent-color/transparent-color-property.png)

この特別なインデックスを持ったピクセルは、透過レイヤーでは透明になり見えません。
（背景レイヤーでは、この「透明と定義された色」を通常の色として表示することができます。）
 
この透明色は、[カラーバー](color-bar.md)でマウスのホイールクリックをするか、メニューの [*スプライト > プロパティ*](sprite-properties.md)で変更が出来ます。

---

**SEE ALSO**

[色](color.md) |
[カラーモード](color-mode.md) |
[スプライトのプロパティ](sprite-properties.md)
