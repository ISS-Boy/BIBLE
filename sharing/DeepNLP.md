# DeepNLP

## Word embedding & Language Model

>  how to get a word embedding?

- 无监督学习
  - NNLM,RNNLM: 训练语言模型为任务，word embedding作为副产品
  - word2Vec，Glove...:网络结构是为了训练去得到word embedding而设计的

## Pre-train & transfer learning

> 有一个好的word embedding,我们总可以知道"milk" 接近“water”，而不是“shoes”
>
> how to use word embedding?

- A two-stage way: 以language model为task做pre-train，然后下游Task使用pre-train得到的embedding层or模型网络参数(基于Transformer的模型)
  - Frozen:embedding层的网络参数固定
  - fine-tune：embedding层的网络参数在back-propagate的时候一起调整

## References
- About word embedding:
  - [word embedding](https://blog.csdn.net/scotfield_msn/article/details/69075227)
  - [Word embedding and DL](http://licstar.net/archives/328#s20)

- About pre-train :
  - [从Word Embedding到Bert模型—自然语言处理中的预训练技术发展史](https://zhuanlan.zhihu.com/p/49271699)
  - [NLP迁移学习](https://zhuanlan.zhihu.com/p/42618178)

- Papers:

  .....