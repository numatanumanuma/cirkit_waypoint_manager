# cirkit_waypoint_navigator

## About
Sequentialy navigate a robot with waypoints generated by `waypoint_generator`.

## Usage
Copy a waypoint file to `waypoint_navigator/waypoints`. 

にコピーしておきましょう。本当はどこでもいいです。`waypoint_navigator/launch/waypoint_nagigator.launch`の`waypointsfile`をさっき作ったやつに書き換えます。  

実際にナビゲーションしましょう。実機なら
```bash
roslaunch third_robot_2dnav autorun.launch
```
でロボットドライバ他`move_base`などを立ち上げます。
navigatorをlaunchします。
```bash
roslaunch waypoint_navigator waypoint_navigator.launch
```
ロボットが自律移動を始めます。 