<div align="center">

# Yas-Train
Yet Another Genshin Impact Scanner  
~~又~~ 一个原神 ~~圣遗物~~ 成就导出器

</div>

## 介绍
基于 [wormtql/Yas-Train](https://github.com/wormtql/yas-train) 的魔改版本，主要用途为训练成就的字体识别模型

该仓库为 [Yas-achievement](https://github.com/wjm/achievement) 的模型训练程序
### 相关资料
- [MobileNetV3](https://arxiv.org/pdf/1905.02244.pdf)
- [CRNN](https://arxiv.org/pdf/1507.05717.pdf)

## 使用
假设你会设置基本的pytorch环境。  
- 生成数据集
```
python main.py gen
```
- 训练
```
python main.py train
```
在`mona/config.py`处可以修改数据集大小、epoch等参数

如果要加速大数据集的生成，可以使用`pargen.py`

如果想使用大数据集验证（又不想大量占用硬盘和内存），可以使用`onlineval.py`来进行在线验证
## 感谢
- [wormtql](https://github.com/wormtql) 的原仓库 [Yas-Train](https://github.com/wormtql/yas-train)
