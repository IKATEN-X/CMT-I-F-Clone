# CMT Interface Unit (Casio FA-32) クローン
CasioのMSX(MX-10/101/PV-7)用CMTインターフェイスのクローンです  

MX-10でテープゲームをしたいなと思いましたが、Casio製のCMTインターフェイス FA-32をオークションで入手しようとすると結構なお値段で出ていて躊躇してました。   
また、所有されている方の中でも故障しだしたりしている人もチラホラいるようだったので、自作できないかと調査してました。  
すると、  
https://basshp.blogspot.com/2015/03/casio-fa-32-clone-interface-de-cassete.html  
こちらで調査の上、回路図を公開されている方がいたので、なんとか回路を解釈し、基板を作ってみました。  

<img src="https://github.com/IKATEN-X/CMT-I-F-Clone/blob/main/image1.jpg" width="300">  
作成に当たり、部品を集めていたところ、トランジスタのBC550/BC547が手に入りずらいので2SC1815Lで、5Vリレーが5端子のもののところ6端子のモノを買ってしまったのでそれで組み替えています。  
下の図が、組み替えた回路図です。  
(初めて使ったFriztingで作った回路図で、コネクタが変ですがご勘弁ください）  
<img src="https://github.com/IKATEN-X/CMT-I-F-Clone/blob/main/image2.jpg" width="300">
<img src="https://github.com/IKATEN-X/CMT-I-F-Clone/blob/main/image3.jpg?raw=true" width="300">  

| 記号  | 容量・サイズ・数 |  
| ------------- | ------------- |  
| R1  | 6.8kΩ |  
| R2～R6  | 10kΩ |  
| R7  | 100Ω |  
| R8  | 1kΩ  |  
| C1  | 電解コンデンサ 1μF |  
| C2  | セラミックコンデンサ 22nF(0.022uF)  |  
| D1  | 1N4001 |  
| Q1、Q2  | 2SC1815L (ECB)<br>(BC550だとCBEなのでダメです） |  
| K2  | N4100HS3 5V |  
| 3.5mmモノラルケーブル | 2本 |  
| 2.5mmモノラルケーブル | 1本 |  
|ケース(72×47.5mm対応) | TB-32-B・TB-32-IV |  
|タッピングビス 3×5| 4本 |  
  
ケースは必須ではないので、あくまで組み立て時に使用したものです。
ケースに入れると結構大きくなります。  
<img src="https://github.com/IKATEN-X/CMT-I-F-Clone/blob/main/image4.jpg?raw=true" width="300">  
  
ガーバーデータのzipファイルも置いてありますので、これをJLCPCBにアップすれば、そのまま基盤を作ることも可能です。
  
回路もそれほど複雑ではないのでブレッドボードで試しで作ることもできます。  
<img src="https://github.com/IKATEN-X/CMT-I-F-Clone/blob/main/image5.jpg?raw=true" width="300">  
