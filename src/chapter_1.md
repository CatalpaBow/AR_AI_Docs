# SquatWaypointを作る
実際に動作するSquatWaypointを実装し、AIシステムについての理解を深めましょう。  
このWaypointの動作には、以下のBehaviorTreeの実装が必要です。
### Squat.bt  
AI兵士が実行するBehaviorTree。屈伸と立ちを一定周期で繰り返し、スクワットをしてるように見せかけている。
### SquatActivity.bt 
AIグループが実行するBehaviorTree。グループメンバー全員に対して個別に**Squat.bt**を呼び出す。  
### SquatWaypoint.bt  
ウェイポイントが実行するBehaviorTree。Waypointが割り当てられたグループに対して**SquatActivity.bt**を呼び出す
最初はSquat.btから実装し、順にSquatActivity.bt,SquatWapoint.btも実装して、最後にSquatWaypointエンティティを実装します。

作成中…