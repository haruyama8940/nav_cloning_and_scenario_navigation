# nav_cloning_and_scenario_navigation

## Introduction  
このリポジトリはnav_cloningとscenario_navigationを組み合わせた，ナビゲーションに関して
環境の作成方法をまとめたリポジトリです．
主に下記のリポジトリをセットアップします．
* [nav_cloning](https://github.com/haruyama8940/nav_cloning)
* [intersection_detector](https://github.com/haruyama8940/intersection_detector)
* [scenario_navigation](https://github.com/haruyama8940/scenario_navigation)
* [orne_navigation](https://github.com/haruyama8940/orne_navigation)
* [real_tsudanuma2-3_sim](https://github.com/masakifujiwara1/real_tsudanuma2-3_sim)

## Install
* system requirements
  * Ubuntu 20.04 LTS
  * ROS noetic
  * Python3
  * Pytorch
  * cuda
  * cuDNN
  
* make workspace
```
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/src
catkin_init_workspace
cd ../
catkin_build
```
* nav_cloning
```
git clone -b pytorch https://github.com/haruyama8940/nav_cloning
git clone https://github.com/MoriKen254/timed_roslaunch.git
```
* scenario_navigation
```
git clone -b intersection https://github.com/haruyama8940/scenario_navigation.git
```
```
sudo apt install mecab
sudo apt install libmecab-dev
pip3 install mecab-python3
```
```
git clone --depth 1 https://github.com/neologd/mecab-ipadic-neologd.git
cd mecab-ipadic-neologd
./bin/install-mecab-ipadic-neologd -n
```

* scenario_navigation_msgs
```
git clone https://github.com/haruyama8940/scenario_navigation_msgs.git
```
* intersection_detector
```
git clone -b merge_scenario https://github.com/haruyama8940/intersection_detector.git
```


