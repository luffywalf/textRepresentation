##### 网上blog阅读 自己整理的笔记 参考见下
参考：https://www.jianshu.com/p/40fbe2bdffd3

#### topic model
* 就是一系列相关的概念 就像一个桶 和这个主题相关度很高的词会被装进这个桶里； 
* 用数学角度说，主题就是词汇表上词语的条件概率分布，与主题密切相关的词，条件概率p(w|z)越大
* 一个词可以装到不同的桶里，一段文字往往含有多个主题
* p(w|d)=∑p(w|z)p(z|d) 
* 用途：
    * 计算文本相似性，考虑到文本语义，避免多义词，同义词的影响
    * 文本聚类，用户聚类
    * 去除噪音，保留最正确的主题，更好的刻画文本主题
          
##### TFIDF
如何自己写以及如何用tfidfvectorizor都比较熟了

##### 基于矩阵分解的LFM - latent factor model
参考：https://yq.aliyun.com/articles/152083
* 常用于推荐系统
* 原理就是用中间的主题latent factor将user-item矩阵分解，即将user, item通过topic联系起来，变为P矩阵：user * topic 和Q矩阵：topic * item，通过梯度下降法不断用P * Q去逼近原本的user-item矩阵 数学上大概是 矩阵的uv分解，将很大的一个稀疏矩阵用两个低维的矩阵去估计逼近～














