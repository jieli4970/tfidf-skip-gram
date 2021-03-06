​	首先计算出tfidf值最大的若干个词语，然后把这些词语转化成当前文本的词向量表示形式，接着计算出当前文本的词向量和其中一类的文本类别向量的余铉相似度值，接着用该值和给定的文本类别的阈值相比较，根据比较结果类对该文本进行分类。

本文在判断文本类别时，利用了TFIDF和Skip-gram相结合的方法来计算，同时考虑了词汇在文本中的重要程度，也兼顾了词与词之间的语义关系，很好体现了Skip-gram模型通过词向量预测上下文的应用，实验证明，该方法在一定范围内是很有效的。

​       由于选取的语料比较少，同时用到的语料参差不齐，导致测试结果的准确性受到一定的影响。接下来将不断寻找新的语料库，并对语料进行进一步的筛选，同时逐步提高语料的规模，再选取一些更加有效的方法作文文本相似度的训练器，给相似度的实际测试奠定良好的基础。

参考：结合TFIDF方法与Skip_gram模型的文本分类方法研究_邬明强 百度学术

算法流程：

![流程图](http://p94g7wqy4.bkt.clouddn.com/study/master/%20informationRetrieving/%E5%9B%BE1.PNG)