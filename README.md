# 库区多机器人集群路径规划仿真

## 快速开始

仓库多机器人路径规划仿真。

1.安装依赖
```
$ pip install -r requirements.txt
```

2.集中规划
```
$ cd centralized\cbs
$ python cbs.py ..\benchmark\8x8_obst12\map_8by8_obst12_agents9_ex0.yaml output.yaml
$ python ..\visualize.py  ..\benchmark\8x8_obst12\map_8by8_obst12_agents9_ex0.yaml output.yaml

$ python cbs.py ..\benchmark\32x32_obst204\map_32by32_obst204_agents10_ex0.yaml output.yaml
$ python ..\visualize.py ..\benchmark\32x32_obst204\map_32by32_obst204_agents10_ex0.yaml output.yaml
```
3.局部规划
```
$ cd ..\..\decentralized\
$ python decentralized.py -m velocity_obstacle
$ python decentralized.py -m nmpc
```