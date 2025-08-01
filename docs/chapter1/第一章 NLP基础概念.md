# 第一章 NLP 基础概念

自然语言处理（Natural Language Processing，NLP）作为人工智能领域的一个重要分支，旨在使计算机能够理解和处理人类语言，实现人机之间的自然交流。随着信息技术的飞速发展，文本数据已成为我们日常生活中不可或缺的一部分，NLP技术的进步为我们从海量文本中提取有用信息、理解语言的深层含义提供了强有力的工具。从早期的基于规则的方法，到后来的统计学习方法，再到当前深度学习技术的广泛应用，NLP领域经历了多次技术革新，文本表示作为NLP的核心技术之一，其研究和进步对于提升NLP系统的性能具有决定性的作用。

欢迎大家来到 NLP 基础概念的学习，本章节将为大家介绍 NLP 的基础概念，帮助大家更好地理解和回顾 NLP 的相关知识。

## 1.1 什么是 NLP

NLP 是 一种让计算机理解、解释和生成人类语言的技术。它是人工智能领域中一个极为活跃和重要的研究方向，其核心任务是通过计算机程序来模拟人类对语言的认知和使用过程。NLP 结合了计算机科学、人工智能、语言学和心理学等多个学科的知识和技术，旨在打破人类语言和计算机语言之间的障碍，实现无缝的交流与互动。

NLP技术使得计算机能够执行各种复杂的语言处理任务，如中文分词、子词切分、词性标注、文本分类、实体识别、关系抽取、文本摘要、机器翻译、自动问答等。这些任务不仅要求计算机能够识别和处理语言的表层结构，更重要的是可以理解语言背后的深层含义，包括语义、语境、情感和文化等方面的复杂因素。

随着深度学习等现代技术的发展，NLP 已经取得了显著的进步。通过训练大量的数据，深度学习模型能够学习到语言的复杂模式和结构，从而在多个 NLP 任务上取得了接近甚至超越人类水平的性能。然而，尽管如此，NLP 仍然面临着诸多挑战，如处理歧义性、理解抽象概念、处理隐喻和讽刺等。研究人员正致力于通过更加先进的算法、更大规模的数据集和更精细的语言模型来解决这些问题，以推动NLP技术不断发展。

## 1.2 NLP 发展历程

NLP 的发展历程是从早期的规则基础方法，到统计方法，再到现在的机器学习和深度学习方法的演变过程。每一次技术变革都极大地推动了 NLP 技术的发展，使其在机器翻译、情感分析、实体识别和文本摘要等任务上取得了显著成就。随着计算能力的不断增强和算法的不断优化，NLP的未来将更加光明，能够在更多领域发挥更加重要的作用。

### 早期探索（1940年代 - 1960年代）

NLP 的早期探索始于二战后，当时人们认识到将一种语言自动翻译为另一种语言的重要性。1950年，艾伦·图灵提出了图灵测试。

> 他说，如果一台机器可以通过使用打字机成为对话的一部分，并且能够完全模仿人类，没有明显的差异，那么机器可以被认为是能够思考的。

这是判断机器是否能够展现出与人类不可区分的智能行为的测试。这一时期，诺姆·乔姆斯基提出了生成语法理论，这对理解机器翻译的工作方式产生了重要影响。然而，这一时期的机器翻译系统非常简单，主要依赖字典查找和基本的词序规则来进行翻译，效果并不理想。

### 符号主义与统计方法（1970年代 - 1990年代）

1970年代以后，NLP 研究者开始探索新的领域，包括逻辑基础的范式和自然语言理解。这一时期，研究者分为符号主义（或规则基础）和统计方法两大阵营。符号主义研究者关注于形式语言和生成语法，而统计方法的研究者更加关注于统计和概率方法。1980年代，随着计算能力的提升和机器学习算法的引入，NLP领域出现了革命性的变化，统计模型开始取代复杂的“手写”规则。

### 机器学习与深度学习（2000年代至今）

2000年代以后，随着深度学习技术的发展，NLP 领域取得了显著的进步。深度学习模型如循环神经网络（Recurrent Neural Network，RNN）、长短时记忆网络（Long Short-Term Memory，LSTM）和注意力机制等技术被广泛应用于 NLP 任务中，取得了令人瞩目的成果。2013年，Word2Vec模型的提出开创了词向量表示的新时代，为NLP任务提供了更加有效的文本表示方法。2018年，BERT模型的问世引领了预训练语言模型的新浪潮，为NLP技术的发展带来了新的机遇和挑战。近年来，基于Transformer的模型，如GPT-3，通过训练巨大参数的模型，能够生成高质量的文本，甚至在某些情况下可以与人类写作相媲美。


## 1.3 NLP 任务

在NLP的广阔研究领域中，有几个核心任务构成了NLP领域的基础，它们涵盖了从文本的基本处理到复杂的语义理解和生成的各个方面。这些任务包括但不限于中文分词、子词切分、词性标注、文本分类、实体识别、关系抽取、文本摘要、机器翻译以及自动问答系统的开发。每一项任务都有其特定的挑战和应用场景，它们共同推动了语言技术的发展，为处理和分析日益增长的文本数据提供了强大的工具。

### 1.3.1 中文分词

中文分词（Chinese Word Segmentation, CWS）是 NLP 领域中的一个基础任务。在处理中文文本时，由于中文语言的特点，词与词之间没有像英文那样的明显分隔（如空格），所以无法直接通过空格来确定词的边界。因此，中文分词成为了中文文本处理的首要步骤，其目的是将连续的中文文本切分成有意义的词汇序列。

```
英文输入：The cat sits on the mat.
英文切割输出：[The | cat | sits | on | the | mat]
中文输入：今天天气真好，适合出去游玩.
中文切割输出：["今天", "天气", "真", "好", "，", "适合", "出去", "游玩", "。"]
```

正确的分词结果对于后续的词性标注、实体识别、句法分析等任务至关重要。如果分词不准确，将直接影响到整个文本处理流程的效果。

```
输入：雍和宫的荷花开的很好。

正确切割：雍和宫 | 的 | 荷花 | 开 | 的 | 很 | 好 | 。
错误切割 1：雍 | 和 | 宫的 | 荷花 | 开的 | 很好 | 。 （地名被拆散）
错误切割 2：雍和 | 宫 | 的荷 | 花开 | 的很 | 好。 （词汇边界混乱）
```

正确的分词结果对于后续的词性标注、实体识别、句法分析等任务至关重要。如果分词不准确，将直接影响到整个文本处理流程的效果。

### 1.3.2 子词切分

子词切分（Subword Segmentation）是 NLP 领域中的一种常见的文本预处理技术，旨在将词汇进一步分解为更小的单位，即子词。子词切分特别适用于处理词汇稀疏问题，即当遇到罕见词或未见过的新词时，能够通过已知的子词单位来理解或生成这些词汇。子词切分在处理那些拼写复杂、合成词多的语言（如德语）或者在预训练语言模型（如BERT、GPT系列）中尤为重要。

子词切分的方法有很多种，常见的有Byte Pair Encoding (BPE)、WordPiece、Unigram、SentencePiece等。这些方法的基本思想是将单词分解成更小的、频繁出现的片段，这些片段可以是单个字符、字符组合或者词根和词缀。

```
输入：unhappiness

不使用子词切分：整个单词作为一个单位，输出：“unhappiness”
使用子词切分（假设BPE算法）：单词被分割为：“un”、“happi”、“ness”
```

在这个例子中，通过子词切分，“unhappiness”这个词被分解成了三个部分：前缀“un”表示否定，“happi”是“happy”的词根变体，表示幸福，“ness”是名词后缀，表示状态。即使模型从未见过“unhappiness”这个完整的单词，它也可以通过这些已知的子词来理解其大致意思为“不幸福的状态”。

### 1.3.3 词性标注

词性标注（Part-of-Speech Tagging，POS Tagging）是 NLP 领域中的一项基础任务，它的目标是为文本中的每个单词分配一个词性标签，如名词、动词、形容词等。这个过程通常基于预先定义的词性标签集，如英语中的常见标签有名词（Noun，N）、动词（Verb，V）、形容词（Adjective，Adj）等。词性标注对于理解句子结构、进行句法分析、语义角色标注等高级NLP任务至关重要。通过词性标注，计算机可以更好地理解文本的含义，进而进行信息提取、情感分析、机器翻译等更复杂的处理。

假设我们有一个英文句子：She is playing the guitar in the park.

词性标注的结果如下：

- She (代词，Pronoun，PRP)
- is (动词，Verb，VBZ)
- playing (动词的现在分词，Verb，VBG)
- the (限定词，Determiner，DT)
- guitar (名词，Noun，NN)
- in (介词，Preposition，IN)
- the (限定词，Determiner，DT)
- park (名词，Noun，NN)
- . (标点，Punctuation，.)

词性标注通常依赖于机器学习模型，如隐马尔可夫模型（Hidden Markov Model，HMM）、条件随机场（Conditional Random Field，CRF）或者基于深度学习的循环神经网络 RNN 和长短时记忆网络 LSTM 等。这些模型通过学习大量的标注数据来预测新句子中每个单词的词性。

### 1.3.4 文本分类

文本分类（Text Classification）是 NLP 领域的一项核心任务，涉及到将给定的文本自动分配到一个或多个预定义的类别中。这项技术广泛应用于各种场景，包括但不限于情感分析、垃圾邮件检测、新闻分类、主题识别等。文本分类的关键在于理解文本的含义和上下文，并基于此将文本映射到特定的类别。

假设有一个文本分类任务，目的是将新闻文章分类为“体育”、“政治”或“科技”三个类别之一。

```
文本：“NBA季后赛将于下周开始，湖人和勇士将在首轮对决。”
类别：“体育”

文本：“美国总统宣布将提高关税，引发国际贸易争端。”
类别：“政治”

文本：“苹果公司发布了新款 Macbook，配备了最新的m3芯片。”
类别：“科技”
```

文本分类任务的成功关键在于选择合适的特征表示和分类算法，以及拥有高质量的训练数据。随着深度学习技术的发展，使用神经网络进行文本分类已经成为一种趋势，它们能够捕捉到文本数据中的复杂模式和语义信息，从而在许多任务中取得了显著的性能提升。

### 1.3.5 实体识别

实体识别（Named Entity Recognition, NER），也称为命名实体识别，是 NLP 领域的一个关键任务，旨在自动识别文本中具有特定意义的实体，并将它们分类为预定义的类别，如人名、地点、组织、日期、时间等。实体识别任务对于信息提取、知识图谱构建、问答系统、内容推荐等应用很重要，它能够帮助系统理解文本中的关键元素及其属性。

假设有一个实体识别任务，目的是从文本中识别出人名、地名和组织名等实体。

```
输入：李雷和韩梅梅是北京市海淀区的居民，他们计划在2024年4月7日去上海旅行。

输出：[("李雷", "人名"), ("韩梅梅", "人名"), ("北京市海淀区", "地名"), ("2024年4月7日", "日期"), ("上海", "地名")]
```

通过实体识别任务，我们不仅能识别出文本中的实体，还能了解它们的类别，为深入理解文本内容和上下文提供了重要信息。随着NLP技术的发展，实体识别的精度和效率不断提高，可以为各种NLP应用提供强大的支持。

### 1.3.6 关系抽取

关系抽取（Relation Extraction）是 NLP 领域中的一项关键任务，它的目标是从文本中识别实体之间的语义关系。这些关系可以是因果关系、拥有关系、亲属关系、地理位置关系等，关系抽取对于理解文本内容、构建知识图谱、提升机器理解语言的能力等方面具有重要意义。

假设我们有以下句子：

```
输入：比尔·盖茨是微软公司的创始人。

输出：[("比尔·盖茨", "创始人", "微软公司")]
```

在这个例子中，关系抽取任务的目标是从文本中识别出“比尔·盖茨”和“微软公司”之间的“创始人”关系。通过关系抽取，我们可以从文本中提取出有用的信息，帮助计算机更好地理解文本内容，为后续的知识图谱构建、问答系统等任务提供支持。

### 1.3.7 文本摘要

文本摘要（Text Summarization）是 NLP 中的一个重要任务，目的是生成一段简洁准确的摘要，来概括原文的主要内容。根据生成方式的不同，文本摘要可以分为两大类：抽取式摘要（Extractive Summarization）和生成式摘要（Abstractive Summarization）。

- 抽取式摘要：抽取式摘要通过直接从原文中选取关键句子或短语来组成摘要。优点是摘要中的信息完全来自原文，因此准确性较高。然而，由于仅仅是原文中句子的拼接，有时候生成的摘要可能不够流畅。
- 生成式摘要：与抽取式摘要不同，生成式摘要不仅涉及选择文本片段，还需要对这些片段进行重新组织和改写，并生成新的内容。生成式摘要更具挑战性，因为它需要理解文本的深层含义，并能够以新的方式表达相同的信息。生成式摘要通常需要更复杂的模型，如基于注意力机制的序列到序列模型（Seq2Seq）。

假设我们有以下新闻报道：

```
2021年5月22日，国家航天局宣布，我国自主研发的火星探测器“天问一号”成功在火星表面着陆。此次任务的成功，标志着我国在深空探测领域迈出了重要一步。“天问一号”搭载了多种科学仪器，将在火星表面进行为期90个火星日的科学探测工作，旨在研究火星地质结构、气候条件以及寻找生命存在的可能性。
```

抽取式摘要：

```
我国自主研发的火星探测器“天问一号”成功在火星表面着陆，标志着我国在深空探测领域迈出了重要一步。
```

生成式摘要：

```
“天问一号”探测器成功实现火星着陆，代表我国在宇宙探索中取得重大进展。
```

文本摘要任务在信息检索、新闻推送、报告生成等领域有着广泛的应用。通过自动摘要，用户可以快速获取文本的核心信息，节省阅读时间，提高信息处理效率。

### 1.3.8 机器翻译

机器翻译（Machine Translation, MT）是 NLP 领域的一项核心任务，指使用计算机程序将一种自然语言（源语言）自动翻译成另一种自然语言（目标语言）的过程。机器翻译不仅涉及到词汇的直接转换，更重要的是要准确传达源语言文本的语义、风格和文化背景等，使得翻译结果在目标语言中自然、准确、流畅，以便跨越语言障碍，促进不同语言使用者之间的交流与理解。

假设我们有一句中文：“今天天气很好。”，我们想要将其翻译成英文。

```
源语言：今天天气很好。

目标语言：The weather is very nice today.
```

在这个简单的例子中，机器翻译能够准确地将中文句子转换成英文，保持了原句的意义和结构。然而，在处理更长、更复杂的文本时，机器翻译面临的挑战也会相应增加。为了提高机器翻译的质量，研究者不断探索新的方法和技术，如基于神经网络的Seq2Seq模型、Transformer模型等，这些模型能够学习到源语言和目标语言之间的复杂映射关系，从而实现更加准确和流畅的翻译。

### 1.3.9 自动问答

自动问答（Automatic Question Answering, QA）是 NLP 领域中的一个高级任务，旨在使计算机能够理解自然语言提出的问题，并根据给定的数据源自动提供准确的答案。自动问答任务模拟了人类理解和回答问题的能力，涵盖了从简单的事实查询到复杂的推理和解释。自动问答系统的构建涉及多个NLP子任务，如信息检索、文本理解、知识表示和推理等。

自动问答大致可分为三类：检索式问答（Retrieval-based QA）、知识库问答（Knowledge-based QA）和社区问答（Community-based QA）。检索式问答通过搜索引擎等方式从大量文本中检索答案；知识库问答通过结构化的知识库来回答问题；社区问答则依赖于用户生成的问答数据，如问答社区、论坛等。

自动问答系统的开发和优化是一个持续的过程，随着技术的进步和算法的改进，这些系统在准确性、理解能力和应用范围上都有显著的提升。通过结合不同类型的数据源和技术方法，自动问答系统正变得越来越智能，越来越能够处理复杂和多样化的问题。

## 1.4 文本表示的发展历程

文本表示的目的是将人类语言的自然形式转化为计算机可以处理的形式，也就是将文本数据数字化，使计算机能够对文本进行有效的分析和处理。文本表示是 NLP 领域中的一项基础性和必要性工作，它直接影响甚至决定着 NLP 系统的质量和性能。

在 NLP 中，文本表示涉及到将文本中的语言单位（如字、词、短语、句子等）以及它们之间的关系和结构信息转换为计算机能够理解和操作的形式，例如向量、矩阵或其他数据结构。这样的表示不仅需要保留足够的语义信息，以便于后续的 NLP 任务，如文本分类、情感分析、机器翻译等，还需要考虑计算效率和存储效率。

文本表示的发展历程经历了多个阶段，从早期的基于规则的方法，到统计学习方法，再到当前的深度学习技术，文本表示技术不断演进，为 NLP 的发展提供了强大的支持。

### 1.4.1 词向量

向量空间模型（Vector Space Model, VSM）是 NLP 领域中一个基础且强大的文本表示方法，最早由哈佛大学Salton提出。向量空间模型通过将文本（包括单词、句子、段落或整个文档）转换为高维空间中的向量来实现文本的数学化表示。在这个模型中，每个维度代表一个特征项（例如，字、词、词组或短语），而向量中的每个元素值代表该特征项在文本中的权重，这种权重通过特定的计算公式（如词频TF、逆文档频率TF-IDF等）来确定，反映了特征项在文本中的重要程度。

向量空间模型的应用极其广泛，包括但不限于文本相似度计算、文本分类、信息检索等自然语言处理任务。它将复杂的文本数据转换为易于计算和分析的数学形式，使得文本的相似度计算和模式识别成为可能。此外，通过矩阵运算如特征值计算、奇异值分解（singular value decomposition, SVD）等方法，可以优化文本向量表示，进一步提升处理效率和效果。

然而，向量空间模型也存在很多问题。其中最主要的是数据稀疏性和维数灾难问题，因为特征项数量庞大导致向量维度极高，同时多数元素值为零。此外，由于模型基于特征项之间的独立性假设，忽略了文本中的结构信息，如词序和上下文信息，限制了模型的表现力。特征项的选择和权重计算方法的不足也是向量空间模型需要解决的问题。

VSM 方法词向量：

```python
# "雍和宫的荷花很美"
# 词汇表大小：16384，句子包含词汇：["雍和宫", "的", "荷花", "很", "美"] = 5个词

vector = [0, 0, ..., 1, 0, ..., 1, 0, ..., 1, 0, ..., 1, 0, ..., 1, 0, ...]
#                    ↑          ↑          ↑          ↑          ↑
#      16384维中只有5个位置为1，其余16379个位置为0
# 实际有效维度：仅5维（非零维度）
# 稀疏率：(16384-5)/16384 ≈ 99.97%
```
> 词汇表是一个包含所有可能出现的词语的集合。在向量空间模型中，每个词对应词汇表中的一个位置，通过这种方式可以将词语转换为向量表示。例如，如果词汇表大小为 16384 ，那么每个词都会被表示为一个 16384 维的向量，其中只有该词对应的位置为 1，其他位置都为 0。

为了解决这些问题，研究者们对向量空间模型的研究主要集中在两个方面：一是改进特征表示方法，如借助图方法、主题方法等进行关键词抽取；二是改进和优化特征项权重的计算方法，可以在现有方法的基础上进行融合计算或提出新的计算方法.

### 1.4.2 语言模型

N-gram 模型是 NLP 领域中一种基于统计的语言模型，广泛应用于语音识别、手写识别、拼写纠错、机器翻译和搜索引擎等众多任务。N-gram模型的核心思想是基于马尔可夫假设，即一个词的出现概率仅依赖于它前面的N-1个词。这里的N代表连续出现单词的数量，可以是任意正整数。例如，当N=1时，模型称为unigram，仅考虑单个词的概率；当N=2时，称为bigram，考虑前一个词来估计当前词的概率；当N=3时，称为trigram，考虑前两个词来估计第三个词的概率，以此类推N-gram。

N-gram模型通过条件概率链式规则来估计整个句子的概率。具体而言，对于给定的一个句子，模型会计算每个N-gram出现的条件概率，并将这些概率相乘以得到整个句子的概率。例如，对于句子“The quick brown fox”，作为trigram模型，我们会计算 $P("brown" | "The", "quick")$、$P("fox" | "quick", "brown")$等概率，并将它们相乘。

N-gram的优点是实现简单、容易理解，在许多任务中效果不错。但当N较大时，会出现数据稀疏性问题。模型的参数空间会急剧增大，相同的N-gram序列出现的概率变得非常低，导致模型无法有效学习，模型泛化能力下降。此外，N-gram模型忽略了词之间的范围依赖关系，无法捕捉到句子中的复杂结构和语义信息。

尽管存在局限性，N-gram模型由于其简单性和实用性，在许多 NLP 任务中仍然被广泛使用。在某些应用中，结合N-gram模型和其他技术（如深度学习模型）可以获得更好的性能。

### 1.4.3 Word2Vec

Word2Vec是一种流行的词嵌入（Word Embedding）技术，由Tomas Mikolov等人在2013年提出。它是一种基于神经网络NNLM的语言模型，旨在通过学习词与词之间的上下文关系来生成词的密集向量表示。Word2Vec的核心思想是利用词在文本中的上下文信息来捕捉词之间的语义关系，从而使得语义相似或相关的词在向量空间中距离较近。

Word2Vec模型主要有两种架构：连续词袋模型CBOW(Continuous Bag of Words)是根据目标词上下文中的词对应的词向量, 计算并输出目标词的向量表示；Skip-Gram模型与CBOW模型相反, 是利用目标词的向量表示计算上下文中的词向量. 实践验证CBOW适用于小型数据集, 而Skip-Gram在大型语料中表现更好。

相比于传统的高维稀疏表示（如One-Hot编码），Word2Vec生成的是低维（通常几百维）的密集向量，有助于减少计算复杂度和存储需求。Word2Vec模型能够捕捉到词与词之间的语义关系，比如”国王“和“王后”在向量空间中的位置会比较接近，因为在大量文本中，它们通常会出现在相似的上下文中。Word2Vec模型也可以很好的泛化到未见过的词，因为它是基于上下文信息学习的，而不是基于词典。但由于CBOW/Skip-Gram模型是基于局部上下文的，无法捕捉到长距离的依赖关系，缺乏整体的词与词之间的关系，因此在一些复杂的语义任务上表现不佳。

### 1.4.4 ELMo

ELMo（Embeddings from Language Models）实现了一词多义、静态词向量到动态词向量的跨越式转变。首先在大型语料库上训练语言模型，得到词向量模型，然后在特定任务上对模型进行微调，得到更适合该任务的词向量，ELMo首次将预训练思想引入到词向量的生成中，使用双向LSTM结构，能够捕捉到词汇的上下文信息，生成更加丰富和准确的词向量表示。

ELMo采用典型的两阶段过程: 第1个阶段是利用语言模型进行预训练; 第2个阶段是在做特定任务时, 从预训练网络中提取对应单词的词向量作为新特征补充到下游任务中。基于RNN的LSTM模型训练时间长, 特征提取是ELMo模型优化和提升的关键。

ELMo模型的主要优势在于其能够捕捉到词汇的多义性和上下文信息，生成的词向量更加丰富和准确，适用于多种 NLP 任务。然而，ELMo模型也存在一些问题，如模型复杂度高、训练时间长、计算资源消耗大等。

## 参考文献

[1] Tomas Mikolov, Ilya Sutskever, Kai Chen, Greg Corrado, Jeffrey Dean. (2013). *Distributed Representations of Words and Phrases and their Compositionality.* arXiv preprint arXiv:1310.4546.

[2] Jacob Devlin, Ming-Wei Chang, Kenton Lee, Kristina Toutanova. (2019). BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding. arXiv preprint arXiv:1810.04805.

[3] Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N. Gomez, Lukasz Kaiser, Illia Polosukhin. (2023). *Attention Is All You Need.* arXiv preprint arXiv:1706.03762.

[4] Malek Hajjem, Chiraz Latiri. (2017). *Combining IR and LDA Topic Modeling for Filtering Microblogs.* Procedia Computer Science, 112, 761–770. https://doi.org/10.1016/j.procs.2017.08.166.

[5] Matthew E. Peters, Mark Neumann, Mohit Iyyer, Matt Gardner, Christopher Clark, Kenton Lee, Luke Zettlemoyer. (2018). *Deep contextualized word representations.* arXiv preprint arXiv:1802.05365.

[6] Salton, G., Wong, A., Yang, C. S. (1975). *A vector space model for automatic indexing.* Communications of the ACM, 18(11), 613–620. https://doi.org/10.1145/361219.361220.

[7] 赵京胜,宋梦雪,高祥,等.自然语言处理中的文本表示研究[J].软件学报,2022,33(01):102-128.DOI:10.13328/j.cnki.jos.006304.

[8] 中文信息处理发展报告（2016）前言[C]//中文信息处理发展报告（2016）.中国中文信息学会;,2016:2-3.DOI:10.26914/c.cnkihy.2016.003326.

