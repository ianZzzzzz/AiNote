convet optimization
性质：
    凸优化只存在全局最小值 不存在局部最小值
    如果一组约束是线性等式约束，则它确定的可行域是一个凸集。
    如果一组约束是线性不等式约束，则它定义的可行域是凸集。
    在实际应用中，我们遇到的等式和不等式约束一般是线性的，因此非常幸运，它们定义的可行域是凸集。
    一个重要的结论是：多个凸集的交集还是凸集
    凸集的并集并不是凸集。
    凸集是连续的 全体实数集是凸集
凸集定义：
    集合内任意两点间的连线上的任何一点都在集合内 即为凸集
凸函数：
    曲线上任意两点连线都位于函数上方
    函数在任何点处的切线都位于函数的下方。
    对于一元函数，凸函数的判定规则为其二阶导数大于等于0 （二阶导大于0 有极小值 反之有极大值
    对于多元函数，引入Hessian矩阵，其可认为是二阶导向多元函数的推广（所以是个对称矩阵 求导次序无关），
    若Hessian矩阵半正定 函数为凸函数 
    正定则严格凸函数（通俗理解 正定>0 半正定>=0 负定<0)
    
    根据多元函数极值判别法，假设多元函数在点M的梯度为0，即M是函数的驻点，则有：

        1.如果Hessian矩阵正定，函数在该点有极小值

        2.如果Hessian矩阵负定，函数在该点有极大值

        3.如果Hessian矩阵不定，则不是极值点（鞍点） （凸函数不存在鞍点）

    判定矩阵正定的常用方法有以下几种：

        1.矩阵的特征值全大于0。

        2.矩阵的所有顺序主子式都大于0。

        3.矩阵合同于单位矩阵I ？？？
    凸函数的非负线性组合是凸函数
    
