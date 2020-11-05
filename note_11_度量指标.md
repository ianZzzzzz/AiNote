# 常见度量指标
    accuracy
    precision
    recall
        展示模型的覆盖能力，假设100个正样本，模型预测到了40个，召回率就为40%
    F1-score
        综合考虑了precision和recall，分为Marco和micro两种F1-score。在multi-class classification的情况下，如果非要用一个综合考量的metric的话，macro-average（宏平均） 会比 micro-average（微平均） 好一些哦，因为macro会受minority class影响更大，也就是说更能体现在small class上的performance。


    ROC-AUC
    PR-AUC