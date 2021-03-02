# buildguide

## キット内容

| 名称                   | 個数 | 備考                                  | 
| ---------------------- | ---- | ------------------------------------- |
| トッププレート         | 2個  |                                       |
| メインpcb              | 2個  |                                       |
| ボトムプレート         | 2個  |                                       |
| 追加ボトムプレート     | 2個  |                                       |
| pro micro              | 2個  |                                       |
| pro micro 保護プレート | 2個  |                                       |
| TRRSジャック           | 2個  |                                       |
| タクトスイッチ         | 2個  |                                       |
| ダイオード             | 57個 |                                       |
| kailh mxソケット       | 59個 | +2個は右上追加キーとisoエンター用です |
| oled モジュール        | 2個  |                                       |
| ys-sk6812mini-e        | 57個 |                                       |
| スペーサー m2 8mm      | 24個 |                                       |
| m2 低頭黒ネジ 5mm      | 48個 |                                       |
| ゴムクッション         | 8個  |                                       |

## 手順

1. 内容物を確認します。足りない物があればすぐに連絡をください。

2. レイアウトを決定します。isoエンターを利用する場合は一行目一番右端のキーを使用することができます。
画像の箇所にisoエンターキーをつけることができます。
![iso画像](https://github.com/Diwamoto/ownly/blob/master/img/iso.png)

<blockquote class="twitter-tweet"><p lang="ja" dir="ltr">このキーボードにisoエンターを付けたイメージです。<br>かっこいいものがなかったのでとりあえず家に転がってたものをつけてます。<br>奥にあるのは彼女が作った買ってるハムスターのキーキャップですw可愛い <a href="https://t.co/QXqz3y2MWy">pic.twitter.com/QXqz3y2MWy</a></p>&mdash; Diwamoto (@Diwamoto_) <a href="https://twitter.com/Diwamoto_/status/1312257024906850304?ref_src=twsrc%5Etfw">October 3, 2020</a></blockquote> 


3. (必須ではない)pro microのusb端子はもげやすいので、100均のエポキシ接着材等で固めます。
<a href="https://youtu.be/b-uNS74-5Xw?t=205" target="_brank">こちら</a>
が参考になると思います（というか、Daihukuさんの動画がとてもわかりやすいので、そっち見た方が作りやすいかもしれません。。。。）

4. pcbを折ります。手できれいに折れるので、残った捨て基板をニッパーなどで取り除いてください。切った端はやすり等で削ると綺麗になくなります。またこのタイミングでpcbの側面をマジック等で塗りつぶしておくと基板感がなくなり高級感が出ます（少しだけ）
![pcb折った画像](https://github.com/Diwamoto/ownly/blob/master/img/PCB.JPG)

5. pcbを裏がえしダイオードをはんだ付けします。ダイオードには向きがあるので気を付けてください。
![ダイオード画像](https://github.com/Diwamoto/ownly/blob/master/img/ダイオード.png)

6. スイッチのソケットをはんだ付けします。決定したレイアウトのシルクの位置に合わせてソケットを置き、はんだ付けしてください。
![ソケット画像](https://github.com/Diwamoto/ownly/blob/master/img/ソケット.png)

(LEDを付ける場合はこの段階で取り付けます。取付の方法はオプションを参考にしてください。)

7.trrsジャックとリセットスイッチをはんだ付けします。oled(液晶)を使用する際はピンソケットもハンダ付けしてください。
![TRRS画像](https://github.com/Diwamoto/ownly/blob/master/img/TRRS.png)

8.primicroにコンスルーをはんだ付けします。oledを使用する場合はoledモジュールにもピンヘッダを取り付けます。

![コンスルー](https://github.com/Diwamoto/ownly/blob/master/img/コンスルー.png)


上の画像の部品をこの向きで取り付けてください（向きは同じです。）

![promicro](https://github.com/Diwamoto/ownly/blob/master/img/pro-micro.png)


9.この段階でpromicroにファームウェアを書き込んでキーボードにつけ、trrsケーブルを接続し左右のキーボードの通電を確認します。ピンセット等で取り付けたソケットをショートさせ反応しないキーがないことを確認します。
promicroのファームウェアの書き込みについては[#primicroにファームウェアを書き込む](#primicroにファームウェアを書き込む)を参照してください。


10. 基板に保護プレート用のスペーサーをねじ止めします。

![](https://github.com/Diwamoto/ownly/blob/master/img/保護プレートスペーサー.png)

11. OLEDモジュールを使用する場合は差し込み、保護プレートをねじ止めします。

![](https://github.com/Diwamoto/ownly/blob/master/img/OLED差し込み.png)

![](https://github.com/Diwamoto/ownly/blob/master/img/保護プレート.png)

12.トッププレートにスペーサーをねじ止めします。

![](https://github.com/Diwamoto/ownly/blob/master/img/スペーサー.png)


13.トッププレートの四隅にスイッチをつけ、pcbに合体させます。(スタビライザーを使用する場合は取り付けて置いてください)

![](https://github.com/Diwamoto/ownly/blob/master/img/取り付け.png)

14.残った穴にスイッチを取り付けます。

![](https://github.com/Diwamoto/ownly/blob/master/img/スイッチ取り付け両手.png)

15.ボトムプレートに追加プレート用のスペーサーを取り付けます。追加プレートを使用しないのであれば取り付ける必要はありません。

![](https://github.com/Diwamoto/ownly/blob/master/img/ボトムスペーサー.png)

16.pcbを裏返し、ボトムプレートをねじ止めします。

![](https://github.com/Diwamoto/ownly/blob/master/img/ボトムプレート取り付け.png)


17.キーキャップを取り付けて完成です。qmkからキーマップを自由に書き換えてあなただけのものを作り上げてください！
（ownlyは「自分だけの物」にしたかったのでこういう名前にした経緯があります）

![](https://github.com/Diwamoto/ownly/blob/master/img/完成.png)
## オプション

### ledの取付
このキットのledには「YS-SK6812MINI-E」を使用しています。こちらは従来のものにタブがついているもので手はんだがしやすくなっております。
基板のシルクに合わせてledの足が欠けている部分をはんだ付けしてください。
![led画像](https://github.com/Diwamoto/ownly/blob/master/img/LED.png)

足がついているのではんだ付けはしやすいですが、以前のもののように熱には弱いです。以下の順番ではんだ付けして、一つ一つ確認しながらハンダ付けすることをお勧めします。予備が付属しておりますが、万一足りなくなった場合はこちらで保障することができませんので、秋月電子等でお求め下さい。
![led順番](https://github.com/Diwamoto/ownly/blob/master/img/LED順番.jpg)

https://akizukidenshi.com/catalog/g/gI-15478/

### primicroにファームウェアを書き込む
キーボードのファームウェアには[qmk](https://github.com/qmk/qmk_firmware)を使用しています。
qmkのインストールにはQMK_MSYSをお勧めします。詳しくは[こちら](https://zenn.dev/diwamoto/articles/1943345edce519)をご覧ください。

**プログラムわからない！やりたくない！！**
安心して下さい。このレポジトリのhexフォルダにあるファイルを[qmk_toolbox](https://github.com/qmk/qmk_toolbox/releases)で
書き込むことでプログラムレスでキーボードを使うことができます。
また、[Remap](https://remap-keys.app/)に対応しているので、こちらからプログラムレスでキーマップを変更することができます。

### rgb_matrixを有効にする
rgb_matrixは今現在まだ分割キーボードをサポートしていませんが、TRRSケーブル経由でLEDを物理的につなぐことで分割キーボードでもrgb_matrixのアニメーションを体験することができます。
まずは`diwamoto`キーマップを有効にします。
```
make ownly:diwamoto:flash

```
コマンドで有効にしてください。
その後、一度USBケーブルとTRRSケーブルを外します。
そして左手のボトムプレートのネジを一度外し、裏返した状態の一番右下の
LEDとTRRSジャックの一つだけ離れているピンを銅線などでジャンパします。
（画像は旧型の物になりますのでねじ穴等の場所は違いますが部品は変わりません。）
![matrix](https://github.com/Diwamoto/ownly/blob/master/img/matrix左.png)

次に、右手のボトムプレートを外します。そして、先ほどジャンパさせた手順と同じように
TRRSジャックの一つだけ離れているピンから一番左下のLEDの右下の足に接続します
（画像はPro MicroのLEDピンに接続しています。LEDピンと先ほど説明した足はつながっていますのでこれでも問題ないのですが、コンスルーを使用し取り外しできるようにしている関係上おすすめできません。）
![matrix](https://github.com/Diwamoto/ownly/blob/master/img/matrix右.png)


ここまできたら基板を元に戻し、動作確認してみましょう。
うまく行けば、両方の手でRGB_MATRIXのアニメーションが流れているハズです。
アニメーションを変更するのはLower/Raiseキーを押しながらGキーを押すと変更できます。

**上の画像は旧版になります。新版については以下の画像を参考にしてください。**

![matrix](https://github.com/Diwamoto/ownly/blob/master/img/LED_matrix対応.jpg)



### oled表示をいじる

oledの操作には

<a href="https://helixfonteditor.netlify.app/" target="_brank">webフォントエディタ</a>
を推奨します。サイトに行き、ファームウェアの中の`lib/glcdfont_ownly.c`を選択してください。

こういう画面になりますので左下の部分を自由にいじる事でled表示を変える事ができます。
![](https://github.com/Diwamoto/ownly/blob/master/img/oledfont.png)
