# CNSegmenter

##模型
本项目使用了隐马尔科夫模型分词，使用pku的语料库进行训练。
马尔可夫模型（Markov Model）是一种统计模型，广泛应用在语音识别，词性自动标注，音字转换，概率文法等各个自然语言处理等应用领域。经过长期发展，尤其是在语音识别中的成功应用，使它成为一种通用的统计工具。公式：argmax C P(O|C)P(C)，其中：P(C1，C2，C3….Ci) = P(C1)P(C2|C1)P(C3|C2)…P(Ci|Ci-1)，我们称P(Cj|Ci)为i到j的状态转移概率，P(O|C) = P(O1|C) * P(O2|C)……P(Oi|C) = P(O1|C1) * P(O2|C2)……P(Oi|Ci)，P(O|C)是观察值数据的概率，都可以通过在大量语料中使用统计的方法求得。

##使用
运行 SegmenterTest 的testSegment()方法即可分词。

##注意
由于语料库有限，所以分词的准确度较低，供学习使用。

  更多内容：[PHY的博客](http://pp1230.github.io/)
