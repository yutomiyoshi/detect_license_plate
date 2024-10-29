### 目的

#### mada



### 開発準備

main.ipynbの案内に沿ってタスクを実行していく前に、1.2.を実行。

#### 0. 訓練データの準備（アノテーション）

元データとなる画像を数十から数百程度用意する。

各画像のナンバープレートの位置をYOLO形式で出力したテキストファイル（.txt）を生成する。（参考URL No.1）

画像とテキストファイルのデータセットを訓練用と評価用に分割して以下のように配置する。

```
datasets
├　images
│　├　train
│　│　└　画像(.jpg)
│　└　val
│　 　└　YOLO形式(.txt)
└　labels
 　├　train
 　│　└　画像(.jpg)
 　└　val
 　 　└　YOLO形式(.txt)
```


#### 1. YOLOのインストール

```
git clone https://github.com/ultralytics/yolov5
```

#### 2. pipインストール

YOLOの運転に必要なパッケージの取り込み。

```
pip install -r yolov5/requirements.txt
```


### 参考URL

| No. | 内容 |
| --- | --- |
| 1 | [画像からYOLO形式アノテーションを生成する。](https://dev-partner.i-pro.com/space/TPFAQ/1007060562/%E3%82%A2%E3%83%8E%E3%83%86%E3%83%BC%E3%82%B7%E3%83%A7%E3%83%B3%E3%83%84%E3%83%BC%E3%83%AB%E3%80%8ElabelImg%E3%80%8F%E3%82%92%E4%BD%BF%E3%81%A3%E3%81%9FAI%E3%83%A2%E3%83%87%E3%83%AB%E4%BD%9C%E6%88%90) |
| 2 | - |