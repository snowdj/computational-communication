#序言
伴随着**大数据时代**的到来和人类科学研究的发展，计算社会科学成为了二十一世纪科学发展的重要方向。其中，可计算思维、工具与方法开始在传播学科当中发挥越来越重要的作用。基于此，计算传播学应运而生。计算传播学是计算社会科学的重要分支，它主要关注人类传播行为的可计算性基础，以传播网络分析、传播文本挖掘、数据科学等为主要分析工具。（以非介入方式）大规模地收集并分析人类传播行为数据、挖掘人类传播行为背后的模式和法则，分析模式背后的生成机制与基本原理。可以被广泛地应用于数据新闻和计算广告等场景。注重编程训练、数学建模、可计算思维。

为了更好地界定计算传播的理论框架和实际应用、同时也是为了学习和应用计算传播学研究方法，我酝酿开设了《计算传播学》工作坊课程。这门课的学生主要是南京大学新闻传播学院2014级的研究生。而本书主要致力于总结在这个过程当中关于计算传播学的思考。

围绕着计算传播学这一核心概念，本书将主要分为三部分，第一部分介绍计算传播学的理论起源，包括“计算”和“传播”各自的含义及其关联，提出计算传播学的基本理论架构；第二部分，则主要介绍可计算思维在传播学研究和实务当中的应用；第三部分则主要总结既有的理论与应用。

本书是采用Gitbook撰写并发布的，因此需要感谢Gitbook团队和Github网站。Gitbook非常好地支持了markdown写作，包括数学公式的展现（例如$$E = MC^2$$）和编程代码的显现：


```Python
from scholarNetwork import scholarNetwork
import matplotlib.pyplot as plt
import networkx as nx

## Set the seed of crawler
seed = 'https://scholar.google.nl/citations?user=nNdt_G8AAAAJ&hl=en&oe=ASCII'

## Nodes number. Start with a small one.
Nmax = 21

## Get the graph g
g = scholarNetwork.getGraph(seed, Nmax)

## plot the network
pos=nx.spring_layout(g) #setup the layout

nx.draw(g, pos, node_shape = 'o',
        edge_color = 'gray', width = 0.5,
        with_labels = True, arrows = True)
plt.show()
```





王成军 

2015年3月5日于南京枫桥雅筑




