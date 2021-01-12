# roboshisukadai2
ロボットシステム学課題2
# 動作環境
OS:Ubuntu 20.04を使用
# 使用した道具
Raspberry Pi4
パソコン
# 内容
上田先生の授業内でのプログラムをもとに作成し、自身で設定した文字が出力されるように改良した
# インストール手順

```
$ cd ~/catkin_ws/src
$ git clone https://github.com/miyabi-shimada/roboshisukadai2.git
$ cd ~/catkin_ws
$ catkin_make
$ source ~/.bashrc
端末1$ cd catkin_ws/src
端末2$ cd catkin_ws/src
端末3$ cd catkin_ws
端末4$ cd catkin_ws/src 

```

の順番でインストールしていく
# 動作方法
1. 端末を4つ用意する
2. 端末1に``` roscore``` と入力
3. 端末2に``` chmod +x count.py```
 ``` rosrun mypkg count.py```
4. 端末3に``` rostopic list``` を入力し、```count```が入っているか確認
　その後、``` rostopic echo /count _up ```
5. 端末4に``` chmod +x twice.py ```
```rosrun mypkg twice.py ```を入力

# 協力者
加藤舞子、西廣巧
# YouTubeURL
https://youtu.be/ex6dHhbF-gU
# 作成者
上田先生　嶋田雅
# ライセンス
BSD 3-Clause License
