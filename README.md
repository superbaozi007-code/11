```mermaid
graph LR
  %% 节点定义
  M[宅宅魅魔 Vivi]
  A[大天使 Lin]
  D[小恶魔 Kokoro]
  C[猫咪 Nyao]
  W[狼人 Ravena]
  R[蟑螂忍者 Kuro]
  V[吸血鬼 Lilith]
  E[精灵女仆 Faye]

  %% 关系连线（标号方便 linkStyle 调整）
  R -->|送快递 Delivery service| M
  D ---|杀手搭档 Assassin partners| R
  R -->|喜欢的偶像 Idol| W
  W -->|宿敌未认出 Rival| V
  M -->|看直播·聊二次元 Watching stream & chat anime| V
  A ---|酒吧同事 Colleague at bar| C
  A ---|打游戏认识·偶尔双排 Partners for online game| E
  W -->|默默follow偶像 Follow idol secretly| D
  C -->|看历史美食直播 Watching stream for food history| V

  %% 应用角色样式
  classDef char fill:#eef7ff,stroke:#2980b9,color:#000,font-weight:bold,font-family:"Helvetica Neue",Helvetica,Arial,sans-serif,stroke-width:2px,rx:15,ry:15;
  class M,A,D,C,W,R,V,E char;

  %% 线条颜色
  linkStyle 0 stroke:#2ecc71,stroke-width:2px,color:#2ecc71;   %% 友好
  linkStyle 1 stroke:#2ecc71,stroke-width:2px,color:#2ecc71;   %% 友好
  linkStyle 2 stroke:#e91e63,stroke-width:2px,color:#e91e63;   %% 暧昧
  linkStyle 3 stroke:#e74c3c,stroke-width:2px,color:#e74c3c;   %% 敌对
  linkStyle 4 stroke:#2ecc71,stroke-width:2px,color:#2ecc71;   %% 友好
  linkStyle 5 stroke:#2ecc71,stroke-width:2px,color:#2ecc71;   %% 友好
  linkStyle 6 stroke:#2ecc71,stroke-width:2px,color:#2ecc71;   %% 友好
  linkStyle 7 stroke:#e91e63,stroke-width:2px,color:#e91e63;   %% 暧昧
  linkStyle 8 stroke:#2ecc71,stroke-width:2px,color:#2ecc71;   %% 友好

  %% 图例
  subgraph Legend[图例 Legend]
    F[友好关系]:::friendly
    H[暧昧关系]:::ambiguous
    X[敌对关系]:::enemy
  end

  %% 图例样式
  classDef friendly stroke:#2ecc71,color:#2ecc71;
  classDef enemy stroke:#e74c3c,color:#e74c3c;
  classDef ambiguous stroke:#e91e63,color:#e91e63;
