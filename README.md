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

  %% 关系连线（带编号）
  R -->|送快递| M
  D ---|杀手搭档| R
  D -->|喜欢的偶像| W
  W -->|宿敌未认出| V
  M -->|看直播·聊二次元| V
  A ---|酒吧同事| C
  A ---|打游戏认识·偶尔双排| V
  C -->|厨房互助| E
  E ---|心事对象| V

  %% 角色样式
  classDef char fill:#d6eaff,stroke:#2980b9,color:#000,font-weight:bold;
  class M,A,D,C,W,R,V,E char;

  %% 线条颜色
  linkStyle 0 stroke:#2ecc71,color:#2ecc71;  %% R-M 友好
  linkStyle 1 stroke:#2ecc71,color:#2ecc71;  %% D-R 友好
  linkStyle 2 stroke:#e91e63,color:#e91e63;  %% D-W 暧昧
  linkStyle 3 stroke:#e74c3c,color:#e74c3c;  %% W-V 敌对
  linkStyle 4 stroke:#2ecc71,color:#2ecc71;  %% M-V 友好
  linkStyle 5 stroke:#2ecc71,color:#2ecc71;  %% A-C 友好
  linkStyle 6 stroke:#2ecc71,color:#2ecc71;  %% A-V 友好
  linkStyle 7 stroke:#2ecc71,color:#2ecc71;  %% C-E 友好
  linkStyle 8 stroke:#e91e63,color:#e91e63;  %% E-V 暧昧

  %% 图例
  subgraph Legend[图例 Legend]
    F[友好关系]:::char
    H[暧昧关系]:::char
    X[敌对关系]:::char
  end
  linkStyle 9 stroke:#2ecc71,color:#2ecc71;
  linkStyle 10 stroke:#e91e63,color:#e91e63;
  linkStyle 11 stroke:#e74c3c,color:#e74c3c;
