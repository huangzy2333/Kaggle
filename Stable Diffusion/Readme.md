记录第一次参加的Kaggle比赛!

Stable Diffusion Image-to-Prompt

最终靠参考大佬分享的高分方案加自己训练了模型调了一些参拿到了铜牌🥉，但也很高兴拿到这个名次！
>多模态比赛 https://www.kaggle.com/competitions/stable-diffusion-image-to-prompts

* Stable Diffusion比赛相关
* 一些Trick
* 最终提交方案
* Top方案


## 比赛相关
比赛目标

本次比赛的目标是扭转生成文本到图像模型的典型方向：不是从文本提示生成图像，而是可以创建一个模型来预测给定生成图像的文本提示。将对包含由 Stable Diffusion 2.0 生成的各种对的数据集进行预测，(prompt, image)以了解潜在关系的可逆性。

本次比赛一大特色就是不提供训练集，需要自己搜集图像文本匹配数据。


## [Trick]
本次比赛的目标是扭转生成文本到图像模型的典型方向：不是从文本提示生成图像，而是可以创建一个模型来预测给定生成图像的文本提示。将对包含由 Stable Diffusion 2.0 生成的各种对的数据集进行预测，(prompt, image)以了解潜在关系的可逆性。

## [最终方案](https://github.com/huangzy2333/Kaggle/blob/main/Stable%20Diffusion/sd-knnregression-clip-vit.ipynb)
Public LB：0.59181  Private LB：0.58885

## Top方案
记录Top3的方案

## 感想
感觉深度学习比赛真的很靠计算资源，还有现在比拼很多大模型



