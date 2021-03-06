# M5Stack


## How to set up

M5Stackの開発をするにはPCに環境構築を行う必要がある．ここにセットアップ方法を述べる．

### 1.Arduino IDEをインストール

　[Downloads](https://www.arduino.cc/en/software)からインストールする．全文英語なので頑張って読んでね

### 2.USB ドライバーをインストール

  接続に必要．Macの人は[SILICON LABS](https://jp.silabs.com/developers/usb-to-uart-bridge-vcp-drivers)からダウンロードしてインストーラーを実行してね．Windowsは知らん
  ．
  
  M5stackをmacに繋いだときに、「Tools」 > 「Port」 のところに、「SLAB_USBtoUART」の選択肢が出現すれば問題ナシ．

![image](https://user-images.githubusercontent.com/48522543/110209652-e9752d00-7ed0-11eb-8f68-dcad3d08c243.png)


### 3.環境設定を行う

Pregerences を開き，Additional Boards Manager URLs のテキストボックスの横にあるボタンをクリックし，以下のURLを入力しOKを押す．

**https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json**
 
  ![image](https://user-images.githubusercontent.com/48522543/110209203-78347a80-7ece-11eb-8aa3-a5ac41956871.png)

### 4.esp32のボードを追加する

書き込み先のボードの設定をする．「Tools」>「Board:"******"」>「Boards Manager...」をクリックすると次の様なウインドウが出てくるので，「esp32」と検索して「esp32 by Espressif Systems」をインストールする．

![image](https://user-images.githubusercontent.com/48522543/110209179-51764400-7ece-11eb-979e-59e6d88e09fa.png)

### 5.M5Stackライブラリのインストール

「Sketch」>「Include Library」>「Manage Libraries...」を選択し，「M5Stack by M5Stack」という名前のライブラリをインストールする．

![image](https://user-images.githubusercontent.com/48522543/110209939-956b4800-7ed2-11eb-8fe0-9b5d3a04a4da.png)


### 6.ボードの設定

書き込み時のボード設定を行う．画像の通りに設定すれば良い．
