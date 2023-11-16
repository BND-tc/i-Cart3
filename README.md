# i-Cart3

オープンソース移動ロボットプラットフォームi-Cart3 の制作に必要な情報のリポジトリ

## パーツリスト (Parts list)
100W/200Wモーター版の組立に必要な部品構成表です

60Wモーター版も近日中に公開予定です


## 3Dモデルデータ (3D Model Data)
Parasolid形式とSTEP形式のモデルデータです


## 構成 (Configuraion)
システムおよび回路の構成の資料です

iCart3_Configuration.pdfを参考に配線をしてください

## ソフトウェア (Software)
i-Cart3用のソフトウェアおよび設定ファイルです

### yp-spur(BLVR対応)
> https://github.com/BND-tc/yp-spur

上記ビルドの際にはlibmodbusが必要となります

BLVRにはあらかじめ左右モータードライバにmxex設定ファイルを適用してください

### yp-spur単体実行例
> /usr/local/bin/ypspur-coordinator -d PORT_PATH --blvr -p PARAM_PATH

> /usr/local/bin/ypspur-coordinator -d /dev/ttyUSB0 --blvr -p /home/pi/iCart3_200W.param

### ros実行例
> rosrun ypspur_ros ypspur_ros _ypspur_bin:=/usr/local/bin/ypspur-coordinator _port:=[PORT_PATH]--blvr _param_file:=[PARAM_PATH] _compatible:=1

> rosrun ypspur_ros ypspur_ros _ypspur_bin:=/usr/local/bin/ypspur-coordinator _port:=/dev/ttyUSB0--blvr _param_file:=/home/pi/iCart3_200W.param _compatible:=1

<strong> --blvrオプションの記載をデバイスポートの直後にスペース無しで記載してください。</strong>
