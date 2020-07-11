# **GRAPH CONVOLUTIONAL NETWORKS**

原文地址：[GRAPH CONVOLUTIONAL NETWORKS](http://tkipf.github.io/graph-convolutional-networks/)

## 概述

许多重要的现实世界数据集都以图或网络的形式出现：社交网络，知识图，蛋白质相互作用网络，万维网等（仅举几例）。
然而，直到最近，很少有人将注意力集中在将神经网络模型推广到此类结构化数据集上。
在过去的几年中，许多论文重新探讨了将神经网络推广到任意结构图上的问题（Bruna等人，ICLR 2014； Henaff等人，2015； Duvenaud等人，NIPS 2015；以及 Li等人，ICLR 2016； Defferrard等人，NIPS 2016； Kipf＆Welling，ICLR 2017），其中一些人现在在以前被基于内核的方法，图 基于正则化技术等。
在本文中，我将简要概述该领域的最新发展，并指出各种方法的优点和缺点。
这里的讨论主要集中在最近的两篇论文上：Kipf＆Welling（ICLR 2017），图卷积网络的半监督分类（免责声明：我是第一作者）Defferrard等。
（NIPS 2016），具有快速局部频谱滤波的图卷积神经网络，以及Ferenc Huszar的评论/讨论文章：图卷积有多强大？
讨论了这类模型的一些局限性。
我在这里（本文结尾处）对Ferenc的评论发表了简短评论。