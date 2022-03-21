# miniZone

![image](https://github.com/takashicompany/minizone/blob/master/images/qmk.jpg?raw=true)

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

---

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
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />

<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />

<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />

<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />

<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
<img src = "https://github.com/takashicompany/minizone/blob/master/images/build/IMG_.jpg?raw=true" width="600px" />
