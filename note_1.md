1 CNN
2 ResNET
3 LSTM
4 XGBoost

1 bn -
    batch nomolization 使得隐含层间数据均匀
2 pooling-
    挑选特征如矩阵中的max值
3 padding- 
    在使用卷积层时 矩阵边缘收到的卷积程度 与其余部分不一致  因此拓展填充图像的边缘（补0或是其他值） 
4 softmax
5 wordVect-
    稀疏矩阵映射为向量
6 Adam
7 SGD
8 Sequence 
    序列学习
        RNN !!!hotfix
        LSTM
9 Regulization--
    L1L2范数惩罚
10 Nomolization-
11 emsemable-
12 loss_type-
13 embedding_size
14 conv_kernel--
    卷积核
15 word2vec 
    和神经网络语言模型不同，直接来学习这个词向量，使用的基本假设是分布式假设，如果两个词的上下文时相似的，那么他们语义也是相似的。
    word2vec分为cbow（根据context预测中心词）和skip-gram（根据中心词预测context）两种。
    但有个问题就是我们的词通常有很多语义的，比如bank是银行还是河岸，具体的意思要取决与上下文，如果我们强行用一个向量来表示语义的话，只能把这两种语义都编码在这个向量里，但实际一个句子中，一个词只有一个语义，那么这种编码是有问题的。
    那么这种上下文的语义可以通过RNN/LSTM/GRU来解决，RNN与普通深度学习不同的是，RNN是一种序列的模型，会有一定的记忆单元，能够记住之前的历史信息，从而可以建模这种上下文相关的一些语义。RNN中的记忆单元可以记住当前词之前的信息。
    但RNN的结构不可支持长期记忆，lstm可以解决RNN长时依赖梯度消失的问题。
16 n-gram词袋
17