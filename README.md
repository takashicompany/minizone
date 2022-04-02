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
