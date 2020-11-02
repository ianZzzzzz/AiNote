# tf.Graph()
    tf.Graph()表示实例化一个用于tensorflow计算和表示用的数据流图，不负责运行计算。在代码中添加的操作和数据都是画在纸上的画，而图就是呈现这些画的纸。我们可以利用很多线程生成很多张图，但是默认图就只有一张。
   tf中可以定义多个计算图，不同计算图上的张量和运算是相互独立的，不会共享。计算图可以用来隔离张量和计算，同时提供了管理张量和计算的机制。  
        # 定义两个计算图
        g1 = tf.Graph()
        g2 = tf.Graph()

        # 在g1中定义张量和操作
        with g1.as_default():
        a = tf.constant([1.0, 1.0])
        b = tf.constant([1.0, 1.0])
        result1 = a + b

        # 在g2中定义张量和操作
        with g2.as_default():
        a = tf.constant([2.0, 2.0])
        b = tf.constant([2.0, 2.0])
        result2 = a + b

        # 创建会话
        with tf.Session(graph=g1) as sess:
        out = sess.run(result1)
        print(out)

        with tf.Session(graph=g2) as sess:
        out = sess.run(result2)
        print(out)

        with tf.Session(graph=tf.get_default_graph()) as sess:
        out = sess.run(result)
        print(out)

        返回：
        [2.0, 2.0]
        [4.0, 4.0]
# tf.nn.embedding_lookup(tensor,index)
     选取一个张量里面索引对应的元素