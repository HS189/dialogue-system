### Blogs

+ 聊天机器人中对话模板的高效匹配方法

  <https://blog.csdn.net/malefactor/article/details/52166235>

+ 聊天机器人知识库模型和推理技术的选择

  <http://blog.sina.com.cn/s/blog_62bcc50c01010g81.html>

  论述以文本匹配为基础的推理机制的可能方案及其优缺点：

  1、正则表达式

     作为在日常开发中最常用的文本匹配方式，正则表达式看起来是自然而然的选择。但且慢，我们先分析一下正则表达式的匹配机制和聊天机器人的匹配流程。

     正则表达式通过回溯机制进行匹配。它能够对连续文本提供表面精确匹配，但没有歧义识别的能力。歧义识别也是中文分词系统要解决的难题之一。所以在聊天机器人系统里，通常采用分词系统预先对用户输入和知识库的“问题”进行分词。如果直接采用正则表达式进行匹配，就可能出现“准确率”不高的问题。而对于聊天机器人，要求能精确匹配问题，找出对应的答案。 

     最主要的问题，想想采用正则表达式后的匹配流程。用户输入“我想查询电费”，然后需要遍历知识库里所有的正则表达式条目，一条条进行匹配，其性能可想而知。因此直接采用正则表达式并不是可取的方案，最多只能作为辅助手段。

     

  2、反向索引

  ​    又叫倒排索引，这种数据结构存储单词与单词自身在一个或多个文档中所在位置之间的映射，常见于全文检索引擎。全文检索在构建索引时，也可以利用分词技术来解决歧义问题，所采用的索引结构也可以保证快速检索到结果的需求。似乎也可以作为推理引擎的选择。但反向索引结果的设计目标是为了通过索引词快速找到对应的文档（或者“问题”），在多个索引词情况下，虽然可以通过组合调用，辅以pagerank算法提高匹配的“准确率”。但这种索引结构不易支持"*"等通配符的模糊匹配方式(好吧，其实lucene之类的全文检索引擎也是支持通配符和模糊匹配”）。另外全文检索引擎的索引结构除了反向索引外，还包括其它信息，比如关键字在文档里的位置，关键字在文档中出现的频率等，这些信息对于应答机器人来说没有必要，也显得过“重”。因此反向索引结构和匹配机制也不能直接拿来使用。

  

  3、aiml回溯推理

     通过前两个问题的分析，可以在1和2之间，一方缺少的东西正是另一方的优势。因此自然可以想到通过结合二者的优点来构建存储模型。AIML模型就是这样一个实现。在AIML中，通过对知识库的“问题”预分词，然后采用多级索引结构进行存储。比如“查询电费”和“查询历史电费”、“查询业扩流程”，可以采用三级索引结构。第一级存储”查询“，第二级存储”电费“、”历史“和”业扩“，第三级存储”电费“和流程”。上级索引拥有指向下级索引的指针。其本身构成一个树状的索引结构。采用这种模型，有以下优点：节省存储空间；多级索引可以保证检索的速度；上级索引拥有访问下级索引的能力，可以保证对整个句子匹配的连续性，容易实现回溯匹配的功能，提供”*"等通配符的模糊匹配能力。因此是一种比较理想的知识库存储模型。

  ​    AIML索引结构和全文检索索引还有另一个重要的区别。由于检索机制的不同，全文检索结构的结果数量是0，1，N（1+）;对于AIML索引结构，其检索结果的数量是0或者1，即不存在1+的结果。对于应答业务场景来说，更需要的是确定性的唯一的结果，所以AIML的方式更适合应答业务场景。

     

   题外话:

  ​    在方案1和方案3里都提到“回溯”，这是正则表达式NFA引擎最重要的性质之一，也是文本匹配领域常用的技术。NFA引擎会依次处理各个子表达式或组成元素，遇到需要在两个可能成功的可能中进行选择的时候，它会选择其一，同时记住另一个，以备稍后可能的回溯需要。在方案3里采用的数据结构，使我们可以只实现简单的星号匹配的回溯（这在聊天机器人匹配场景里是够用的），也可以根据特定需求实现更复杂的匹配功能。

     另外，关于aiml(Artificial Intelligence Markup Language) ，其本身是为建立聊天机器人的知识库所设计的一套标记语言，特点是简单易用，适合人工建立较大规模的知识条目，另外遵循这套非官方规范，可以做到知识库的共享。事实上在网上已经有人贡献很多英文、法语甚至日语等各种语系的聊天知识库，但可惜的是中文的几乎没有（事实是我没有找到）。aiml起源于英文，虽然理论上适用于各种语系，在实际实现中还是需要针对不同语言及应用场景的特点，对其做一些裁剪或者增强。

     aiml定义的是知识库标记语言，至于知识库如何在内存中存储、如何进行匹配，则没有强制定义。



### Application

On this site you will find dozens of Chatterbots in the categories.

<http://www.simonlaven.com/>



#### ELIZA

1966-麻省理工学院

用于临床治疗中模仿心理医生与病人互动

功能：关键词匹配和回复规则 - question what's the difference with regular expression?



tools:

<http://www.simonlaven.com/eliza.htm>

<https://github.com/jezhiggins/eliza.py>

<https://github.com/fortyMiles/PAIP-Python/tree/master/eliza>

Source paper: <https://web.stanford.edu/class/linguist238/p36-weizenabaum.pdf>

Strongly inspired by ["Paradigms of Artificial Intelligence Programming"](https://www.amazon.com/Paradigms-Artificial-Intelligence-Programming-Studies/dp/1558601910/ref=sr_1_1?ie=UTF8&qid=1537264309&sr=8-1&keywords=programming+paradigm&dpID=51aMLUO8KLL&preST=_SX218_BO1,204,203,200_QL40_&dpSrc=srch) by Peter Norvig.





#### UC

1988-加州伯克利分校

用于帮助用户学习使用UNIX操作系统

功能：分析输入语言、理解用户意图、选择合适内容、生成对话内容





#### ALICE (Artificial Linguistics Internet Computer Entity)

1995-Richard S Wallace

广泛应用于移动端虚拟助手

功能：AIML语言 - question what's the difference with regular expression?



tools:

<http://www.simonlaven.com/alice.htm>

<https://pandorabots.com/docs/>

<https://pandorabots.com/docs/aiml/aiml-basics.html>



### 中间语义表示

调用aiml、chatscript、IF中间语义表示等模板技术演进

more:

<https://en.wikipedia.org/wiki/Dialogue_system>



#### AIML

todo

<https://en.wikipedia.org/wiki/AIML>



<https://github.com/Shuang0420/aiml> py2/py3 徐阿衡 Rcommend!!!

<https://github.com/yaleimeng/py3Aiml_Chinese>  py3 chinese

<https://github.com/crownpku/aiml_chatbot>



<https://www.devdungeon.com/content/ai-chat-bot-python-aiml>

<https://github.com/DevDungeon/ChattyCathy> py3 english



<http://www.snakehacker.me/411>

<https://github.com/SnakeHacker/QA-Snake> py2 chinese

简介：

[Eric](https://github.com/SnakeHacker/QA-Snake)是一个采用Python编写的基于多搜索引擎和AIML技术的问答机器人。目前支持的功能有：闲聊，通用问答等。



<https://github.com/sohelamin/chatbot>  py2 english



<http://www.cnblogs.com/liufanping/p/5879822.html>

<https://github.com/Fanping/iveely.search> java



**待实现的功能：**

**1，自动生成模板（转换器-将excel等转换为模板）**

**2，问句转换成一种标准化/结构化Query**



通配符：

AIML1.0提供了*和_，表示“出现一次或者多次”（以下我简称它们为“1+统配符”）

AIML2.0新添加了^和#，表示“出现零次或者多次”（以下我简称它们为“0+统配符”）

它们的优先级关系：# -> _ -> ^ -> *;



AIML(Artificial Intelligence Markup Language-人工智能标记语言)

AIML是一种定义了匹配模式和响应规则的一种XML