# CMT Interface Unit (Casio FA-32) クローン
CasioのMSX(MX-10/101/PV-7)用CMTインターフェイスのクローンです  

MX-10でテープゲームを楽しみたいと思い、Casio純正のCMTインターフェイスFA-32を入手しようとしました。しかし、オークションでは高額で取引されており、手が出しづらい状況でした。また、既に所有している方の中でも故障が発生している例が見受けられ、自作を検討することにしました。  
  
調査を進めたところ、以下のサイトで回路図が公開されているのを発見しました：  
https://basshp.blogspot.com/2015/03/casio-fa-32-clone-interface-de-cassete.html  
  
これを参考にし、回路図を解釈して基板を作成しました。  

<img src="https://github.com/IKATEN-X/CMT-I-F-Clone/blob/main/image1.jpg" width="300">  
  
改良点  
作成時に以下の変更を加えています：  
  
トランジスタの置き換え  
BC550/BC547が入手困難だったため、代わりに2SC1815Lを使用しました（BC550はCBEピン配置のため非互換）。  
  
リレーの置き換え  
5端子の5Vリレーが手に入らなかったため、6端子のリレー（N4100HS3 5V）を使用しました。  
  
以下は組み替え後の回路図です。初めてFriztingを使用して作成したため、コネクタの配置が不自然な部分がありますがご了承ください。  

<img src="https://github.com/IKATEN-X/CMT-I-F-Clone/blob/main/image2.jpg" width="300">
<img src="https://github.com/IKATEN-X/CMT-I-F-Clone/blob/main/image3.jpg?raw=true" width="300">  

必要な部品  

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
  
ケースについて：  
ケースは必須ではありませんが、組み立て時に使用しました。ケースに入れるとサイズが大きくなるため、好みに応じて使用してください。  
<img src="https://github.com/IKATEN-X/CMT-I-F-Clone/blob/main/image4.jpg?raw=true" width="300">  
  
作成方法  
ガーバーデータのZIPファイルを用意しています。これをJLCPCBにアップロードすれば、そのまま基板を製造可能です。また、回路がそれほど複雑ではないため、ブレッドボードで試作することもできます。  
<img src="https://github.com/IKATEN-X/CMT-I-F-Clone/blob/main/image5.jpg?raw=true" width="300">  
