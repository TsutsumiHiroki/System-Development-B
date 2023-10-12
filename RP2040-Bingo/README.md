# RP2040-Bingo

# 技術仕様
1. 動作プラットフォーム : [Raspberry Pi Pico](https://www.raspberrypi.com/products/raspberry-pi-pico/)
2. 開発プラットフォーム : Windows OS
3. 開発言語 : Arduino(C/C++)
4. 利用ライブラリ : 特になし．(Arduino開発環境を整えれば自動的にインクルードされるため．)

--- 

# Raspberry Pi Pico

## Raspberry Pi Picoとは？

Raspberry Pi 財団が開発した**RP2040マイコン**を搭載した開発基板．
インターフェースにはI2C, UART, SPI, を搭載．
GPIO pinは豪華にも26本搭載．小さいながらも高性能．

## ピン配置

[Datasheet](../Document/pico-datasheet.pdf#4)の4ページに記載されている．

# Arduino-Pico

[Arduino-Pico | Github](https://github.com/earlephilhower/arduino-pico)

Arduinoの持つエコシステムにRP2040を対応．

## ドキュメント

[Arduino-Pico](https://arduino-pico.readthedocs.io/en/latest/)

分かりやすい．(はず)

## インストール

[installation | Github](https://github.com/earlephilhower/arduino-pico#installation)

1. Arduino IDE > ファイル > 環境設定 を開き，"Additional Boards Manager URLs" に.jsonファイルを貼り付ける．
2. ツール > ボード > ボードマネージャー を開き検索欄に"pico"と入れ，Raspberry Pi Pico/RP2040 を追加．

# 動作

Pico のD10番ピンに接続されているタクトスイッチを押すことでランダムな数字が抽選される．

また，抽選が開始するとD25番ピンに接続されているLEDが点灯し，抽選が終わるとLEDが消灯する．

![q](../Movie/IMG_8504.gif)




