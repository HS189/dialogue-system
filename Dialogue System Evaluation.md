### paper

+ How NOT To Evaluate Your Dialogue System: An Empirical Study of Unsupervised Evaluation Metrics for Dialogue Response Generation, Chia-Wei Liu, Ryan Lowe, Iulian V. Serban, Michael Noseworthy, Laurent Charlin, Joelle Pineau, EMNLP 2016 [arxiv](https://arxiv.org/abs/1603.08023) 



How to create a proper test set?/What's the principle to create test set?

评估指标：平均每轮对话时长...

+ task-orient

  1. 单场景

     多轮

     轮数越多，说明人机对话越流畅，用户聊天意愿越强。

  2. 跨场景

     场景切换

     轮数越少，说明解决问题所需时间越短。

+ chatbot

  1. 多样性回答

  2. 一致性回答

     机器人信息及用户信息等

  3. 兜底回答

     语料无法覆盖的场景


+ 测试工具

  积累的测试数据-learning to rank

+ Error Analysis

  1. 库中无相似句（相似度低于设定的阈值）
  2. 模型精度较低
  3. 