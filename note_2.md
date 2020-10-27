AAAI2020

低资源文本风格迁移数据集
A Dataset for Low-Resource Stylized Sequence-to-Sequence Generation
me: 学习文风口风
应用： 正式文本翻译 有礼貌的机器对话
data： Machine Translation Formality Corpus（MTFC） 和 Twitter Conversation Formality Corpus（TCFC），分别研究机器翻译风格迁移和对话风格迁移

通过预训练生成跨语种自然语言
Cross-Lingual Natural Language Generation via Pre-Training
me： 恕我愚钝 编码解码象限没看懂

基于事实感知的句子切分改写任务与置换不变训练
Fact-aware Sentence Split and Rephrase with Permutation Invariant Training
me： 让机器来拆分带有从句的复杂句子时，对于从句的主语会发生误判，导致歧义。（人也经常会误判
解决方案：恕我愚钝，没看很明白。
        复杂句子中的“事实”是确定的 ，通过 要求 拆分后的短句不可违背复杂句中的“事实”来提升准确率
        可是“事实”要怎么定义，我还没看。
            “本篇论文引入了基于事实感知的句子编码 FaSE 以及置换无关训练的策略 PIT。整个模型的框架如图8所示，FaSE 借助多任务学习的方式使得编码器编码的特征不仅用于句子切分改写任务，同时还用于判断从当前复杂句中是否可以推断出给定的事实。引入事实判定的辅助任务使得模型能够从复杂长句中更好地捕获事实信息，从而提高句子切分的准确率；PIT 策略被广泛用于解决多谈话者场景下语音分离任务中的标签排序问题。在句子切分改写任务中，我们引入 PIT 策略来寻找具有最小损失的排列顺序作为优化的目标，从而缓解由于排列顺序随机性给 seq2seq 模型学习带来的影响，从而使得整个训练过程更加稳定。

            作者：微软亚洲研究院
            链接：https://www.zhihu.com/question/355253606/answer/1004763788
”
data：WebSplit-v1.0 数据集

通过建模隐含的实体类型信息来改进实体链接任务
Improving Entity Linking by Modeling Latent Entity Type Information
me：对于句子中的多义词，机器很难选择正确的那个含义
原因：多个含义间的向量太过接近
解决方案：1 预训练（没有创新）
        2 BERT相关 恕我愚钝 还没看 目前了解BERT是类似word2VECT的东西

