https://github.com/qhduan/ConversationalRobotDesign



#### Watson

https://www.ibm.com/developerworks/cn/cognitive/library/cc-cognitive-media-telco-4-trs/index.html

???

#### OLAMI【欧拉密】- 威盛电子

https://cn.olami.ai/wiki/?mp=overview&content=overview.html<br>一种在智能对话中实现上下文功能的方法 https://blog.csdn.net/speeds3/article/details/78302774
接口文档详细，比较有参考意义！  
OLAMI 语法描述语言（OLAMI Syntax Language，简称：OSL）是 OLAMI 平台针对自然语言处理所发展出的独特语法描述语言，自然语言语义互动（Natural Language Interaction, 简称：NLI）管理系统采用 OSL 取代复杂的编码编程，使用简单、容易学习而且灵活有弹性。  
OSL 易于学习的特性，让毫无工程背景的人员也能轻易上手，能替您的智能语音/语言交互产品开发后的维护工作，以及尤其对于智能对话的能力扩展变得非常容易，有效降低产品研发与维护的时程及成本。

上下文处理：<br>https://cn.olami.ai/wiki/?mp=nli&content=nli_context_processing.html<br>[一种在智能对话中实现上下文的方法](https://www.cnblogs.com/stdioh/p/7727399.html)



#### 灵云机器人 - 捷通华声 - 政务

https://www.aicloud.com/dev/index/index

技能体验

https://www.aicloud.com/dev/ability/index.html?key=nlu#ability-experience

https://www.aicloud.com/home/product/subpage?key=nicss#demo-experience



#### 图灵机器人 - 儿童教育机器人

refer:<br>知识图谱在问答系统中的应用和挑战-2016-知识图谱会议

闲聊-对话体验

http://uzoo.cn/100001

技能-对话体验

http://biz.turingos.cn/chat

文档中心

http://docs.turingos.cn/

http://docs.turingos.cn/script/intro_doc/

帮助中心

https://www.kancloud.cn/turing/www-tuling123-com/718218

![规则系统](https://github.com/bifeng/dialogue-system/raw/master/image/turing_rule_based.png)

![挑战](https://github.com/bifeng/dialogue-system/raw/master/image/turing_challenge.png)



#### 百度机器人

https://baidu.com/

#### 云问机器人

https://v3.faqrobot.org/register.html



#### 小i机器人 - iBotCloud

#### 文因互联 - 



#### 云知声 - 车载

https://github.com/oraleval

https://github.com/oraleval/Grammar-rules

[JSGF](https://en.wikipedia.org/wiki/JSGF)

**JSGF** stands for **Java Speech Grammar Format** or the **JSpeech Grammar Format** (in a W3C Note). Developed by [Sun Microsystems](https://en.wikipedia.org/wiki/Sun_Microsystems), it is a textual representation of [grammars](https://en.wikipedia.org/wiki/Formal_grammar) for use in [speech recognition](https://en.wikipedia.org/wiki/Speech_recognition) for technologies like [XHTML+Voice](https://en.wikipedia.org/wiki/XHTML%2BVoice). JSGF adopts the style and conventions of the [Java programming language](https://en.wikipedia.org/wiki/Java_(programming_language)) in addition to use of traditional grammar notations.

The [Speech Recognition Grammar Specification](https://en.wikipedia.org/wiki/SRGS) was derived from this specification.



#### 思必驰 - 

refer:<br>[启发式对话中的知识管理](https://blog.csdn.net/dQCFKyQDXYm3F8rB0/article/details/81571615) [pdf](百度网盘-NLP专场：启发式对话中的知识管理（思必驰）.pdf)

![规则系统](https://github.com/bifeng/dialogue-system/raw/master/image/rule_system_sbc.png)

![对话管理](https://github.com/bifeng/dialogue-system/raw/master/image/dialogue_management_sbc.png)



#### 科大讯飞





#### 小爱同学 - 小米





#### 蚂蚁金服-MISA（Machine Intelligence Service Assistant）

refer:<br><https://www.jiqizhixin.com/articles/interview-with-Ant-Financial-MISA>

MISA 的主要模块有猜问题、问题识别、反问交互三个。「猜问题」是蚂蚁金服在客服领域的首创，是一个利用用户可能与本次致电相关的信息，基于深度学习算法框架构建的问题识别模型。「问题识别」是根据用户的描述定位他可能遇到的问题。「反问交互」是在用户给出的信息不全时，利用「要素拆解和补全」的方式帮助问题识别模块圈定范围，降低问题识别的难度，以反问的形式与用户进行交互。

##### 猜问题

input suggestion - question recommendation

CTR

##### 问题识别

将输入分为因子、轨迹、文本三类。因子是由业务方定义的、具有明确含义的特征，例如：过去 24 小时是否有还款行为、过去 24 小时是否发生过转账行为等。因子大约有数百个。轨迹是用户最近的 120 个「行为」组成的时间序列，其中一个行为指对远程服务器发生一次请求。行为的种类超过一万种。文本是用户的描述以文本形式表达；在「猜问题」环节，文本指用户的历史描述，在正常的「问题识别」环节，文本即把本次电话里用户对问题的语音描述转换成文本。文本是一个长度各不相同，甚至可能空缺的输入。

![模型融合](https://github.com/bifeng/dialogue-system/raw/master/image/intent_tree_et.png)

![匹配模型融合](https://github.com/bifeng/dialogue-system/raw/master/image/match_model.png)

![匹配模型架构](https://github.com/bifeng/dialogue-system/raw/master/image/model_architect.png)

分类模型返回不同类别的可能性打分，意图树可能只返回某一个最可能的类别。

##### 反问交互

![多轮反问](https://github.com/bifeng/dialogue-system/raw/master/image/multi_turn.png)

用户的大多数问题都能够以「业务、框架、类型」三要素方式进行拆分。例如「花呗不能还款」，「花呗」就是涉及的业务，问题的核心动词「还款」就是框架，「失败」是导致用户提问的诉求类型。有超过一千个用户问题都可以被拆解成三要素的形式，其中包括一百多类业务、不到一百类框架和不超过十种问题类型。

三要素拆分方式的方式能够帮助快速缩小识别范围。用户在描述中，可能不能一次把三要素都描述清楚，但是如果给出了某部分要素，比如用户说「我要还款」，就给出了框架「还款」和类型「如何」，这时我们就可以就缺失的「业务」要素进行反问，比如，「您是要进行花呗还款、借呗还款还是信用卡还款？」

从技术的角度上来讲，我们在构建了**语义要素库**之后，是可以实现 zero-shot 的问题识别的。即，不需要见到特定的要素组合的训练样本，只要在其他训练样本中见过单独的要素在其他场景下出现，一样可以识别这个要素组合，对应到相应问题。

另外，我们也构建了多任务学习的框架。三要素识别任务的目标是非常类似的，都可以看做是多分类问题。多任务学习让不同任务间的数据可以共享。虽然每一个单独的任务都有足够的数据，但是不同任务间目标会让特征提取各有侧重，提高模型效果。





#### 小薇、茉莉

https://github.com/b3log/xiaov

http://www.itpk.cn/



| 代码         | 描述               | 示例                             |
| ------------ | ------------------ | -------------------------------- |
| **[date]**   | 当前的日期和时间   | 现在的时间是[date]。             |
| **[cqname]** | 机器人的名字       | 我叫[cqname]，你叫什么啊！       |
| **[father]** | 机器人的爸爸       | 我的爸爸是[father]。             |
| **[mother]** | 机器人的妈妈       | 我的妈妈是[mother]。             |
| **[name]**   | 机器人对用户的称呼 | [name]你好，很高兴认识你         |
| **[height]** | 机器人的身高       | 我身高[height]呢                 |
| **[weight]** | 机器人的体重       | 我的体重是[weight]               |
| **[sex]**    | 机器人的性别       | [cqname]是[sex]的哦              |
| **[zodiac]** | 机器人的星座       | [cqname]是[zodiac]的，[name]你呢 |
| **[blood]**  | 机器人的血型       | 我是[blood]血型的                |
| **[school]** | 机器人的学校       | 我目前在[school]学校呢           |
| **[city1]**  | 机器人的城市       | 我来自[city1]                    |
| **[city2]**  | 机器人的城市地区   | 我来自[city1]的[city2]           |



#### 追一科技



#### 广州火焰信息科技有限公司

http://www.birdbot.cn/product-bot.html



