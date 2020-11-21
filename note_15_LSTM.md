#  NN for seriers data

    对于一个序列数据来说，我们通过序列的前n项来推测第n+r项

    以 预测下一词 为例 ：  
        y 词2
        x 词1 

```mermaid
    graph TB
  
    x --> LSTM --> opt --> LSTM --> y

    

```