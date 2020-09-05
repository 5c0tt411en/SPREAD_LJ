# SPREAD LJ
9月11日のイベントでのLJ用．

# 開発レギュレーション
## 素材
- `tox/MATERIAL_TEMP.tox`から作る
- 各ContainerごとにOut SOPで出し，Merge SOPに繋げる
- SOPで作った素材は -1 < x < 1, -1 < y < 1 となるようにする
- 上記範囲外の場合際枠線がつくので注意．SOPto CHOP > CHOPto SOPとすると解消する
- 音入力を使用する場合は，`/work/MATERIAL_TEMP/container1/`の`select1`(Select CHOP)からパラメタリンクする

## UI
### 素材同士の並び順
上 > 下

### 素材あたりの内部的なUIの並び順
左 > 右 : 素材のON/OFFボタン > ラジオボタン（素材内のモード切替など）> ノブ（パラメタ） > スライダ

### ボタン
- 通常のButton COMPから作る
- 素材名をボタン内テキストで命名する

### ラジオボタン
- `tox/TEMP_RADIO.tox`から作る
- それぞれのボタンの名前を命名する

### ノブ
- `tox/TEMP_KNOB.tox`から作る
- それぞれのボタンの名前を命名する

### スライダ(場所をとるのでできればノブのみで開発)
- 通常のSlider COMPから作る

# TODO
- 素材を増やす
- キーストーンを書けた際，頂点１点目だけ座標がズレるバグ修正