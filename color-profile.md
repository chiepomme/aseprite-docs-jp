# カラープロファイル

画面の中のピクセルは、特定の RGB の値を持った小さな四角にみえます。RGB のそれぞれの値は 0.0 から 1.0 の値（整数なら 0 から 255）として扱われることが多いでしょう。
この RGB の値を3次元的な座標として捉えると、それぞれの値を赤・緑・青の軸上での位置だと考えることができます。

![RGB Cube](color-profile/rgb-cube.png)

この立方体での位置について考えてみましょう。私たちは、*RGB=(0, 0, 0)* が黒を、*RGB=(255, 0, 0)* が赤を、*RGB=(255, 255, 255)* が白を表すといったことは分かっています。

ところで、[白色](https://ja.wikipedia.org/wiki/%E7%99%BD%E8%89%B2%E7%82%B9)というのは厳密にはなんなのでしょうか。あなたが使っているモニターが製造過程でキャリブレーションされて、メーカーが「よし、これは白色だ」と言ったして、その環境の照明はどうなっていたのでしょうか。

色を扱うデバイス（モニター、プリンター、カメラ、スキャナーなど）は、キャリブレーションを必要とします。
それは、環境の中の光をなんらかの RGB の値に変換する、または逆に、先ほどの立方体のなんらかの RGB の値を[光波](https://ja.wikipedia.org/wiki/%E5%85%89)に変換するためです。

カラープロファイルは、RGB の値がどの[色空間](https://ja.wikipedia.org/wiki/%E8%89%B2%E7%A9%BA%E9%96%93)のものであるかを定義します。それは純粋な赤・青・緑・白というのがなんであるかというのを定義することです。これによって、あるデバイス（たとえば、あなたが画像を編集するモニター）での特定の RGB の値の見え方をほかのデバイス（たとえば、あなたの作品を見る人のモニタ）での見え方とマッチさせることができます。

インターネット上の画像は通常は [sRGB 色空間](https://en.wikipedia.org/wiki/SRGB)を使用していますが、
[PNG ファイル](https://ja.wikipedia.org/wiki/Portable_Network_Graphics)や [JPEG ファイル](https://ja.wikipedia.org/wiki/JPEG)には、[ICC カラープロファイル](https://ja.wikipedia.org/wiki/ICC%E3%83%97%E3%83%AD%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB) を含めることができます。カラープロファイルには [RGB の色域](https://ja.wikipedia.org/wiki/%E8%89%B2%E5%9F%9F)と、[ガンマ補正](https://ja.wikipedia.org/wiki/%E3%82%AC%E3%83%B3%E3%83%9E%E8%A3%9C%E6%AD%A3)が含まれています。

Aseprite v1.2.10-beta2 からは、[カラープロファイルを `.aseprite` ファイルにも埋め込めるようになりました](https://github.com/aseprite/aseprite/blob/master/docs/ase-file-specs.md#color-profile-chunk-0x2007)。

カラープロファイルは、[スプライトのプロパティ](sprite-properties.md)から割り当てもしくは変換できます。
Aseprite がどのように色を扱うかは *編集 > 環境設定 > カラー* から設定ができます。

![Color Management Preferences](color-profile/color-management-preferences.png)

---

**SEE ALSO**

[色](color.md) |
[スプライトのプロパティ](sprite-properties.md)
