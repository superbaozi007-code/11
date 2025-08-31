# 11
```mermaid
graph LR
  %% 节点定义
  M[魅魔 Vivi]
  A[天使 Lin]
  D[小恶魔 Kokoro]
  C[猫猫 Nyao]
  W[狼人 Ravena]
  R[蟑螂忍者 Kuro]
  V[吸血鬼 Lilith]
  E[精灵 Faye]

  %% 关系连线
  R -->|送快递 Delivery service| M:::friendly
  D ---|杀手搭档 Assassin partners| R:::friendly
  R -->|喜欢的偶像 Idol| W:::friendly
  W -->|宿敌未认出 Rival | V:::enemy
  M -->|看直播·聊二次元 Watching stream & chat anime| V:::friendly
  A ---|酒吧同事 Colleague at bar| C:::friendly
  A ---|打游戏认识·偶尔双排 Partners for online game| E:::friendly
  W -->|默默follow偶像 Follow idol secretly| D:::friendly
  C -->|看历史美食直播 Watching stream for food history| V:::friendly

   %% 样式定义
  classDef friendly stroke:#2ecc71,color:#2ecc71;
  classDef enemy stroke:#e74c3c,color:#e74c3c;
  classDef ambiguous stroke:#e91e63,color:#e91e63;
  classDef char fill:#d6eaff,stroke:#2980b9,color:#000,font-weight:bold;

  %% 应用角色样式
  class M,A,D,C,W,R,V,E char;

  %% 图例
  subgraph Legend[图例 Legend]
    F[友好关系]:::friendly
    H[暧昧关系]:::ambiguous
    X[敌对关系]:::enemy
  end
