# yolo相关知识

## v5 

- yaml(`Yet another Markup Language`)文件用来配置数据库、网络结构
- 图片大小是32的倍数：卷积 $2^5 = 32$
- -1代表上一层 
- 训练结束生成：
  - weight文件
  - 效果统计
  - 模型pt文件
  - 图片输出

## v10

- 官方源码，有demo，用户可以自己上传图片验证效果
- docs下有很多介绍，index.md是总目录。
- utils 
  - loss.py 继承了v8。不同之处：v8只计算1次；v10计算2次（由于双标签分配）

- Ultralytics文件下重点看（核心代码）
  - cfg下，data.yaml, model.yaml