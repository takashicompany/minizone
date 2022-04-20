# miniZone

<img src = "https://github.com/takashicompany/minizone/blob/master/images/qmk.jpg?raw=true" width="600px" />

miniZoneはiPad miniのようなタブレット端末と一緒に持ち歩くことをコンセプトにしたコンパクトなキーボードです。  
横幅はiPad miniと同じですので、一緒にケースに入れることが可能です。  
小さいながらも高い実用性を目指しました。  
もちろん、iPad miniだけでなく他のタブレット端末やPCで使っても便利です。  
従来のキーキャップの80%のサイズ(0.8u = 16mm)ですが、少ない指の動きで文字を打つことが可能です。  

また、LEDによるアンダーグロウやOLEDといった機能も実装しております。  
[BLE Micro Pro](https://shop.yushakobo.jp/products/ble-micro-pro?variant=37665571340449)を使えばBluetoothで接続することも可能です。  
オプションパーツを揃えることでCR1632電池を基盤に取り付けることも可能です。  
さらにトラックボールを搭載して、キーボードのから手を離さずにすべてを操作を行うことができます。  
(トラックボールを利用する際のソースコードは[こちら](https://github.com/takashicompany/qmk_firmware/tree/minizone/trackball/keyboards/takashicompany/minizone/keymaps/trackball))。

---

miniZone is a compact keyboard designed to be carried with a tablet device like iPad mini.  
Its width is the same as that of the iPad mini, so it can be placed in a case together.  
We aimed for high practicality in spite of its small size.  
Of course, it is useful not only for iPad mini but also for other tablet devices and PCs.  
It is 80% the size of a conventional keycap (0.8u = 16mm), but allows you to type with fewer finger movements.  

Also, functions such as LED underglow and OLED are implemented.  
With [BLE Micro Pro](https://shop.yushakobo.jp/products/ble-micro-pro?variant=37665571340449), it is also possible to connect via Bluetooth.
CR1632 battery can be attached to the base by using optional parts.  
In addition, a trackball is included, allowing you to perform all operations without taking your hands off the keyboard.  
(Source code for using the trackball is [here](https://github.com/takashicompany/qmk_firmware/tree/minizone/trackball/keyboards/takashicompany/minizone/keymaps/trackball)).  

## トラックボールでの動作
https://user-images.githubusercontent.com/4215759/162611440-2bb0ec75-2dbf-48b8-8c0d-54c8666c1aff.mp4

- トラックボールを指定の秒数(デフォルトでは10ミリ秒)動かし続けると、マウス入力レイヤーが有効になる。
- マウス入力レイヤーが有効の時にYキーを押すと左クリックになる
- マウス入力レイヤーが有効の時にIキーを押すと右クリックになる
- マウス入力レイヤーが有効の時にUキーを押した状態でトラックボールを操作するとスクロールとして入力される
- マウス入力レイヤー状態で指定の秒数(デフォルトでは1秒)の間上述のキーを入力をしない、または上述のキー以外を押下すると、マウス入力レイヤーが解除される

ソースコードは[こちら](https://github.com/takashicompany/qmk_firmware/tree/minizone/trackball/keyboards/takashicompany/minizone/keymaps/trackball/keymap.c)。

## 部品

### キットに含まれているもの
|部品|個数|備考|
|:--|:--|:--|
|PCB|1||
|スイッチプレート|1||
|側面プレート|1||
|ボトムプレート|1||
|Pro Microプレート|1||
|OLED Pro Microプレート|1||
|トラックボール Pro Microプレート|1||
|[ダイオード(表面実装型)](https://shop.yushakobo.jp/collections/all-keyboard-parts/products/a0800di-02-100)|38||
|[タクトスイッチ](https://akizukidenshi.com/catalog/g/gP-08081/)|1||
|ゴム足シール|8||
|M2ネジ 8mm|12||
|M2ネジ 5mm|10||
|M2スペーサー 7mm|6||
|M2ナット|10||


### ご自身で用意頂くもの
|部品|個数|備考|
|:--|:--|:--|
|[Kailh Choc v1キースイッチ](https://shop.yushakobo.jp/collections/all-switches/products/pg1350)|38||
|0.8uキーキャップ(16mm)|38|詳細は後述|
|Pro Micro|1|BLE Micro Proにも対応済み|

#### キーキャップ
キーキャップは0.8uサイズ(16mm)をご利用ください。

[こちらの記事](https://e3w2q.github.io/10/)を参考にするとより良いかと思います。

以下は動作確認済みのキーキャップです。

[Choc 向け 挟ピッチ16mm 薄型キーキャップ（50個）  
<img src = "https://img.make.dmm.com/images/item/1273303/main_angled_R_20210609122258214_l.jpg" width="400px" />](https://make.dmm.com/item/1273303/)

[YKNキーキャップセット(Chocスイッチ 16x16mmキーピッチ用) v1.2  
<img src = "https://img.make.dmm.com/images/item/1280053/16x16choc2_20210221120518672_l.jpg" width="400px" />](https://make.dmm.com/item/1280053/)


### お好みで
|部品|個数|備考|
|:--|:--|:--|
|BLE Micro Pro|1|トラックボールの動作は確認済み。OLEDは未確認。|
|コンスルー|2|BLE Micro Proを使う場合は13ピンのものを使用することもできます。|
|[LED(SK6812MINI-E)](https://shop.yushakobo.jp/products/sk6812mini-e-10)|1|キーボードの表面をライティングします。|
|[LED(WS2812B](https://shop.yushakobo.jp/products/a0800ws-01-10)|10|アンダーグロウです。|

### OLEDを搭載する場合
|部品|個数|備考|
|:--|:--|:--|
|[OLEDモジュール](https://shop.yushakobo.jp/collections/all-keyboard-parts/products/oled)|1||
|[OLED用ピンソケット](https://shop.yushakobo.jp/products/a1600ps-01-1)|1|ピンヘッダがあれば取り付け自体は可能だが付け替えができなくなるので使用を推奨。|

### トラックボールモジュールを搭載する場合
|部品|個数|備考|
|:--|:--|:--|
|[7mmオプティカルトラックボールモジュール１uタイプ](https://shop.yushakobo.jp/products/adtb7m)|1||
|[トラックボールモジュール用レベル変換基板](https://shop.yushakobo.jp/products/a0800tl-01-1/)|1||
|[OLED用ピンソケット](https://shop.yushakobo.jp/products/a1600ps-01-1)|1|ピンヘッダがあれば取り付け自体は可能だが付け替えができなくなるので使用を推奨。|

### BLE Micro Pro用に電源を搭載する場合
|部品|個数|備考|
|:--|:--|:--|
|[HU1632](https://www.monotaro.com/p/8835/2765/)|1||
|[チップ積層セラミックコンデンサー](https://akizukidenshi.com/catalog/g/gP-02151/)|1||
|[電源スイッチ(MK12C02)](https://ja.aliexpress.com/item/32798526843.html)|1||
|ボタン電池(CR1632)|1||

### Pimoroni Trackballモジュール(PIM447)を搭載する場合

Rev5以降で搭載が可能です。

|部品|個数|備考|
|:--|:--|:--|
|[PIM447](https://www.marutsu.co.jp/pc/i/32844496/)|1||
|[5ピンソケット](https://www.hirosugi-net.co.jp/shop/g/g24082/)|1||

## 組み立て方

### 1. PCBの表と裏を確認する

表  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9827.jpg?raw=true" width="600px" />

裏  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9829.jpg?raw=true" width="600px" />

### 2. ダイオードをハンダづけする

ダイオードは表面実装型のものを推奨しております。  
スルーホール型も取り付けが可能ですが、キースイッチプレートをPCBにタイトに取り付ける必要がありますので、表面のハンダの盛り上がりを極力抑える必要があります。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9853.jpg?raw=true" width="600px" />

表面にハンダが流れないようにマスキングテープで塞ぎます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9838.jpg?raw=true" width="600px" />

ダイオードの取り付け位置を確認します。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9850.jpg?raw=true" width="600px" />

以下の動画のようにダイオードを取り付けます。  

https://user-images.githubusercontent.com/4215759/126895350-43ae4cd4-408b-4ff4-ab5c-2903e0420978.mov

片側にハンダを事前に盛り付けます(予備ハンダ)。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9852.jpg?raw=true" width="600px" />

ピンセットでダイオードを持ちながら予備ハンダを溶かして片側のハンダ付けを行います。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9854.jpg?raw=true" width="600px" />

もう一箇所もハンダ付けを行います。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9855.jpg?raw=true" width="600px" />

全部で38箇所のハンダ付けを行います。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9859.jpg?raw=true" width="600px" />

### 3. リセットスイッチの取り付け

リセットスイッチを取り付けます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9861.jpg?raw=true" width="600px" />

ダイオードと同じ要領で一部に予備ハンダを置きます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9863.jpg?raw=true" width="600px" />

合計4箇所をハンダ付けします。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9877_2.jpg?raw=true" width="600px" />

### 4. Pro Microを取り付ける

キーボードの入力を処理する部分としてPro Microを取り付けます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9866.jpg?raw=true" width="600px" />

取り付け位置はPCB中央の奥側、表面です。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9868.jpg?raw=true" width="600px" />

取り付けの際に、Pro MicroのピンとPCBのピンが合致することを確認してください。  
PCBはBLE Micro Proに対応するために13ピンとなっております。(Pro Microは12ピン)  
一番奥側のピンはBLE Micro Pro用になっております。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9870.jpg?raw=true" width="600px" />

Pro Microをはんだ付けします。  
miniZoneのPCBはコンスルーに対応しております。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9872.jpg?raw=true" width="600px" />

ファームウェアは[Remapサイト上でインストールする](https://remap-keys.app/catalog/w4Y6eN0uA5mSJ4qyGqcC/firmware)ことも可能です。  
<img src = "https://user-images.githubusercontent.com/4215759/162598262-265cbee5-1e7b-4f7f-b9ec-6a0220455873.png" width="600px" />

QMKへのプルリクエストは[こちら](https://github.com/qmk/qmk_firmware/pull/16644)にございます。

Pro MicroをPCBに取り付けた後、ファームウェアを書き込んで2.で取り付けたダイオードの動作をチェックします。  
キースイッチ穴をショートさせて(キースイッチ穴をピンセットなどでつなぐ)キーが入力されるかを確認します。  

<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9874.jpg?raw=true" width="600px" />


### 5. LEDを取り付ける

LEDの取り付けは、最後でも問題有りません。  
LEDを取り付けなくてもキーボードは動作します。

LED1番のみ、[SK6812MINI-E](https://shop.yushakobo.jp/products/sk6812mini-e-10)を使います。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9884.jpg?raw=true" width="600px" />

中央手前側、PCB裏面に取り付けます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9885.jpg?raw=true" width="600px" />

ダイオードやリセットスイッチの取り付けと同じく、予備ハンダを行います。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9886.jpg?raw=true" width="600px" />

4箇所をはんだ付けします。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9888.jpg?raw=true" width="600px" />

はんだ付けができたらPro MicroをUSBでPCなどに取り付けて光るかを確認します。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9889.jpg?raw=true" width="600px" />

LED2番から11番の計10個は[WS2812B](https://shop.yushakobo.jp/products/a0800ws-01-10)を使います。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9891.jpg?raw=true" width="600px" />

こちらも同様に予備ハンダを行った後に、LEDを取り付けます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9893.jpg?raw=true" width="600px" />

全箇所が点灯することを確認します。  
点灯しない場合は、 `RGB_TOG` キーをキーマップに設定し、キーを押してみてください。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0214.jpg?raw=true" width="600px" />

### 6. OLEDピンソケットの取り付け

この工程は後回しにしても構いません。

[OLED](https://shop.yushakobo.jp/products/oled/)や[トラックボールモジュール用レベル変換基板](https://shop.yushakobo.jp/products/a0800tl-01-1)を使用する際には[OLED用ピンソケット](https://shop.yushakobo.jp/products/a1600ps-01-1)を取り付けるとスムーズに付け替えが可能です。  

<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0226.jpg?raw=true" width="600px" />

取り付け位置は、ProMicroの手前側です。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9899.jpg?raw=true" width="600px" />

取り付ける際は、マスキングテープなどで固定するとハンダ付けがスムーズに行えます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0236.jpg?raw=true" width="600px" />

裏側からハンダ付けを行います。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9901.jpg?raw=true" width="600px" />

### 7. キースイッチプレートとキースイッチの取り付け

miniZoneはKailh Choc v1キースイッチとCherry MX互換のキースイッチに対応しております。  
**Cherry MX互換キースイッチを利用する際は、スイッチプレートの取り付け位置に留意ください。場合によってはスペーサーとネジを別途購入いただくのが良いかと思います。**

キースイッチプレートから保護紙を剥がします。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9839.jpg?raw=true" width="600px" />

キースイッチプレートをPCBの表面に載せます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0217.jpg?raw=true" width="600px" />

キースイッチプレートにキースイッチを8個ほどはめて、仮止めを行います。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0218.jpg?raw=true" width="600px" />

PCBを裏返してキースイッチをハンダ付けします。  
裏返す際にマスキングテープで固定しておくと作業がスムーズに行えるかと思います。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0220.jpg?raw=true" width="600px" />

キースイッチの足を2箇所ハンダ付けすれば完了です。  
他の箇所も同様にハンダ付けを行います。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0221.jpg?raw=true" width="600px" />

全部で38箇所にキースイッチを取り付けます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0223.jpg?raw=true" width="600px" />

### 8. スペーサーの取り付け

Pro Microプレートを取り付ける際に支柱となるスペーサーを取り付けます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0232.jpg?raw=true" width="600px" />

下図のように4箇所にスペーサーを取り付けます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0236.jpg?raw=true" width="600px" />

取り付けの際は5mmのネジを使用します。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0256.jpg?raw=true" width="600px" />

下図のようにPCBの裏面からネジでスペーサーを固定します。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0234.jpg?raw=true" width="600px" />

### 9. 側面プレートとボトムプレートの取り付け

側面プレートの保護シートを剥がします。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0237.jpg?raw=true" width="600px" />

側面プレートはPCBの裏側からPCBの外周を覆うように取り付けます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0238.jpg?raw=true" width="600px" />

ボトムプレートも同様に保護シートを剥がします。  
肉抜き部分にアクリル片が残っている場合はドライバーやピンセットなどで押し込んで取り出してください。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0240.jpg?raw=true" width="600px" />

ボトムプレートをPCBの裏面に載せます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0243.jpg?raw=true" width="600px" />

8mmのネジとナットを用いてキースイッチプレート・側面プレート・ボトムプレートを固定します。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0245.jpg?raw=true" width="600px" />

10箇所にネジを取り付けます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0248b.jpg?raw=true" width="600px" />

底面からナットでネジを固定します。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0249.jpg?raw=true" width="600px" />

Pro Micro付近のネジ穴のみ、ボトムプレートから8mmネジを取り付けます。  
この箇所はスペーサーでネジを固定します。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0250.jpg?raw=true" width="600px" />

下図のようにスペーサーを取り付けます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0253.jpg?raw=true" width="600px" />

### 10. Pro Microプレートの取り付け

Pro Microプレートから保護シートを剥がします。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0255.jpg?raw=true" width="600px" />

Pro Microプレートをスペーサーに取り付けます。  
取り付けの際は5mmのネジを用います。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0259.jpg?raw=true" width="600px" />

### 11. ゴム足シールの取り付け

ゴム足シールを取り付けます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0260.jpg?raw=true" width="600px" />

個人のお好みでつけて頂く感じが良いかと思います。
取り付け例は以下になります。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0263.jpg?raw=true" width="600px" />

### 12. キーキャップの取り付け
キーキャップを取り付けます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0267.jpg?raw=true" width="600px" />

### 13. 完成したら...

完成しましたら、ぜひSNSなどに写真を投稿頂ければと思います。
Twitterのハッシュタグは [`#miniZone #自作キーボード`](https://twitter.com/search?q=%23%E8%87%AA%E4%BD%9C%E3%82%AD%E3%83%BC%E3%83%9C%E3%83%BC%E3%83%89%20%23miniZone&src=typed_query) を付けていただけると幸いです。
キットを組み立てた感想や、キーボードを使った所感などをお待ちしております！

また、毎週日曜日の１9時より実施されている[#KEEP_PD](https://twitter.com/hashtag/KEEB_PD?f=live)に投稿頂くこともオススメです。  
開催の告知は[@KEEB_PD](https://twitter.com/KEEB_PD)にて行われております。

ご不明な点などございましたら、[@takashicompany](https://twitter.com/takashicompany)にメンションやDM頂ければ回答できるかと思います。

### 14. オプション : OLEDの取り付け

miniZoneはOLEDを取り付けることが可能です。  
「 6. OLEDピンソケットの取り付け」を事前に行うとスムーズに進められます。
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0289.jpg?raw=true" width="600px" />

OLED用のファームウェアをPro Microに書き込みます。  
[こちら](https://remap-keys.app/catalog/w4Y6eN0uA5mSJ4qyGqcC/firmware)から「Default VIA」を書き込むことも可能です。  
OLEDとピンヘッダをハンダ付けする際は、ピンソケットに差し込んだ状態で行うとスムーズに作業が可能です。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0294.jpg?raw=true" width="600px" />

OLED用のPro Microプレートを取り付けて完成です。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0297.jpg?raw=true" width="600px" />

### 15. オプション : トラックボールの取り付け

[7mmオプティカルトラックボールモジュール１uタイプ](https://shop.yushakobo.jp/products/adtb7m?variant=37665336164513)を取り付けることができます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9933.jpg?raw=true" width="600px" />


取り付けの際は[トラックボールモジュール用レベル変換基板](https://shop.yushakobo.jp/products/a0800tl-01-1)を用います。  
「 6. OLEDピンソケットの取り付け」を事前に行うとスムーズに進められます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9930.jpg?raw=true" width="600px" />

最終的な取り付けのイメージは以下になります。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0317.jpg?raw=true" width="600px" />

トラックボールモジュールの配線を上述の図のような取り付けができるように長さを調整します。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9936.jpg?raw=true" width="600px" />

導線を切断しないようにカッターでビニール膜に切れ込みを入れていきます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9937.jpg?raw=true" width="600px" />

下図のように導線の部分を長めに出しておくとハンダ付けの際に調整がしやすいです。
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9938.jpg?raw=true" width="600px" />

下図のように導線を折り込むようにハンダ付けをすると外れづらくなります。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9939.jpg?raw=true" width="600px" />

表面は下図のようになるようにトラックボールモジュールをハンダ付けし、またピンヘッダを変換基盤にハンダ付けで固定します。
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9940.jpg?raw=true" width="600px" />

トラックボールモジュールの導線が折れないように、トラックボールモジュールをPro Micro上に配置します。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0317.jpg?raw=true" width="600px" />

トラックボールモジュール用のPro Microプレートを取り付けます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0319.jpg?raw=true" width="600px" />

トラックボール用のファームウェアは[Remap](https://remap-keys.app/catalog/w4Y6eN0uA5mSJ4qyGqcC/firmware)にて配布しております。
また、トラックボール用のソースコードはQMKへのプルリクエストを送っていないため、実装を確認したい方は[こちら](https://github.com/takashicompany/qmk_firmware/tree/minizone/trackball/keyboards/takashicompany/minizone/keymaps/trackball)を御覧ください。

トラックボールを指定時間(デフォルトは10ミリ秒)の間連続して操作すると、マウス入力レイヤー(デフォルトではレイヤー9)が有効になり、クリックやドラッグ、ホイールスクロールが入力可能になります。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/trackball_via.png?raw=true" width="600px" />


[Remap](https://remap-keys.app/)上で任意の箇所にマウス入力を設定することも可能です。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/trackball_custom.png?raw=true" width="600px" />

|Code|入力|備考|
|:--|:--|:--|
|0x5DA6|クリック1|左クリック|
|0x5DA7|クリック2|右クリック|
|0x5DA8|クリック3|デバイスに依存|
|0x5DA9|マイスホイールモード|押下している間、トラックボールの操作がマイスホイールの入力して扱われる|

### 16. BLE Microと電池基盤の取り付け

miniZoneはBLE Micro Pro用の電源を搭載して、Bluetoothによる無線接続が可能です。 
<img src = "https://cdn.shopify.com/s/files/1/0532/0880/9633/products/DSC0005_2048x2048.jpg?raw=true" width="600px" />

また、12ピンのコンスルーやピンヘッダでもPCBに取り付けることが可能です。  
下図の赤丸部分を空けたままにしても動作が可能です。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9955b.jpg?raw=true" width="600px" />

電池ホルダーとして[HU1632](https://www.monotaro.com/p/8835/2765/)をPCBに取り付けることが可能です。  
使用するボタン電池はCR1632となります。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9950.jpg?raw=true" width="600px" />

電池ホルダーをPCBに取り付ける際は、マスキングテープなどで固定すると作業がスムーズに進められます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9952.jpg?raw=true" width="600px" />

以下の箇所をハンダ付けします。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9954b.jpg?raw=true" width="600px" />

[チップ積層セラミックコンデンサー](https://akizukidenshi.com/catalog/g/gP-02151/)をPCBに取り付けます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9876.jpg?raw=true" width="600px" />

予備ハンダをしてコンデンサーをハンダ付けします。向きは特にありません。
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9880.jpg?raw=true" width="600px" />

電源の[スイッチ(MK12C02)](https://ja.aliexpress.com/item/32798526843.html)を取り付けます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9957.jpg?raw=true" width="600px" />

合計7箇所をハンダ付けします。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9959.jpg?raw=true" width="600px" />

下図のようにボタン電池(CR1632)を取り付けて完成です。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0445.jpg?raw=true" width="600px" />

BLE Micro Pro用のトラックボールの実装は[こちら](https://github.com/takashicompany/bmp_qmk_firmware/tree/minizone/keyboards/takashicompany/minizone/keymaps/default)になります。

上述のソースコードからBLE Micro Pro用のファームウェアをビルドするか、[こちら](https://github.com/takashicompany/minizone/releases/download/v1.0.0/takashicompany_minizone_default.uf2)からダウンロードしたものを[BLE Micro Proに書き込んでください](https://sekigon-gonnoc.github.io/BLE-Micro-Pro/#/build_firmware?id=%e7%94%9f%e6%88%90%e3%81%97%e3%81%9f%e3%83%95%e3%82%a1%e3%83%bc%e3%83%a0%e3%82%a6%e3%82%a7%e3%82%a2%e3%82%92%e6%9b%b8%e3%81%8d%e8%be%bc%e3%82%80)。

### 17. Pimoroni Trackballモジュール(PIM447)の取り付け

<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0500.jpg?raw=true" width="600px" />

<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0502.jpg?raw=true" width="600px" />

<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0553.jpg?raw=true" width="600px" />

<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_0551.jpg?raw=true" width="600px" />

