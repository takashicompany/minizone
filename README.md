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
(トラックボールを利用する際のソースコードは[こちら](https://github.com/takashicompany/qmk_firmware/tree/minizone/trackball/keyboards/takashicompany/minizone/keymaps/trackball))

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
(Source code for using the trackball is [here](https://github.com/takashicompany/qmk_firmware/tree/minizone/trackball/keyboards/takashicompany/minizone/keymaps/trackball))

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
|M2ネジ 8mm|12||
|M2ネジ 5mm|10||
|M2スペーサー 7mm|6||
|M2ナット|10||

### ご自身で用意頂くもの
|部品|個数|備考|
|:--|:--|:--|
|[Kailh Choc v1キースイッチ](https://shop.yushakobo.jp/collections/all-switches/products/pg1350)|38||
|0.8uキーキャップ(16mm)|38|[Choc 向け 挟ピッチ16mm 薄型キーキャップ](https://make.dmm.com/item/1273303/)、[KNキーキャップセット(Chocスイッチ 16x16mmキーピッチ用) v1.2](https://make.dmm.com/item/1280053/)にて動作することを確認済み|
|Pro Micro|1|BLE Micro Proにも対応済み|

### お好みで
|部品|個数|備考|
|:--|:--|:--|
|コンスルー|2||

### OLEDを搭載する場合
|[OLEDモジュール](https://shop.yushakobo.jp/collections/all-keyboard-parts/products/oled)|1||
|[OLED用ピンソケット](https://shop.yushakobo.jp/products/a1600ps-01-1)|1|ピンヘッダがあれば取り付け自体は可能だが付け替えができなくなるので使用を推奨。|

### トラックボールモジュールを搭載する場合
|[7mmオプティカルトラックボールモジュール１uタイプ](https://shop.yushakobo.jp/products/adtb7m)|1||
|[トラックボールモジュール用レベル変換基板](https://shop.yushakobo.jp/products/a0800tl-01-1/)1||
|[OLED用ピンソケット](https://shop.yushakobo.jp/products/a1600ps-01-1)|1|ピンヘッダがあれば取り付け自体は可能だが付け替えができなくなるので使用を推奨。|

### BLE Micro Pro用に電源を搭載する場合
|部品|個数|備考|
|:--|:--|:--|
|[HU1632](https://www.monotaro.com/p/8835/2765/)|1||
|[チップ積層セラミックコンデンサー](https://akizukidenshi.com/catalog/g/gP-02151/)|1||
|[電源スイッチ(MK12C02)](https://ja.aliexpress.com/item/32798526843.html)|1||
|ボタン

## 組み立て方

### 1. PCBの表と裏を確認する

<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9827.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9829.jpg?raw=true" width="600px" />

### 2. ダイオードをハンダづけする

ダイオードはこちら。  

<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9853.jpg?raw=true" width="600px" />

表面にハンダが流れないようにマスキングテープで塞ぐ。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9838.jpg?raw=true" width="600px" />

ダイオードの取り付け位置を確認。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9850.jpg?raw=true" width="600px" />

片側にハンダを盛り付ける(予備ハンダ)。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9852.jpg?raw=true" width="600px" />

ピンセットでダイオードを持ちながら予備ハンダを溶かして片側のハンダ付けを行う。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9854.jpg?raw=true" width="600px" />

もう一方もハンダ付けを行う。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9855.jpg?raw=true" width="600px" />

全部で38箇所のハンダ付けを行う。
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9859.jpg?raw=true" width="600px" />

### 3. リセットスイッチの取り付け

リセットスイッチを取り付けます。  
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9861.jpg?raw=true" width="600px" />

ダイオードと同じ要領で一部に予備ハンダを置きます。
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9863.jpg?raw=true" width="600px" />

4箇所をハンダ付けします。
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_9877_2.jpg?raw=true" width="600px" />

### 4. Pro Microを取り付ける

キーボードの頭脳部分としてPro Microを取り付けます。  
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

最終的な取り付けのイメージは以下です。
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

