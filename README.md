# Business-Analytics-Project
这是我们于2019年12月在哥大的IEOR4650 商业分析 的课程上做的团队项目，整个项目由我和组员Jiani Lu, Chenfei Hou, Yuxing Chen, Jie Chen共同协作完成。此项目旨在帮助人气不高的和新加入的Airbnb房东提高他们的人气，这样既使得那些房东的生意兴隆，有能使得Airbnb公司从更红火的市场中赚取更多的收益。此项目是基于纽约市Airbnb的数据做的分析，而我在此项目中主要负责推荐引擎的设计和实现。

我们利用 Unsupervised KNN 建立一个推荐引擎。该引擎会向用户推荐跟他们浏览过的房源类似的低人气房源和新房源从而提高低人气房源和新房源的曝光率。（我们认为用户浏览过的房源是他们所感兴趣的，所以向他们推荐类似的。）当然，被推荐给用户的房源在质量上要过关，所以我们仅过滤出评分高于特定阈值的房源来做推荐。总之，推荐引擎是帮助那些酒香巷子深的房源（人气少但评分不低）和新房源来提高它们的曝光率。引擎使用者也可以通过设定参数值来灵活调整推荐给用户的高人气房源和低人气房源的比例。（总是给用户推荐低人气的也不太好，高人气和低人气的组合起来推荐为佳。）

我们也尝试创建预测模型来基于给定的条件预测一个房源的评分。一个新房东可以利用该模型来对自己房源的口碑有个大体的预估。与此同时我们也通过模型了解了各特征对评分的影响（是正是负？是大是小？）这样新房东可以大体判断怎样使自己的房源更受欢迎，苦于低评分的房东也可以知道如何提高自己房源的质量，从而赢得好口碑和被推荐引擎推荐的机会。在这上面我们实验了线性回归，随机森林，KNN和神经网络四种方法。同时我们也利用Weibull Timing Model来帮助新房东预测他们的第一笔生意要大概多久，这期间的时间如何受房源各特征的影响。

此项目的展示短视频在此链接 https://www.bilibili.com/video/BV1U54y1X7Le
