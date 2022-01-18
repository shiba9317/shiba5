# 2021年度ロボットシステム学：課題1「myled.c」

## 概要
・課題1「myled.c」とは、2021年後のロボットシステム学課題1の、Raspberry Pi 3・LED・ブレットボード・配線・抵抗等を使用し、
echo 1 > /dev/myled0でON/OFを切り替え、LEDを光らせるという物である。

## 目的
・Ubuntu18.04をOSとして利用し、Raspberry Pi 3 等でLEDを光らせる事を目的とする。

## 動作環境
・Ubuntu18.04（OS）

## 使用する物
・Raspberry Pi　3　×1

・LED　×1

・ブレットボード　×1

・配線（オスメスジャンパーピン）　×2

・抵抗　×1

## 全体図
![Screenshot_2022-01-06-12-52-50-88 882](https://user-images.githubusercontent.com/92848929/148341496-f8ad5920-cb3d-4f7b-88de-b9204515a768.png)

## 参考資料
![Screenshot_2022-01-06-12-53-14-63 881](https://user-images.githubusercontent.com/92848929/148341840-8edb8a74-7819-4745-aedd-087691377ba3.png)

・URL→https://www.raspberrypi.org/documentation/usage/gpio/README.md (GPIO and the 40-pin Header)
## 実行操作
1．Ubuntu18.04を立ち上げる

2．Raspberry Pi 3 に電源を入れ、Ubuntu18.04に接続する

3．ブレットボードにLEDと配線と抵抗を、下の写真のように設置する

![IMG20220106125503 884](https://user-images.githubusercontent.com/92848929/148341654-c723e299-4758-4925-979d-41553e379d16.jpg)

4．ブレットボードの配線をRaspberry Pi 3のGPIO25とGroundに、下の写真のように接続する

![Screenshot_2022-01-06-12-53-21-59 883](https://user-images.githubusercontent.com/92848929/148341728-e95884b4-b6ec-4767-8a68-07ce03001c86.png)

5．vi myled.cと打ち込み、ファイルを作る

6．myled.cにプログラムを書き込む

7．wqでファイルを保存する

8．makeと打ち込み、ファイルをコンパイルする

9．コマンドsudo install myled.koを実行する

10．コマンドsudo chmod 666 /dev/myled0を実行する

11．echo 1 > /dev/myled0と打ち込み、LEDを光らせる

12．echo 1 > /dev/myled1と打ち込み、LEDの光を、消す

## ライセンス
・GNU General Public License

## 動作
・youtubeにて、その動作を確認できる動画を公開する

・URL→https://youtube.com/shorts/TBEo0DftCY4?feature=share
