
![Typo International](img/work/proj-2/mekaron.JPG)

#### 競技内容
相手の本陣についた風船を全部割るか，相手についた風船をより多く割った方の勝利  
<u>[全国大会の動画](https://www.youtube.com/watch?v=JsvMJymd_TA)</u>

#### コンセプト
動いている相手の風船を割るより，本陣を狙うほうが割りやすいので，猛スピードで相手の本陣まで移動し，2軸の2本のアームを使って風船を割ることにした  

#### ロボットの動作
マウス型コントローラを2つ使い，それぞれの座標に2軸のロボットアームが追従する  

#### 担当箇所
ロボット2台の走行系と2軸アームのプログラムと回路設計  

練習風景は[こちら](https://youtu.be/Er_QlfssfvA)

#### この時に得た能力
PD制御  
躍度最小  
同構造型マスタースレーブの制御

#### 自分がやったことの詳細
クリックして詳細を表示できます  
<details><summary><span class="yubi"><font color=blue><u>人の腕を教示してそれをロボットにフィードバックする部分</u></font></span></summary>  
人の腕に腕の関節の角度を読むセンサを取り付け，その角度をロボットのアームにフィードバックして腕の操作性を上げた  
初めの頃はロボットの腕の関節が片方に4つあったため，人間の肩を2軸，肘，そして腕のひねりを計測し，操作していた
</details>  
<details><summary><font color=blue><u><span class="yubi">作動二輪・3輪オムニの制御</span></u></font></summary>  
作動2輪はタイヤを2個使った走行系で，ロボットの移動速度を上げる目的で使った  
3輪オムニはオムニホイールを3つ使った全方位移動を可能にするために使った
</details>  

<details><summary><span class="yubi"><font color=blue><u>自作マウスとロボットとの通信</u></font></span></summary>  
4軸のアームから2軸のアームに変更した際に自作のマウスを2個使ってアームを制御し，そこから得た値をアームの座標系に変換し，シリアル通信でデータを転送した．  
![Typo International](img/work/proj-2/mosue_update.jpg)
</details>  

<details><summary><span class="yubi"><font color=blue><u>風船を割るパーツの作成</u></font></span></summary>  
風船を簡単に割る道具が必要になり，機械版の手が空いてなかったため，私が設計した．  
![Typo International](img/work/proj-2/spikes.JPG)  
</details>

<details><summary><span class="yubi"><font color=blue><u>相手ロボットと一定の距離を保つプログラム</u></font></span></summary>  
距離センサを3つ使って測定し，そこから得た距離により相手との距離感を保った  
動画は[こちら](https://youtu.be/LpwO2E48w8Y)
</details>  

<details><summary><span class="yubi"><font color=blue><u>発射機構の制御</u></font></span></summary>  
コントローラから発射シーケンスが送られたら，発射するようにした  
動画は[こちら](https://youtu.be/J-SdjVSxDy0)
</details>

#### 反省
あまり新しいことをやってなかった  
コントローラとロボットとの同期に時間がかかりすぎた
#### 感想
この年のロボットはあまり新しいことに挑戦せず，確実に動くロボットを作ったため，昨年より楽に作業が進んだ．
ただ，一番大変だったのは自チームのロボットが4軸あった時のコントローラとの同期だった．  
ロボット側も，コントローラ側もセンサの初期値が毎回変動するため，そこの調整の自動化を怠ったため，時間がかかった．
