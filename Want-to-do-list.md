# I want to do follow the lists 

## Blender
+ laser expression
+ rig
  + UR5e動かしたい
+ 一部にデカール貼り
+ テクスチャ貼り
+ マテリアルに詳しくなりたい

## Sony Spressense IMU
+ 使いこなし？

## talk with AMR

## AMR predictable reaction

---
## Mermaid記法
```mermaid
graph TD
    A[開始] --> B[処理]
    B --> C[終了]
```


```mermaid
flowchart TD
    A[開始] --> B{判定?}
    B -->|Yes| C((処理1))
    B -->|No| D(終了)
    C --> D
```
- ノード形状: `A[矩形]` `A(丸角)` `A((円))` `A{Rhombus}`
- 矢印: `-->` (実線矢印) `---` (実線) `-.->` (点線)[2]

## シーケンス図（Sequence）
ロボット制御の流れなどに便利です。
```mermaid
sequenceDiagram
    participant U as URロボット
    participant A as AMR
    U->>+A: 移動開始
    A-->>-U: 完了確認
    Note right of A: 座標更新
```
```mermaid
classDiagram
    class Robot {
        -String name
        +move(x, y)
        #privateInit()
    }
    class Sensor
    Robot <|-- Sensor
```

