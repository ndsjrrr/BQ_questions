# BQ问题准备

Q：startup如何来明确谁是PM，CEO，还有我的上司？和一个Tech Manager。这几个的顺序如何安排呢？ 

### 0 所有能用的故事汇总

1 有一个需求是，将之前手机端的一个新增tags 和 删除tags 的feature给做出来。(体现的Ownership)

2 修改交互体验。将 点击 勾选的交互优化，升级成为 允许卡片拖拽功能。(体现的Ownership)

3 【gather information and respond quickly】短时间之内学习（提升AI生成质量）1 Prompt Engineering 2 Multi-Agent System 3 Fine-tuning (体现的是Learn and Be Curious)

4 在短时间之内做出选择（take calculated risk) 体现的是 bias for action

- 【ST】组长休假了，product launch date是在一周内。目前已经通过完beta测试，临时加入了一个tiktok log in的需求。然后有一个Tiktok Developer申请的时候，无法通过。在被rejected的记录里要求的是，需要有一个在登陆时候的 Term of Services 与 Privacy Policy 两个内容。但是我们目前并没有。
- 【A】我当时纠结了很久。xxx。担心
  - 1 无法赶在正常的date时候 launch；
  - 2 UI来不及设计。
  - 在经过和PM重新沟通priority, 将部分在正式版本准备发布的功能明确。
  - 3 最后决定采用在登陆页面的页脚加入两个超链接。这一个办法，不仅不需要担心太多UI的设计，同时也可以避免对原有登陆页面做更多的代码修改。在其他页面也可以看到这个页脚。
- 【R】 最后改完后立即提交申请，通过了Tiktok审查。得到了组长的表扬。

5 没有足够的时间（bias for action) 【感觉不太能用】

- 【ST】：有一次，只有不到2周，我们的老板和PM要求我们完成一个Project页面的前后端对接。这个feature设计到和前一个页面Drivce的Card类之间的交互。
- 【A】 Actions: 由于时间非常紧张，导致我们在考虑这两个依赖关系的时候，并没有考虑全所有的情况。业务代码的逻辑也越来越复杂。导致后来没有想清楚。
  - Break Down
  - Assign 给别人
  - 加班 （稍微提一下）a little bit overtime
- 【R】 Result：我们采用了简化的方法。将原本n to n的两个实体，变成了1 to n的依赖，避免了之前的相互依赖关系而导致的corner cases不可控的情况。
- Lesson：我学习到了，每次在接到需求的时候，需要对
  - 1 需求进行合理的评估，包括确定各种corner cases。
  - 2 对时间需要据理力争，需要和pm沟通好最后所需要的时间。

6 【long term vs short term】

- 【ST】有一段时间，公司业务扩张很快，有欠下了许多技术债。代码的各个模块之间耦合度非常高。
- 【T】此外，在这段时间中，PM也需要我在两周的时间内，上3个新的feature。当时我考虑到，加的feature如果太多，太紧急，上线以后很容易会出问题。
- 【A】我重新和PM沟通，确认好priority。PM把这几个需要有的feature的重要程度排序。我确认，认为先把原有的代码进行重构，我主张先尽快把原有的代码进行重构，再赶前2个新的功能。把最后一个留到这次版本更新之后。
- 【R】Outcome是，虽然这3个feature只完成了两个，但是后期上线了以后，并没有出现任何需要返工才能完成的问题。此外，在实现第三个功能的时候，由于代码比较工整，结构清晰，在实现第三个功能的时候，并没有花过多的时间。
- 【L】我现在还是主张认为，需要定期解决之前遗留的代码问题，而不是盲目赶工。赶工只会导致花费更多的时间，在测试出现问题以后，再返工。

7 【Tight DDL / work under pressure】

- 【ST】原product launch date是xx。但是在Beta test的时候，customer临时提出新的feature：【希望要一个类似chatgpt的UI，而不是一个普通的按钮 -< pop up window -> edit】。但是PM又不想delay launch date。
- 【A】1 和pm沟通 proritization，确保最紧急的任务优先级定期设置好一个checkpoint;
  -  2 和tech lead开会，确保没有block其他人给任务预留好足够的时间用来做testing + plan B（直接上线优化前的版本）。
  - 3 和tech manager沟通，尝试加入新的resources（UI同事）来一起解决这个问题。
- 【R】最终customer对我们的产品非常满意，得到了赞许。【不会编】

8 【Critical Failure】

- 【ST】在我第一次实习的时候，有一次在开发一个vue前端页面的时候，涉及到流式输出的案例，由于我对这个内容不太熟悉，在mid-point milestone的时候严重behind。
- 【A】
  - 于是我在这次miss了之后，主动和我的manager制定好了新的plan，以及三个milestone，在每个milestone都check in 不会miss
  - 此外，我还向他询问要了更多的学习资料和博客来去补足
- 【R】在最终提交PR的时候，我的这个feature按时间完成。获得上级的认可。

9 【类似的 你最大的weakness】

- 我遇到过failure是由于前期准备的时间太多，导致最终我的项目miss ddl。
- 在实习的时候，vue做流式输出的时候。
- Lesson Learn：1 前期学习不需要系统学完，应该从做中学（make decision without enough information）2 定一个时间，专门找一个senior sde who knows the taks go through 来speed up这个过程。3 一定做好计划，分清除 subtask。每个subtask设置一个checkpoint，检查，确保不会miss。



10 Receive Negative Feedback

【ST】我的tech lead在刚开始的时候，给我做code review完了以后，提到过我的代码风格有问题，并且我的extendibility较差。

【A】我在收到feedback以后，1 主动询问有没有一些推荐的书籍资料。medium的几篇文章 + clean code。2 学习senior sde的代码是如何写的。此外，我还主动和其他几个junior sde一起互相进行code review。not only can i learn from my own mistakes, but also I can learn from theirs' mistake as well

【R】在几个月之后，我再也没有收到过这个feedback。并且，i was told from my senior sde that I was the quickest learner among all the junior sdes.





11 Conflict with Teammates - 类似于我的这个[long term vs short term]的这个逻辑

- 【ST】有一段时间，公司业务扩张很快，有欠下了许多技术债。代码的各个模块之间耦合度非常高。此外，在这段时间中，PM也需要我在两周的时间内，上3个新的feature。

我和我的另一个enginner起了冲突。

他认为，我们应该先把任务完成。后面再考虑refactor的事

我认为，我们应该先尽可能refactor，不然long term来看，代码很难维护，新的featrues再加进去就更加乱了。

【Actions】

1 Open discussion

- 和同事交流，Had a conversation with teammates, to fully understand her concern. Time is important时间很重要

2 Data-driven Explanation【对比两个方法的pros & cons】

- Expressed my view about the project, want to make the system better and closer to the actual industry environment so the work is meaningful. 
- Also shared some of my examples from my previous git status, showcasing that the change and optimization can improve the performance!

3 Proposing a Compromise

- Banalacing our priorities, only optimize the part that are practical and easy to optimize without spending a lot of time rewrting the whole features again.
- Decouple the code using a message queue. 
- For the other part, we can optimize them later

【Results】

After reaching a agreement, I quickly implement the changes. The optimization took us about 2 days, which did not affect our progress too much.

The decoupled process improve the overall system realiability and both my teammate and I were satisfied with this outcome. We did not affect our plan too much, and we also enhanced our system scalability.



当时我考虑到，加的feature如果太多，太紧急，上线以后很容易会出问题。

- 【A】我重新和PM沟通，确认好priority。PM把这几个需要有的feature的重要程度排序。我确认，认为先把原有的代码进行重构，我主张先尽快把原有的代码进行重构，再赶前2个新的功能。把最后一个留到这次版本更新之后。
- 【R】Outcome是，虽然这3个feature只完成了两个，但是后期上线了以后，并没有出现任何需要返工才能完成的问题。此外，在实现第三个功能的时候，由于代码比较工整，结构清晰，在实现第三个功能的时候，并没有花过多的时间。
- 【L】我现在还是主张认为，需要定期解决之前遗留的代码问题，而不是盲目赶工。赶工只会导致花费更多的时间，在测试出现问题以后，再返工。



12 稍微有一点这个 make decision without enough data

【S T】接到一个task，关于如何进行Ai生成内容的优化。我当时的时间，只有2周，没有办法完全test出所有的方法并进行implement。

【A】我首先用3天进行research，发现一共有3种办法。1 prompt engineering 2 multi-agent  3 fine-tuning来去完成。由于这个任务时间比较紧急，没有时间来去做一些test dataset并且跑几个小的demo来去看这几个的performance。

- 定性评估美中方法可能会有的时间成本和潜在收益；
  - 1 Prompt  Engineering , 周期短+灵活，且不需要大量的GPU成本。缺点是可能提升效果有限
  - 2 multi-agent : 周期中等，需要设计agent架构和交互逻辑，效果可能显著但是不稳定
  - 3 fine-tuning: 周期比较长，需要准备大量的数据进行训练，且效果可能比较好，也有比较大的风险
- 考虑到两周的时间，我首先快速使用这个prompt-engineering的方法做出一个可用的方案。并且在剩下的4天时间内，实施了一个比较简单的Multi-agent workflow。保证在完成之前，首先有一个可用的解决方案，并且也有一定的优化空间。

【R】：

1 在有限时间内完成了交付，prompt engineering的方法提升了10%的性能（survey: average user rating) 

2 虽然这个multi-agent的方法并没有完全实施完，但是也作为一个非常potential的demo。可以后续进一步优化。这个demo获得了tech lead的认可。



13 Weakness

我认为我的一个主要弱点是过于注重details，尤其是在前期准备阶段投入过多时间，这有时会影响项目的最终交付。

- 【ST】在一个需要实现新功能的项目中，我被分配负责开发一个基于用户内容的推荐系统，这是我之前没有直接经验的领域。我需要在六周内设计并实现这个模块。
- 【A】由于对这个领域不够熟悉，我决定先深入学习相关技术和Best Practice。我花了将近三周时间阅读文档、研究论文和分析类似实现方案，希望找到最优解决方案。当我终于开始编码时，我发现时间已经所剩无几，而我对实际实现中的挑战认识不足。虽然我加班加点工作，但最终还是没能在截止日期前完成所有功能，导致项目延期。这次经历给我上了宝贵的一课。
- 【R】通过这次失败，我学到了几个重要经验：不必在开始前掌握所有信息——应该采取"边做边学"的策略，即使信息不完整也要开始行动尽早寻求有经验同事的指导项目开始时就制定详细计划，将大任务分解为小的子任务，并为每个子任务设置检查点



### 1 proud project

【ST】我最proud的project是我在CoScribe AI工作时间做的一个multi-modal RAG system. RAG stands for Retrival Augmented Generateion. 它需要首先将各种来自于不同的modal的文件，such as audio, video, pdf... 等给预处理成文字，然后存入这个Vector DB中。

我的这个项目比较chanllenge的地方在于，其retrival的部分需要不断进行优化，才能匹配出更精准/相关的结果，才能更好地匹配出信息。之前的做法是 仅通过Vector Similarity Search itself。但是这个对于一些需要精准匹配关键字的场景并不擅长，可能会丢失一部分信息。于是，后续，使用了hybrid search, a keyword-sensitive sementic search approch, 来combine both vector search and keyword search algo to take advantage of their respecive strengths while mitigating their respective limitations.



【A】后面，我通过 1 看 langchian的 官方文档，做了 Hybrid search，并且进行reranking，

【R】最终context recall rate 提高了15%。并且这个软件的DAU improves by 20% after in the updated version.

【过程中，遇到的问题是：retrival准确率低。如何优化，尝试了不同的方式；有几个方式不太好，最后通过多路召回reranking产生最optimal效果。】Business impact, User Survey shows that 两种方法的pros + cons有什么可以继续优化的blabla。



### 2 tight ddl(Deliver Results)



### 3 critical feedback



### 4 help others 



### 5 decide incomplete with data 



### 6 learn new things 



### 7 Customer Obsession



### 8 make a mistake







# Sample Solution：

## Disagreement with others

1 核心观点：冲突 - 坚持自己的看法 / 妥协 - 行动过程 - 最终结果

- Have a backbone / Disagree and Commit 
  - 围绕 坚持 - 冲突 - 妥协
- Earn Trust 
  - 沟通 - 化解分歧 - 让对方相信你的想法
- Are Right, A Lot
  - 如果过程中涉及到你的抉择，判断，复盘

#### Situation:

我的看法：多做一点优化

他的看法：Quick finish 不做优化



#### Task：

我想学习更多，而不是简单把事情做完。

我需要convince 他这些optimization是值得extra effort的。



#### Actions：

1 Open discussion

- Had a conversation with teammates, to fully understand her concern. Time is important

2 Data-driven Explanation:

- Expressed my view about the project, want to make the system better and closer to the actual industry environment so the work is meaningful. 
- Also shared some of my examples from my previous git status, showcasing that the change and optimization can improve the performance!

3 Proposing a Compromise:

- Banalacing our priorities, only optimize the part that are practical and easy to optimize without spending a lot of time rewrting the whole features again.
- Decouple the code using a message queue. 
- For the other part, we can optimize them later



#### Results:

After reaching a agreement, I quickly implement the changes. The optimization took us about 2 days, which did not affect our progress too much.

The decoupled process improve the overall system realiability and both my teammate and I were satisfied with this outcome. We did not affect our plan too much, and we also enhanced our system scalability.



优化的地方：

developed an individual coding sandbox, decouple workflow....

没有优化的：

some other more classes that might affect the system performances.



