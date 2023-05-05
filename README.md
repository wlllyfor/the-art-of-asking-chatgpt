# 向ChatGPT询问的艺术

本文档是对 Ibrahim John 的书籍《THE ART OF ASKING CHATGPT FOR HIGH QUALITY ANSWERS》的中文翻译，主要目的是练习我的英文阅读能力顺便学习一下 chatgpt相关的一些提问技巧，欢迎 star。

在翻译的过程中，原文没有给出具体的示例，我结合 chatgpt3.5 插入了一些具体示例图片。

原 pdf 文件详见本仓库。

<a name="nYoiZ"></a>
## 介绍
我很高兴地欢迎大家阅读我的新书《向ChatGPT索取高质量答案的艺术： 提示工程技术的完整指南》。<br />本书是一本全面的指南，用于了解和利用各种提示技术，从ChatGPT生成高质量的答案。<br />我们将探讨如何利用不同的提示工程技术来实现不同的目标。ChatGPT是一种最先进的语言模型，能够生成类似人类的文本。然而，了解向ChatGPT提问的正确方式，以获得我们所期望的高质量输出，是至关重要的。<br />而这正是本书的目的。无论你是普通人、研究人员、开发人员，还是仅仅想把ChatGPT作为自己领域的个人助理，这本书都是为你写的。<br />我使用了简单的语言和到位的实际解释，以及每个提示技术的例子和提示公式。通过这本书，你将学会如何使用提示工程技术来控制ChatGPT的输出，并根据你的具体需求生成文本。<br />在本书中，我们还提供了一些例子，说明如何结合不同的提示技术来实现更具体的结果。<br />我希望你会发现这本书的信息量很大，而且很有乐趣，就像我写这本书一样。
<a name="zMe8z"></a>
## 提示性工程技术介绍
提示工程是创建提示、询问或指示的过程，用于指导ChatGPT等语言模型的输出。它允许用户控制模型的输出，并生成符合其特定需求的文本。<br />ChatGPT是一个最先进的语言模型，能够生成类似人类的文本。它建立在转化器架构上，这使它能够处理大量的数据并生成高质量的文本。<br />然而，为了从ChatGPT获得最好的结果，了解如何正确提示模型是很重要的。<br />提示允许用户控制模型的输出，并生成相关、准确和高质量的文本。<br />在使用ChatGPT时，了解它的能力和限制是很重要的。<br />该模型能够生成类似人类的文本，但如果没有适当的指导，它可能并不总是产生所需的输出。<br />这就是提示工程的作用，通过提供明确和具体的指示，你可以指导模型的输出，并确保它是相关的。<br />提示公式是提示的具体格式，它一般由3个主要元素组成：

- 任务：对提示要求模型生成的内容的清晰和简明的陈述。
- 指示：模型在生成文本时应遵循的指示。
- 角色：模型在生成文本时应承担的角色。

在本书中，我们将探讨可用于ChatGPT的各种提示工程技术。我们将讨论<br />不同类型的提示，以及如何使用它们来实现你想要的特定目标。
<a name="p31G4"></a>
## 指令提示技术 
现在，让我们开始探索 "指令提示技术"，以及如何用它来从ChatGPT生成高质量的文本。指令提示技术是一种指导ChatGPT输出的方法，它为模型提供了具体的指令，使其得以遵循。这种技术对于确保输出是相关的和高质量的非常有用。<br />要使用指令提示技术，你需要为模型提供一个清晰简明的任务，以及供模型遵循的具体指令。<br />例如，如果你要生成客户服务回应，你将提供一个任务，如 "生成对客户咨询的回应"，以及指示，如 "回应应该是专业的，并提供准确的信息"。<br />提示公式： "按照这些指示生成[任务]： [说明]"<br />例子： 生成客户服务回复：

- 任务： 生成对客户询问的回应
- 指示： 答复应该是专业的，并提供准确的信息
- 提示公式： "按照这些指示对客户的询问做出专业和准确的回答： 回答应该是专业的，并提供准确的信息。"

例子： 生成一份法律文件：

- 任务： 生成一份法律文件
- 指示： 该文件应符合相关法律和法规的规定
- 提示公式： "生成一份符合相关法律和法规的法律文件，并遵循以下说明指示：该文件应符合相关法律和法规。"

在使用指令提示技术时，重要的是要记住，指令应该是清晰和具体的。这将有助于确保产出的相关性和质量。指令提示技术可以和下一章中解释的 "角色提示 "和 "种子词提示 "结合起来，以提高ChatGPT的输出。

![gpt0.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/21494320/1681985333896-e488606d-b3c4-4b5d-beb7-9c2c5f35abdb.jpeg#averageHue=%23ececec&clientId=u137130a2-d4e3-4&from=ui&id=uee679410&originHeight=3248&originWidth=1648&originalType=binary&ratio=2&rotation=0&showTitle=false&size=640185&status=done&style=none&taskId=u6268d9a8-8dcc-4b47-922c-04b37b6c0e6&title=)
<a name="mGH9g"></a>
## 角色提示
角色提示技术是一种引导ChatGPT输出的方法，它为模型提供一个特定的角色。这种技术对于生成适合特定环境或受众的文本非常有用。<br />要使用角色提示技术，你需要为模型提供一个清晰而具体的角色。例如，如果你正在生成客户服务的回应，你将提供一个角色，如 "客户服务代表"。<br />提示公式： "生成[任务]作为一个[角色]" <br />例子：<br />生成客户服务响应：

- 任务： 生成对客户询问的答复
- 角色： 客户服务代表
- 提示公式： "作为一名客户服务代表，对客户的询问做出答复。" 

生成一个法律文件：

- 任务： 生成一个法律文件
- 角色：律师
- 提示公式： "以律师的身份生成一份法律文件"。

将角色提示技术与指令提示和种子词提示结合起来使用会提高ChatGPT的输出效果。<br />下面是一个如何结合指令提示、角色提示和种子词提示技术的例子：

- 任务： 为一个新的智能手机生成一个产品描述 
- 指示： 描述应该是有信息的，有说服力的，并突出智能手机的独特功能。
- 角色： 营销代表 
- 种子词: "创新"
- 提示公式： "作为一名营销代表，产生一个信息量大、有说服力的产品描述，突出新智能手机的创新特点。该智能手机有以下特点[插入你的特点]"

在这个例子中，指令性提示被用来确保产品描述的信息性和说服力。角色提示被用来确保描述是从营销代表的角度来写的。种子词提示用于确保描述的重点是智能手机的创新功能。

![gtp0-1.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/21494320/1682046703467-a4dbd314-f654-4593-bd87-3e720d95237a.jpeg#averageHue=%23e4e4e4&clientId=u137130a2-d4e3-4&from=ui&id=uf06d9224&originHeight=1066&originWidth=1648&originalType=binary&ratio=2&rotation=0&showTitle=false&size=320429&status=done&style=none&taskId=u4c32a141-702a-478f-9358-40027953797&title=)
<a name="qCNZq"></a>
## 标准提示语
标准提示是指导ChatGPT输出的一种简单方法，它提供了一个特定的任务让模型完成。<br />例如，如果你想生成一篇新闻文章的摘要，你可以提供一个任务，如 "总结这篇新闻文章"。<br />提示公式： "生成一个[任务]"<br />例子：<br />生成一篇新闻文章的摘要： 

- 任务： 总结这篇新闻报道
- 提示公式： "生成这篇新闻报道的摘要" 

生成一个产品评论：

- 任务： 为一款新的智能手机写一篇评论
- 提示公式： "生成对这款新智能手机的评论"

另外，标准提示可以与其他技术相结合，如角色提示和种子词提示，以提高ChatGPT的输出。<br />下面是一个如何结合标准提示、角色提示和种子词提示技术的例子：

- 任务： 为一个新的笔记本电脑生成一个产品评论 
- 指示： 该评论应该是客观的、信息丰富的，并突出笔记本电脑的独特功能。
- 角色： 技术专家
- 种子词："强大"
- 提示公式： "作为一个技术专家，产生一个客观和信息丰富的产品评论，突出新笔记本电脑的强大功能。"

在这个例子中，标准的提示技术被用来确保模型产生一个产品评论。角色提示被用来确保评论是以技术专家的角度来写的。种子词提示被用来确保评论的重点是笔记本电脑的强大功能。

![gpt0-2.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/21494320/1682046946399-a14c6d13-742e-4d1b-a8ff-e45640e33ec8.jpeg#averageHue=%23dde1e6&clientId=u137130a2-d4e3-4&from=ui&id=uf9745d93&originHeight=508&originWidth=1648&originalType=binary&ratio=2&rotation=0&showTitle=false&size=161382&status=done&style=none&taskId=uac1e75f5-570f-4ddd-a104-6517d9d39f4&title=)
<a name="Td1UJ"></a>
## 零、一和少量样本提示 
零样本、一次样本和少量样本提示是用于从ChatGPT中生成文本的技术，只需极少或没有例子。当某一特定任务的数据有限或者是新任务的时候，这些技术是有用的。当特定的任务可用的数据有限时，或者当任务是新的，没有明确的定义时，这些技术是有用的。<br />当任务没有可用的例子时，就会使用零样本提示技术。该模型被提供给一个一般的任务，并根据其对任务的理解生成文本。<br />当任务只有一个例子可用时，就使用一次样本提示技术。向模型提供例子，并根据其对例子的理解生成文本。<br />当任务中可用的例子数量有限时，就会使用少量提示技术。向模型提供例子，并根据其对例子的理解生成文本。<br />提示公式： "根据[数目]的例子生成文本" <br />例子：<br />为一个新产品生成一个产品描述，但没有可用的例子：

- 任务： 为一个新的智能手表写一个产品描述
- 提示公式： "为这个新的智能手表生成一个没有实例的产品描述"

生成一个有实例的产品比较：

- 任务： 将一款新的智能手机与最新的iPhone进行比较
- 提示公式： "用一个例子（最新的iPhone）生成这个新智能手机的产品比较"

生成一个有少数例子可用的产品评论：

- 任务： 写一篇关于一个新的电子阅读器的评论
- 提示公式： "用很少的例子（3个其他的电子阅读器）生成对这个新的电子阅读器的评论"

这些技术可以用来根据模型对任务的理解或提供的例子来生成文本。

![gpt0-3.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/21494320/1682047143451-47c83213-9552-4e03-a801-7bfeea335326.jpeg#averageHue=%23e9e9e9&clientId=u137130a2-d4e3-4&from=ui&id=uc9a5fd16&originHeight=1130&originWidth=1648&originalType=binary&ratio=2&rotation=0&showTitle=false&size=286270&status=done&style=none&taskId=udf2456a4-c63a-49f5-a616-a82c89170dd&title=)
<a name="glClT"></a>
## 提示语：让我们思考一下
"让我们思考一下"的提示是一种用来鼓励ChatGPT产生反思和沉思的文本的技巧。这种技巧对写论文、诗歌或创意写作等任务很有用。<br />让我们思考一下的提示公式是简单的短语 "让我们思考一下"，然后是一个主题或问题。<br />例子：<br />生成一篇反思性文章：

- 任务： 以个人成长为主题写一篇反思性文章
- 提示公式： "我们来思考一下：个人成长" 

生成一首诗：

- 任务： 写一首关于季节变化的诗
- 提示公式： "让我们想一想：变化的季节" 

这个提示是要求就一个特定的话题或想法进行对话或讨论。 演讲者邀请ChatGPT参与到关于当前主题的对话。<br />该模型提供了一个提示，作为对话或文本生成的起点。<br />然后，该模型使用其训练数据和算法来生成与提示相关的反应。这种技术使ChatGPT能够根据所提供的提示，生成符合语境的、连贯的文本。<br />要使用ChatGPT的 "让我们想想这个提示 "技术，你可以遵循以下步骤：<br />1. 确定你想讨论的主题或想法。<br />2. 制定一个提示，清楚地说明这个话题或想法，并开始对话或生成文本。<br />3. 用 "让我们想想 "或 "让我们讨论 "作为提示的前言，以表明你正在发起对话或讨论。以表明你正在发起一场对话或讨论。<br />下面是几个使用这种技巧的提示的例子：

- 提示： "让我们思考一下气候变化对农业的影响"
- 提示： "让我们讨论一下人工智能的现状"
- 提示： "让我们谈谈远程工作的好处和坏处"

你也可以添加一个开放式的问题、声明或一段你希望模型继续或建立的文字。<br />一旦你提供了提示，模型将使用其训练数据和算法，生成与提示相关的回应，并将以连贯的方式继续对话。<br />这种独特的提示有助于ChatGPT以不同的角度和视角给出答案，从而产生更多动态和信息的段落。<br />使用提示的步骤简单易行，它确实可以使你的写作发生变化。请试一试，自己看看吧。

![gpt1.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/21494320/1681979348095-b063addf-27ef-41d3-abd5-9404ae798c1b.jpeg#averageHue=%23e7e7e7&clientId=u137130a2-d4e3-4&from=ui&id=ud8b75aba&originHeight=1098&originWidth=1648&originalType=binary&ratio=2&rotation=0&showTitle=false&size=298105&status=done&style=none&taskId=ub2fd0e9e-b006-4fb5-a619-5aad01d25d0&title=)
<a name="vvhrA"></a>
## 自洽性提示
自洽性提示是一种技术，用于确保ChatGPT的输出与提供的输入一致。这种技术对于事实检查、数据验证或文本生成中的一致性检查等任务非常有用。文本生成中的一致性检查。<br />自洽性提示的提示公式是输入的文本，然后是 "请确保以下文本是自我一致的"的指令。<br />或者，可以提示模型生成与所提供的输入一致的文本。<br />提示示例及其公式： <br />例1：文本生成

- 任务：生成一个产品评论
- 指示：该评论应与输入的产品信息一致。
- 提示公式： "生成一个与以下产品信息一致的产品评论[插入产品信息]"

例2：文本总结

- 任务： 总结一篇新闻报道
- 指示： 摘要应与文章中提供的信息相一致
- 提示公式： "以与所提供的信息一致的方式对以下新闻文章进行总结[插入新闻文章]"

例3：文本完成

- 任务： 完成一个句子
- 指示： 完成的内容应与输入的上下文一致
- 提示公式： "以符合上下文的方式完成以下句子[插入句子]"

例4：<br />1. 事实核查：

- 任务： 检查某篇新闻文章中的一致性
- 输入文本： "文章中说该城市的人口是500万，但后来又说人口是700万。" 
- 提示公式： "请确保以下文字是自洽的： 文章说该城市的人口是500万，但后来又说人口是700万。"

2. 数据验证：

- 任务： 检查给定数据集的一致性
- 输入文本： "数据显示，7月的平均温度为30度，但最低温度记录为20度。"
- 提示公式： "请确保下面的文字是自洽的： 数据显示，7月的平均温度是30度，但最低温度记录为20度。"

![gpt0-4.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/21494320/1682047575601-053e56cd-b5f8-41f5-a0c1-1f59522d514d.jpeg#averageHue=%23e4e4e4&clientId=u137130a2-d4e3-4&from=ui&id=u81685969&originHeight=1116&originWidth=1648&originalType=binary&ratio=2&rotation=0&showTitle=false&size=332161&status=done&style=none&taskId=u70d0945d-004f-4e8a-af8b-362ad3e04d2&title=)
<a name="jk9vn"></a>
## 种子词提示
种子词提示是一种用于控制ChatGPT输出的技术，它提供了一个特定的种子词或短语。<br />种子词的提示公式是种子词或短语，后面是 "请根据以下种子词生成文本 "的指令：<br />文本生成：

- 任务： 生成一个关于龙的故事
- 种子词："龙"
- 提示公式： "请根据以下种子词生成文本：龙"

语言翻译：

- 任务： 将一个句子从英语翻译成西班牙语 
- 种子词："hello"
- 提示公式： "请根据以下种子词生成文本：hello"

这个技术允许模型生成与种子词相关的文本，并在此基础上进行扩展。这是一种控制模型生成的文本与某个主题或语境相关的方法。<br />种子词提示可以与角色提示和指令提示相结合，以创造更具体和有针对性的生成文本。通过提供一个种子词或短语，模型可以生成与该种子词或短语相关的文本，通过提供所需输出和角色的信息，模型可以生成与角色或指令一致的特定风格或语气的文本。这允许对生成的文本进行更多的控制，对广泛的应用是很有用的<br />下面是提示实例及其公式： <br />例子1：文本生成

- 任务： 生成一首诗
- 指示： 这首诗应与种子词 "爱 "有关，并应以十四行诗的风格来写。
- 角色： 诗人
- 提示公式： "以诗人的身份产生一首与种子词'爱'有关的十四行诗"

例2：文本完成

- 任务： 完成一个句子
- 指示： 完成的内容应与种子词 "科学 "有关，并应以研究论文的形式写出。
- 角色： 研究人员
- 提示公式： "以研究人员的身份，用与种子词'科学'有关的方式，并以研究论文的风格来完成以下句子：[插入句子]"

例3：文本归纳

- 任务： 总结一篇新闻报道
- 指示： 摘要应与种子词 "政治 "相关，并应以中立和不偏不倚的语气来写。
- 角色： 记者
- 提示公式： "作为一名记者，以中立和不偏不倚的语气，用与种子词'政治'有关的方式来总结以下新闻文章： [插入新闻文章]"

![gpt2.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/21494320/1681981792659-e23336b2-d872-49c9-961a-6609d09c8a90.jpeg#averageHue=%23f2f2f2&clientId=u137130a2-d4e3-4&from=ui&id=ue7068345&originHeight=882&originWidth=1648&originalType=binary&ratio=2&rotation=0&showTitle=false&size=176692&status=done&style=none&taskId=ua755f830-b5a1-4b50-b220-2ce47fce27c&title=)
<a name="T0am3"></a>
## 知识生成提示
知识生成提示是一种技术，用于从ChatGPT中获取 新的和原始的信息。<br />知识生成的提示公式是 "请产生关于X的新的和原始的信息"，其中X是感兴趣的主题。<br />这是一种使用模型已有的知识来产生新信息或回答问题的技术。<br />要在ChatGPT中使用这个提示，应该向模型提供一个问题或话题作为输入，同时提供一个提示，指明生成文本的任务或目标。该提示应包括有关所需输出的信息，如要生成的文本类型和任何具体要求或限制。<br />下面是提示的例子和它们的公式： <br />例子1：知识生成

- 任务： 生成关于一个特定主题的新信息
- 指示： 生成的信息应该是准确的，与主题相关的。
- 提示公式： "产生关于[特定主题]的新的和准确的信息"

例2： 回答问题

- 任务： 回答一个问题
- 指示： 回答要准确并与问题相关
- 提示公式： "回答以下问题： [插入问题]"

例3：知识整合

- 任务： 将新的信息与现有的知识进行整合
- 指示： 整合的内容要准确，并与主题相关。
- 提示公式： "将以下信息与关于[特定主题]的现有知识相结合： [插入新信息]"

例4：数据分析：

- 任务： 从给定的数据集中产生关于客户行为的洞察力
- 提示公式： "请从这个数据集中生成关于客户行为的新的和原始的信息"

![gpt9.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/21494320/1682057667846-21e82021-160d-4839-b531-d7de86ea34cf.jpeg#averageHue=%23eaeaea&clientId=u137130a2-d4e3-4&from=ui&id=u28ad1572&originHeight=1112&originWidth=1648&originalType=binary&ratio=2&rotation=0&showTitle=false&size=250899&status=done&style=none&taskId=u2316d275-8e43-418a-bded-40b72e2a1e0&title=)

<a name="WabCb"></a>
## 知识整合提示 
这种技术利用模型已有的知识来整合新的信息或连接不同的信息。<br />这种技术对于将现有的知识与新的信息结合起来，以产生对某一特定主题的更全面的理解是很有用的。<br />如何用ChatGPT来使用它：<br />应向模型提供一个新的信息和现有的知识作为输入，同时提供一个提示，说明生成文本的任务或目标。该提示应包括关于所需输出的信息，如要生成的文本类型和任何具体要求或限制。<br />提示的例子和它们的公式： <br />例1：知识整合

- 任务： 将新的信息与现有的知识进行整合
- 指示： 整合的内容要准确，并与主题相关。
- 提示公式： "将以下信息与关于[特定主题]的现有知识相结合： [插入新信息]"

例2：连接信息片段

- 任务： 连接不同的信息片段
- 指示： 联系应该是相关的和有逻辑的 
- 提示公式： "以相关和符合逻辑的方式连接以下信息：[插入信息1][插入信息2]"

例3：更新现有知识

- 任务： 用新的信息更新现有的知识
- 指示： 更新的信息应该是准确和相关的
- 提示公式： "用以下信息更新关于[特定主题]的现有知识： [插入新信息]"

![gtp10.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/21494320/1682048269478-04ba865a-235d-4e32-95f0-caa3b2e82751.jpeg#averageHue=%23e7e7e7&clientId=u137130a2-d4e3-4&from=ui&id=ubaa3d51c&originHeight=1200&originWidth=1648&originalType=binary&ratio=2&rotation=0&showTitle=false&size=318325&status=done&style=none&taskId=u3134f9b3-5c56-4185-9980-650f186c716&title=)
<a name="iYZGu"></a>
## 多项选择提示
这种技术以一个问题或任务和一组预定义的选项作为潜在的答案来展示一个模型。<br />这种技术对于生成仅限于一组特定选项的文本很有用，可以用于回答问题、完成文本和其他任务。该模型可以生成仅限于预定义选项的文本。<br />要使用ChatGPT的多项选择提示，应该向模型提供一个问题或任务作为输入，同时提供一组预定义的选项作为潜在的答案。该提示还应该包括关于所需输出的信息，如要生成的文本类型和任何具体要求或限制。<br />提示的例子和它们的公式： <br />例1： 问题回答

- 任务： 回答一个多选题
- 指示： 答案应该是预定义的选项之一
- 提示公式： "通过选择下列选项之一来回答下列问题： [插入问题] [插入选项1] [插入选项2] [插入选项3]"

例2：文本填写

- 任务： 用预定义的选项之一完成一个句子
- 指示： 完成的内容应该是预定义的选项之一。
- 提示公式： "从以下选项中选择一个来完成下面的句子： [插入句子] [插入选项1] [插入选项2] [插入选项3]"

例3：情绪分析

- 任务： 将一段文字分类为正面、中性或负面
- 指示： 该分类应该是预定义的选项之一
- 提示公式： "从以下选项中选择一个，将以下文本分类为正面、中立或负面： [插入文本][正面][中性][负面]"

![gpt3.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/21494320/1681984824678-19909e43-ae40-4c2d-862b-5e6b9db8aef4.jpeg#averageHue=%23e7e7e7&clientId=u137130a2-d4e3-4&from=ui&id=Nezff&originHeight=808&originWidth=1648&originalType=binary&ratio=2&rotation=0&showTitle=false&size=215604&status=done&style=none&taskId=uba54d0c9-aed6-464f-8803-cefb24d0b1b&title=)
<a name="MZ8os"></a>
## 可解释的软提示 
可解释的软提示是一种技术，它允许控制模型的生成文本，同时为模型提供一些灵活性。它是通过向模型提供一组受控输入和一些关于期望输出的附加信息来实现的。这种技术 允许产生更多可解释和可控制的文本。提示例子及其公式：<br />例子1：文本生成

- 任务： 生成一个故事
- 指示： 故事应基于一组给定的人物和一个特定的主题。
- 提示公式： "根据以下人物生成一个故事： [插入人物]和主题：[插入主题]"

例2：文本完成

- 任务： 完成一个句子
- 指示： 完成的句子应具有特定作者的风格
- 提示公式： "以[特定作者]的风格完成以下句子： [插入句子]"

例3：语言模型

- 任务： 生成特定风格的文本
- 指示： 该文本应具有特定时期的风格 
- 提示公式： "以[特定时期]的风格生成文本： [插入上下文]"

![gpt12.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/21494320/1682058753307-96672cec-7ced-4a2b-8c43-8b1b9bdc9de9.jpeg#averageHue=%23e7e7e7&clientId=u137130a2-d4e3-4&from=ui&id=u79b920bf&originHeight=1284&originWidth=1648&originalType=binary&ratio=2&rotation=0&showTitle=false&size=335720&status=done&style=none&taskId=ue195f09f-9fd3-4d14-8030-2cf1fde78e2&title=)
<a name="kN9Vt"></a>
## 受控生成提示 
受控生成提示是允许以对输出的高度控制来生成文本的技术。<br />这是通过向模型提供一组特定的输入，如模板、特定的词汇或一组约束来实现的，这些输入可以用来指导生成过程。下面是一些提示例子和它们的公式：<br />例子1：文本生成

- 任务： 生成一个故事
- 指示： 该故事应基于一个特定的模板 
- 提示公式： "根据以下模板生成一个故事： [插入模板]" 

例2：文本完成

- 任务： 完成一个句子
- 指示： 完成时应使用一个特定的词汇 
- 提示公式： "使用以下词汇完成以下句子：[插入词汇]： [插入句子]" 

例3：语言模型

- 任务： 生成特定风格的文本
- 指示： 该文本应遵循一套特定的语法规则
- 提示公式： "生成遵循以下语法规则的文本： [插入规则]： [插入上下文]"

通过向模型提供一组可用于指导生成过程的特定输入，受控生成提示允许生成的文本更可控和可预测

![gpt13.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/21494320/1682059763397-427c0168-940b-494a-bef4-6b4fe370fef8.jpeg#averageHue=%23e9e9e9&clientId=u137130a2-d4e3-4&from=ui&id=u548a2a11&originHeight=440&originWidth=1648&originalType=binary&ratio=2&rotation=0&showTitle=false&size=113903&status=done&style=none&taskId=ufdc43bb0-e102-4030-a0b5-a6d49239a40&title=)
<a name="u68i9"></a>
## 回答问题的提示 
问题回答提示是一种技术，它允许模型生成回答特定问题或任务的文本。这是通过向模型提供一个问题或任务作为输入，以及任何可能与该问题或任务相关的附加信息来实现的。<br />一些提示的例子和它们的公式是：<br />例子1： 事实性问题的回答

- 任务： 回答一个事实性问题
- 指示： 回答要准确，要有针对性 
- 提示公式： "回答下列事实性问题： [插入问题]"

例2： 定义

- 任务： 提供一个词的定义
- 指示： 定义应该是准确的
- 提示公式： "给下面这个词下个定义：[插入词]"

例3：信息检索

- 任务： 从一个特定的来源获取信息
- 指示： 检索到的信息应该是相关的 
- 提示公式： "从以下来源获取有关[特定主题]的信息： [插入来源]"

这对回答问题和信息检索等任务很有用。

![gpt14.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/21494320/1682061442747-a624680c-3e75-43bb-b705-a831b5a52720.jpeg#averageHue=%23e9e9e9&clientId=u137130a2-d4e3-4&from=ui&id=u850846f7&originHeight=408&originWidth=1648&originalType=binary&ratio=2&rotation=0&showTitle=false&size=102803&status=done&style=none&taskId=uee5847f3-96e3-4808-bca1-f1c3c0931d2&title=)
<a name="HMyyG"></a>
## 总结性提示 
总结提示是一种技术，它允许模型生成一个给定文本的较短版本，同时保留其主要观点和信息。<br />这是通过向模型提供一个较长的文本作为输入并要求它生成该文本的摘要来实现的。<br />这种技术对于文本总结和信息压缩等任务非常有用。<br />如何用ChatGPT来使用它：<br />应向模型提供一个较长的文本作为输入，并要求其生成该文本的摘要。该提示还应该包括有关期望输出的信息，如期望的摘要长度和任何具体要求或限制。<br />提示的例子和它们的公式： <br />例1：文章摘要

- 任务： 总结一篇新闻文章
- 指示： 摘要应该是对文章主要内容的简要概述
- 提示公式： "用一个简短的句子概括以下新闻文章： [插入文章]"

例2：会议记录

- 任务： 总结一份会议记录
- 指示： 摘要应强调会议的主要决定和行动
- 提示公式： "总结以下会议记录，列出主要的决定和采取的行动： [插入会议记录]"

例3：书籍摘要 

- 任务： 对一本书进行总结
- 指示： 总结应该是对该书主要内容的简要概述
- 提示公式： "用一个简短的段落来总结下面这本书： [插入书名]"

![gpt15.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/21494320/1682064544920-b003c4f1-4c6e-4692-8d86-0118646bb097.jpeg#averageHue=%23e8e8e8&clientId=u137130a2-d4e3-4&from=ui&id=u2f3b9fd4&originHeight=458&originWidth=1648&originalType=binary&ratio=2&rotation=0&showTitle=false&size=129003&status=done&style=none&taskId=udb9fe39e-eaae-415d-b051-8f085c9d790&title=)
<a name="mOBuh"></a>
## 对话提示
对话提示是一种技术，它允许模型生成模拟两个或多个实体之间对话的文本。通过向模型提供一个背景和一组人物或实体，以及他们的角色和背景，并要求模型 产生它们之间的对话<br />因此，应该向模型提供一个背景和一组人物或实体，以及他们的角色和背景。角色或实体，以及他们的角色和背景。还应该向模型提供有关期望输出的信息，如对话的类型和任何具体要求或限制。<br />提示的例子及其公式： <br />例子1： 对话的产生

- 任务： 生成两个人物之间的对话
- 指示： 对话应该是自然的，并与给定的环境相关。
- 提示公式： "在下面的语境中[插入语境]，生成以下人物[插入人物]之间的对话"

例2：写故事

- 任务： 在一个故事中生成一段对话
- 指示： 对话应与故事中的人物和事件相一致
- 提示公式： "在以下故事[插入故事]中的以下人物[插入人物]之间产生一段对话"

例3：聊天机器人的开发

- 任务： 为一个客户服务聊天机器人生成一段对话
- 指示： 对话应该是专业的，并提供准确的信息
- 提示公式： "当客户问及[插入话题]时，为客户服务聊天机器人生成一个专业而准确的对话"

因此，这种技术对对话生成、故事写作和聊天机器人开发等任务很有用。

![gpt16.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/21494320/1682067854645-3756f488-ca5a-417c-b553-d426f65f5883.jpeg#averageHue=%23ebebeb&clientId=u137130a2-d4e3-4&from=ui&id=u7ef1bd8f&originHeight=1258&originWidth=1648&originalType=binary&ratio=2&rotation=0&showTitle=false&size=270069&status=done&style=none&taskId=ud9124b94-6bbd-4ce3-a1f2-a23433f9778&title=)
<a name="ZTOZu"></a>
## 对抗性提示 
对抗性提示是一种技术，它允许模型生成对某些类型的攻击或偏见有抵抗力的文本。这种技术可以用来训练更加稳健和抵抗某些类型的攻击或偏见的模型。<br />要使用ChatGPT的对抗性提示，应该为模型提供一个提示，该提示的设计是让模型难以生成与预期输出一致的文本。该提示还应该包括有关期望输出的信息，如要生成的文本类型和任何具体要求或限制。<br />提示实例及其公式：<br />例1：文本分类的对抗性提示

- 任务： 生成被分类为特定标签的文本
- 指示： 生成的文本应该很难被归类为特定的标签
- 提示公式： "生成难以被归类为[插入标签]的文本"

例2：情绪分析的对抗性提示

- 任务： 生成难以被归类为特定情感的文本
- 指示： 生成的文本应该难以被归类为特定的情感。
- 提示公式： "生成难以被归类为具有[插入情感]的文本"

例3：语言翻译的对抗性提示

- 任务： 生成难以翻译的文本
- 指示： 生成的文本应该是难以翻译成目标语言的。
- 提示公式： "生成难以翻译成[插入目标语言]的文本"

![gpt17.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/21494320/1682218735893-70c66143-0c10-4dcd-b635-461d0f40b176.jpeg#averageHue=%23e8e8e8&clientId=u137130a2-d4e3-4&from=ui&id=u060836db&originHeight=916&originWidth=1648&originalType=binary&ratio=2&rotation=0&showTitle=false&size=236572&status=done&style=none&taskId=u038535de-8e72-4b9c-be84-959072d3da0&title=)
<a name="LoBop"></a>
## 聚类提示
聚类提示是一种技术，它允许模型根据某些特征或特性将类似的数据点分组。<br />这是通过向模型提供一组数据点并要求它根据某些特征或特性将它们分组来实现的。<br />这种技术对于数据分析、机器学习和自然语言处理等任务非常有用。

如何用ChatGPT来使用它：<br />应向模型提供一组数据点，并要求它根据某些特征或特性将它们分组。该提示还应该包括关于所需输出的信息，如要生成的集群数量和任何具体要求或限制。<br />提示的例子及其公式：<br />例1：客户评论的聚类

- 任务： 将类似的顾客评论归为一组
- 指示： 评论应根据情绪进行分组
- 提示公式： "根据情绪将以下顾客评论分组： [插入评论]"

例2：对新闻文章进行分组

- 任务： 将类似的新闻文章归为一组
- 指示： 这些文章应该根据主题进行分组 
- 提示公式： "根据主题，将下列新闻文章分组： [插入文章]" 

例3：科学论文的分组

- 任务： 将类似的科学论文分组
- 指示： 应根据研究领域对论文进行分组
- 提示公式： "根据研究领域，将下列科学论文分组： [插入论文]"

![gpt18.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/21494320/1682236865912-b3ce670c-cd9c-4de5-a259-76e7a707210e.jpeg#averageHue=%23e3e8ec&clientId=u137130a2-d4e3-4&from=ui&id=u39596f51&originHeight=978&originWidth=1648&originalType=binary&ratio=2&rotation=0&showTitle=false&size=271798&status=done&style=none&taskId=u7af847c2-8010-4496-b583-5cfd9cb3821&title=)

<a name="fNnfW"></a>
## 强化学习提示 
强化学习提示是一种技术，它允许模型从其过去的行为中学习，并随着时间的推移提高其性能。要使用ChatGPT的强化学习提示，应该向模型提供一组输入和奖励，并允许它根据收到的奖励调整其行为。提示还应该包括有关期望输出的信息，如要完成的任务和任何具体的要求或限制。这种技术对决策、游戏和自然语言生成等任务很有用。<br />提示的例子和它们的公式：<br />例子1： 文本生成的强化学习

- 任务： 生成与特定风格一致的文本
- 指示： 该模型应根据其生成符合特定风格的文本所获得的奖励来调整其行为。
- 提示公式： "使用强化学习来生成与以下风格一致的文本[插入风格]"

例2： 语言翻译的强化学习

- 任务： 将文字从一种语言翻译成另一种语言
- 指示： 该模型应根据其产生准确翻译的奖励来调整其行为
- 提示公式： "使用强化学习将以下文本[插入文本]从[插入语言]翻译成[插入语言]"

例3： 问题回答的强化学习

- 任务： 生成一个问题的答案
- 指示： 该模型应根据产生准确答案所获得的奖励来调整其行为。
- 提示公式： "使用强化学习来生成以下问题的答案[插入问题]"

![gpt19.png](https://cdn.nlark.com/yuque/0/2023/png/21494320/1682232356449-4a867bb4-9d85-42c8-8448-04fdab8f35ca.png#averageHue=%235ba98c&clientId=u137130a2-d4e3-4&from=ui&id=u5591b67c&originHeight=1676&originWidth=1336&originalType=binary&ratio=2&rotation=0&showTitle=false&size=365519&status=done&style=none&taskId=u27ae2a81-1bf4-484f-a52e-70029f5852a&title=)
<a name="juLgG"></a>
## 课程学习提示 
课程学习是一种技术，它允许模型通过首先在较简单的任务上进行训练，并逐渐增加难度来学习复杂的任务。<br />要使用ChatGPT的课程学习提示，应该为模型提供一连串难度逐渐增加的任务。提示还应该包括有关期望输出的信息，如要完成的最终任务和任何具体要求或限制。<br />这种技术对自然语言处理、图像识别和机器学习等任务很有用。<br />提示的例子和它们的公式：<br />例1：文本生成的课程学习

- 任务： 生成与特定风格一致的文本
- 指示： 该模型应在较简单的文体上进行训练，然后再转向较复杂的文体
- 提示公式： "使用课程学习来生成符合以下风格的文本[插入风格]，并按以下顺序[插入顺序]"

例2：语言翻译的课程学习

- 任务： 将文本从一种语言翻译成另一种语言
- 指示： 该模型应在较简单的语言上进行训练，然后再转向较复杂的语言
- 提示公式： "使用课程学习，按照下列语言[插入语言]的顺序翻译文本[插入顺序]"

例3：用于回答问题的课程学习 任务： 生成一个问题的答案

- 指示： 该模型应先在较简单的问题上进行训练，然后再转向较复杂的问题
- 提示公式： "使用课程学习来生成以下问题的答案[插入问题]，顺序如下[插入顺序]"

![gpt20.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/21494320/1682235989837-deac338a-f229-461a-82d4-26c4850dd44a.jpeg#averageHue=%23e1e8ef&clientId=u137130a2-d4e3-4&from=ui&id=ub51251f4&originHeight=1318&originWidth=1648&originalType=binary&ratio=2&rotation=0&showTitle=false&size=294234&status=done&style=none&taskId=u9911c712-1cf4-4f85-ab1c-73841d9764a&title=)

![gpt20-1.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/21494320/1682236003780-bad51a10-148b-442a-b0bc-19735043f7d5.jpeg#averageHue=%23ebebeb&clientId=u137130a2-d4e3-4&from=ui&id=udad26ee3&originHeight=764&originWidth=1648&originalType=binary&ratio=2&rotation=0&showTitle=false&size=189793&status=done&style=none&taskId=u635c921e-a65b-485b-9efc-2c34d7fd835&title=)
<a name="wZfAZ"></a>
## 情绪分析提示 
情感分析是一种技术，它允许模型确定一段文本的情感基调或态度，例如它是积极的、消极的还是中立的。<br />要使用ChatGPT的情感分析提示，应该向模型提供一段文本，并要求它根据其情感进行分类。<br />提示还应该包括关于所需输出的信息，如要检测的情感类型（如正面、负面、中性）以及任何具体要求或限制。<br />提示示例及其公式：<br />例1：客户评论的情绪分析

- 任务： 确定客户评论的情绪
- 指示： 该模型应将评论分类为正面、负面或中性
- 提示公式： "对以下客户评论[插入评论]进行情感分析，并将其分类为正面、负面或中性。"

例2：对推文进行情感分析

- 任务： 确定推文的情绪
- 指示： 该模型应该将推文分类为正面、负面或中性
- 提示公式： "对以下推文[插入推文]进行情感分析，并将其分类为正面、负面或中性。"

例3：产品评论的情感分析

- 任务： 确定产品评论的情绪
- 指示： 该模型应将评论分类为正面、负面或中性
- 提示公式： "对以下产品评论[插入评论]进行情感分析，并将其分类为正面、负面或中性。"

这种技术对自然语言处理、客户服务和市场研究等任务很有用。<br />![gpt18.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/21494320/1682220482685-195248f6-fb31-475b-a4c7-49b6e45f3b72.jpeg#averageHue=%23e0e6ed&clientId=u137130a2-d4e3-4&from=ui&id=XxaQh&originHeight=846&originWidth=1648&originalType=binary&ratio=2&rotation=0&showTitle=false&size=242306&status=done&style=none&taskId=u78f08fc2-5561-4490-afa9-4446b3220c5&title=)
<a name="UgsB4"></a>
## 命名实体识别提示 
命名实体识别（NER）是一种技术，它允许一个模型对文本中的命名实体进行识别和分类，如人、 组织、地点和日期。<br />要使用ChatGPT的命名实体识别提示，模型应该得到一段文本。应提供一段文本，并要求其识别和分类文本中的命名实体。<br />该提示还应该包括关于所需输出的信息，如需要识别的命名实体的类型（如人、组织、地点、日期）以及任何具体的要求或限制。<br />提示的例子及其公式：<br />例1：新闻文章中的命名实体识别

- 任务： 识别一篇新闻文章中的命名实体并对其进行分类
- 指示： 该模型应该对人物、组织、地点和日期进行识别和分类。
- 提示公式： "对以下新闻文章[插入文章]进行命名实体识别，并对人物、组织、地点和日期进行识别和分类。"

例2：法律文件中的命名实体识别

- 任务： 对法律文件中的命名实体进行识别和分类
- 指示： 该模型应该对人、组织、地点和日期进行识别和分类。
- 提示公式： "对以下法律文件[插入文件]进行命名实体识别，并对人、组织、地点和日期进行识别和分类。"

例3：研究论文中的命名实体识别 

- 任务： 在一篇研究论文中识别和分类命名的实体
- 指示： 该模型应该对人、组织、地点和日期进行识别和分类。
- 提示公式： "对以下研究论文[插入论文]进行命名实体识别，并对人、组织、地点和日期进行识别和分类。"

![gpt22.png](https://cdn.nlark.com/yuque/0/2023/png/21494320/1682239377391-73f4fd24-37f4-4e92-8400-90acd725c206.png#averageHue=%23f2f3f4&clientId=u137130a2-d4e3-4&from=ui&id=u794c2943&originHeight=1610&originWidth=830&originalType=binary&ratio=2&rotation=0&showTitle=false&size=315072&status=done&style=none&taskId=u6ea18c85-015a-4688-81a7-997d9162fea&title=)
<a name="fmZFH"></a>
## 文本分类提示
文本分类是一种技术，它允许一个模型将文本归入不同的类别或类别。这种技术对自然语言处理、文本分析和情感分析等任务很有用。<br />值得注意的是，文本分类与情感分析不同。情感分析具体侧重于确定文本中表达的情感或情绪。<br />这可能包括确定文本是否表达了一种积极、消极或中性的情绪。情感分析通常用于客户评论、社交媒体帖子和其他形式的文本，其中表达的情感很重要。<br />要使用ChatGPT的文本分类提示，应该向模型提供一段文本，并要求它根据预定义的类别或标签进行分类。提示还应该包括关于所需输出的信息，如类或类别的数量，以及任何具体要求或限制。<br />提示的例子及其公式：<br />例1：客户评论的文本分类

- 任务： 将顾客的评论分为不同的类别，如电子产品、服装和家具等。
- 指示： 该模型应根据评论的内容进行分类
- 提示公式： "对以下顾客评论[插入评论]进行文本分类，并根据其内容将其分为不同的类别，如电子产品、服装和家具。"

例2：新闻文章的文本分类

- 任务： 将新闻文章分为不同的类别，如体育、政治、娱乐等
- 指示： 该模型应根据文章的内容进行分类
- 提示公式： "对以下新闻文章[插入文章]进行文本分类，并根据其内容将其分为体育、政治和娱乐等不同类别。"

例3：电子邮件的文本分类

- 任务： 将电子邮件分为不同的类别，如垃圾邮件、重要的、紧急的等
- 指示： 该模型应该根据邮件的内容和发件人对其进行分类
- 提示公式： "对下列电子邮件[插入电子邮件]进行文本分类，并根据其内容和发件人将其分为不同的类别，如垃圾邮件、重要或紧急。"

![gpt18.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/21494320/1682236865912-b3ce670c-cd9c-4de5-a259-76e7a707210e.jpeg#averageHue=%23e3e8ec&clientId=u137130a2-d4e3-4&from=ui&id=k07Uy&originHeight=978&originWidth=1648&originalType=binary&ratio=2&rotation=0&showTitle=false&size=271798&status=done&style=none&taskId=u7af847c2-8010-4496-b583-5cfd9cb3821&title=)
<a name="zIKB0"></a>
## 文本生成提示
文本生成提示与本书中提到的其他几种提示技术有关，如零、一和少数样本提示、受控生成提示、翻译提示、语言建模提示、句子完成提示。<br />所有这些提示都是相关的，因为它们都涉及到生成文本，但它们在生成文本的方式和对生成文本的具体要求或约束方面有所不同。<br />文本生成提示可用于微调预先训练好的模型或为特定任务训练新的模型。提示例子及其公式：<br />例1：故事写作的文本生成

- 任务： 根据给定的提示生成一个故事
- 指示： 故事至少要有1000字，包括一组特定的人物和情节。
- 提示公式： "根据以下提示[插入提示]，生成一个至少1000字的故事，包括人物[插入人物]和情节[插入情节]。"

例2：语言翻译的文本生成

- 任务： 将一个给定的文本翻译成另一种语言 说明： 翻译要准确，要有成语
- 提示公式： "将以下文本[插入文本]翻译成[插入目标语言]，并确保其准确无误和符合习惯。"

例3：为完成文本而生成文本

- 任务： 完成一个给定的文本
- 指示： 生成的文本应该是连贯的，与输入的文本一致的
- 提示公式： "完成以下文字[插入文字]，并确保其与输入文字连贯一致。"

![gpt23.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/21494320/1682240422727-aa182822-3eaa-4475-9555-ac38f50a663d.jpeg#averageHue=%23e7e7e7&clientId=u137130a2-d4e3-4&from=ui&id=ucc4d93d9&originHeight=1232&originWidth=1648&originalType=binary&ratio=2&rotation=0&showTitle=false&size=328243&status=done&style=none&taskId=u62994334-874c-483b-9f3d-ac807e54ef4&title=)
