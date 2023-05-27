训练过程
>借鉴各位大佬的，自己对代码和模型知道的还是太少了

* [数据处理](#数据处理)
* [训练单模型](#训练单模型)
* [KNN](#KNN)
* [Clip](#Clip)
* [模型集成](#模型集成)


## 数据处理
首先是对diffusiondb-2m的数据进行筛选，（1）筛选仅英文，（2）筛选图片尺寸长宽为512✖️512的图片，（3）prompt长度大于5，（4）没有特殊符号的，（5）头和尾各15个字符相同的prompt删除重复的，也可以用cossimilarity>0.8（可以自己调整阈值）来删除相似的prompt。最终得到一拥有462636条prompt和对应图片地址的data。

利用他人产生的图片prompt配对data，大多是用chatgpt组合产生出prompt，再用sd2生成图片。

最终使用的数据集样本量为576668。主要也是因为计算资源有限，kaggle的免费计算资源承受不了再大的数据集跑模型了。


## 训练单模型
#### [Vit]()
(1)vit_base_patch16_224 -> vit_large_patch16_384 单模型效果提升

#### [Clip-Vit]()
clip-vit-large-patch14(https://www.kaggle.com/competitions/stable-diffusion-image-to-prompts/discussion/398529)
非常巧妙地训练模型达到0.58+的一种方法，我也是用这个单模型训练57万数据达到了我的单模型最高lb：0.55835

## KNN

## ClipInterrogator

## 模型集成
(1)CLIPInterrogator+OFA+ViT



