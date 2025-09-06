# 100-day-challenge-005
## 今回のテーマ：Unreal Engineで2Dゲームを作る

Paper2D という2D用プラグインを使ってみる  
素材は https://kenney.nl/assets/rolling-ball-assets  
空のレベルを作り、カメラを置いて Orthographic に設定  
ブループリントクラスを作成し、ActorにしてPaddleを作成  
プロジェクト設定の入力の軸マッピングでキー入力を設定。ただしこの軸マッピングは現在は推奨されていない  
PaddleのイベントグラフでInputEventを受け取り、Add Actor Local Offsetで座標移動  
実行すると黒い丸が出る。これはデフォルトゲームモードで作成されたプレイヤー。これを消すために新たにゲームモードを作成し、デフォルトポーンクラスのNoneに設定
