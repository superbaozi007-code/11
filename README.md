# 11
```mermaid
graph LR
  %% 节点定义
  M[魅魔 Mira]
  A[天使 Seraphina]
  D[小恶魔 Vivi]
  C[猫猫 Neko]
  W[狼人 Selene]
  R[蟑螂忍者 Kuroko]
  V[吸血鬼 Camille]
  E[精灵 Evelyn]

  %% 关系连线
  R -->|送快递| M:::friendly
  D ---|杀手搭档| R:::friendly
  D -->|喜欢的偶像| W:::ambiguous
  W -->|宿敌未认出| V:::enemy
  M -->|看直播·聊二次元| V:::friendly
  A ---|酒吧同事| C:::friendly
  A ---|打游戏认识·偶尔双排| V:::friendly
  C -->|厨房互助| E:::friendly
  E ---|心事对象| V:::ambiguous

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
