对于任意给定的精度，任意连续的多元函数都能通过有限个节点多层的神经网络来表示。但是表示效率（节点和层数越少越好）就取决于具体问题和具体的激活函数。

比如说你要逼近的真实函数是3x^2+2y^2+5xy。你的输入层是一个x一个y。然后你第一层有7个节点，其中有4个节点每个节点的输出值等于输入值加权和的平方。另外两个节点输出量等于输入量的加权和，最后还有一个节点，其输出量等于一个常数。
第二层的输出量等于输入量。其输入量等于第一层7个节点的加权和。于是你就有了一个计算网络，能拟合任意二阶多项式函数。

“激活函数是用来引入非线性的”，这个说法是不完全正确的。它确实引入了非线性，但是并不是每一种形式的非线性函数都能作为激活函数。最基本的要求是这个函数族得在连续函数空间稠密。其次高效的激活函数(可能还)需要满足KST的要求，而sigmoid恰好做到了。至于其他计算方面的优点，那取决于怎么算权重。比如基于梯度的计算方法当然需要容易计算导数的激活函数。

作者：黑怕
链接：https://www.zhihu.com/question/24259872/answer/623699200
来源：知乎
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。