# Wintab

Wintab (`WinTab32.dll`) は、ワコムが作成したタブレット系デバイスと Windows で通信を行うための古い API です。 Windows 8 以前は、ワコム製・他社製問わずタブレットからの筆圧情報にアクセスするためのデファクトスタンダードでした。 Windows 8 からは、マイクロソフトが新しい公式 API ポインター API と Windows Ink を提供し始めました。

ときどき、この DLL を読み込む時にプログラムが固まってしまったり、読み込めても正しく動かないことがあります。ドライバーをインストールしたり、Windows を再起動することで解決することもあります。もしこれらを試しても治らない場合は、[タブレット設定](tablet.md)でポインター API を試し、それでも治らない場合「wintab32ライブラリのロード」を無効にしてください。*編集 > 環境設定 > タブレット* （または古いバージョンであれば *編集 > 環境設定 > 実験的機能* ）から無効にできます。

![Don't load the WinTab driver](wintab/disable-wintab.png)

## Aseprite が起動しない

プログラムが起動さえしない場合、`-disable-wintab` オプションを付けて起動を試すことができます。（Aseprite v1.2 以降）

    "C:\Program Files\Aseprite\Aseprite.exe" -disable-wintab

これは、`WinTab32.dll` のロードを無効にします。タブレットは正しく動かないかもしれませんが、少なくともマウスやトラックパッドで使うことができます。（繰り返しになりますが、[Windows ポインタ API](tablet.md)も試してみてください。）

## Steam

Steam 版の場合、Aseprite の起動オプションで `-disable-wintab` オプションを指定できます。

1. Steam ライブラリの Aseprite を右クリックし、プロパティを開きます。

   ![Open Aseprite Properties](steam/steam-1-open-properties.png)

2. 起動オプションボタンがあればクリックします。（訳注：最新版ではそのまま入力できるようになっています）

   ![Open launch options](steam/steam-2-launch-options.png)

3. `-disable-wintab` オプションを記入し「OK」を押します。

   ![Add disable wintab option](steam/steam-3-disable-wintab.png)

---

**SEE ALSO**

[タブレット](tablet.md) |
[トラブルシューティング](troubleshooting.md)
