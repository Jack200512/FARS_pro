# FARS_pro
A beginner-level RAG question answering project exploring retrieval and generation techniques, including hybrid search and Flan-T5 models, with focus on tuning parameters to improve performance under limited GPU resources.
---
# 基于SQuAD数据集的RAG问答系统优化实验

本项目基于检索增强生成（RAG）框架，探索在有限资源条件下，通过优化检索策略及参数调优等方式提升问答性能的实验。项目重点分析了不同检索方法（如FAISS、纯向量内积、BM25+混合检索）、生成模型（Flan-T5系列）、以及生成解码策略（Beam Search宽度、最大生成长度等）对最终准确率（Exact Match）和F1分数的影响。

## 项目简介
该实验主要包括以下内容：
- 检索模块的多种实现与优化：包括放弃FAISS IVF索引，采用纯向量内积计算，并结合BM25与混合检索策略实现更优上下文召回。
- 生成模块的参数调优：探索Beam宽度、最大生成tokens等解码参数对结果的影响。
- 参数调优流程：通过系统化的参数扫描和分析，确定各阶段最佳配置，实现性能提升。
- 实验评估与性能分析：记录Exact Match与F1分数，结合推断时间与资源限制进行综合考量。

## 项目内容概览
- DataSet：SQuAD数据集
- fars-pro.ipynb：代码实现与关键输出结果
- evaluation.py：官方评估脚本
- 基于SQuAD数据集的RAG问答系统优化实验_实验报告.md：详细实验报告
---
完整的实验过程、参数设置、性能表现以及调参分析均收录在[基于SQuAD数据集的RAG问答系统优化实验_实验报告.md]文件中，建议阅读以进一步理解本项目的相关细节。
