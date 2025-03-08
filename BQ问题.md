# BQ问题

下面一共7类14个问题，每一类你选一个问题就可以。准备一下答案，准备好了咱们可以约个时间一起看一下。有时间的时候把简历发给我。感恩节快乐！

1 Tell me about a time when you worked against tight deadlines and didn't have time to consider all options before making a decision. 

How much time did you have? What approach did you take?  What did you learn from the situation? 

- ST：有一次，只有不到2周，我们的老板和PM要求我们完成一个页面的前后端对接。这个feature设计到两个实体之间的交互，相互依赖关系。
- A: Actions: 由于时间非常紧张，导致我们在考虑这两个依赖关系的时候，并没有考虑全所有的情况。业务代码的逻辑也越来越复杂。导致后来没有想清楚。
  - Break Down
  - Assign 给别人
  - 加班 （稍微提一下）a little bit overtime
- R: Result：我们采用了简化的方法。将原本相互依赖的两个实体，变成了一个一对一的依赖，避免了之前的相互依赖关系而导致的corner cases不可控的情况。
- Lesson：我学习到了，每次在接到需求的时候，需要对1 需求进行合理的评估，包括确定各种corner cases。2 对时间需要据理力争，需要和pm沟通好最后所需要的时间。



Tell me about a time when you had to gather information and respond immediately to a situation. What was the outcome? Would you have done anything differently?

【Work in Ambiguous Situation】

看看stakeholder是谁 -> gather information



- Situation Task：老板PM希望我们能够在1天之内，解决一个AI生成质量较差的问题。
- Actions：
  - 给自己3个小时的时间内做尽可能多的调研，搜集有关如何能够提升AI生成质量的论文与博客。并产生几个可以优化的策略：prompt engineering(CoT), multi-agent system, fine-tuning ;  
  - 用1个小时，和技术经理确认好技术路线，由于时间紧急，优先采用最简单的方法prompt engineering来完成。 - 用3个小时修改prompt，并提交任务。- 后续还加班3个小时，也快速搭建了一个简易的multi-agent system来改进生成质量。
- Result ：能够在规定的时间内完成任务，并且评估后认为生成质量有所改进。后续给老板将加班后的成果也发给老板，老板对结果十分满意，给我表扬。



2 Give me an example of when you were able to anticipate a customer's need with a solution/product they didn't know they needed/wanted yet. How did you know they needed this? How did they respond? 

- 有一个feature：我们有一个多选的功能，将点击多个文件进行多选，然后点击 移动到  xx 文件夹中。后面，我修改成了可以在web中可以拖动到xx文件夹中。一开始测试的时候，之前多选的方案，他们也没有提出有使用上的问题。｜｜ 之所以会提出这个需求，是因为自己亲自体验后，发现这个UX不太顺手，因此就修改了。现在客户都非常喜欢这个新的拖动文件夹的方案。

Give me an example of a time when you asked for customer feedback. How did you use that feedback to drive innovation or improvement? How did the customer respond?

- 



3 Tell me about a time when you not only met a goal but considerably exceeded expectations. How were you able to do it? What challenges did you have to overcome? 

- ST：有一个需求是，将之前手机端的一个新增tags 和 删除tags 的feature给做出来。
- A：我不仅仅把这个需求实现了，同时也在想，如何才能更好地，将UIUX体验做的更好。原来的增加操作是，按右侧+按钮，弹出一个输入框，输入tags内容。长按后，可以删除该tags内容。1 我加入了 “修改tags”的操作。并且允许用户短按可以修改tags的内容。2 ；长按时，首先进入编辑状态，加入了“允许用户对tags进行排序”，并且在编辑状态时，右上方有一个小的 删除按钮，可以完成tags的删除操作。
- 在这个过程中遇到的挑战是，需要找到合适的库，来完成 编辑状态的动画效果，才能让用户感知到进入了编辑状态，并且可以编辑且删除原来的tags。
- R：收到了PM和UI设计师的表扬，认为我的这个设计更完善。

Give me an example of a time when you were able to deliver an important project under a tight deadline. What sacrifices did you have to make to meet the deadline? How did they impact the final deliverable? What was the final outcome?





4 Tell me about a time when you were trying to understand a complex problem on your team and you had to dig into the details to figure it out. 

Who did you talk with or where did you have to look to find the most valuable information? 

How did you use that information to help solve the problem? 

- 想不到 不知道如何回答
- 没有真实遇到过很复杂的问题， 需要编写吗？
- 





5 Tell me about a time when you worked to improve the quality of a product/service/solution that was already getting good customer feedback. 

Why did you think it needed improvement? How did customers react? 

- 【同3】

Tell me about a time when you had to make a decision between standards and delivery. What tradeoffs did you have make? What was the outcome? Knowing what you know now, would you have done anything differently?

- 【同1】



6 Describe a time when you took on work outside of your comfort area. How did you identify what you needed to learn to be successful? How did you go about building expertise to meet your goal? Did you meet your goal? 

- 学习how to led a team. 我后期需要和团队密切协作，并带领以为暑期intern一起完成工作。因为我并没有带人的基础，而且我并不擅长管理。为此，我学习了许多管理知识。
- 我通过读书，来明确一名好的技术管理需要怎么做。
- 最终，带领这位intern，爬取tiktok上的data，并进行数据分析，为后续接入RAG做基础。他在我的带领下，学习到了很多data处理的知识，并且最终很好地完成了这份工作。



Give me an example of a time when you explored a new or unexpected area of an existing space. Why hadn't this been explored already? Why did you move forward? What were the results or what was the impact?

- 



7 Tell me about a time when you took on something significant outside your area of responsibility. Why was it important? What was the outcome?

- 

Tell me about a time when you made a hard decision to sacrifice short term gain forsomething that would create long term value for the business. What
was the outcome? Knowing what you know now, would you have done anything differently?

- 有一段时间，公司业务扩张很快，有欠下了许多技术债。代码的各个模块之间耦合度非常高。此外，在这段时间中，PM也需要我在两周的时间内，上3个新的feature。当时我考虑到，加的feature如果太多，太紧急，上线以后很容易会出问题。因此，我主张先尽快把原有的代码进行重构，再赶这3个新的功能。
- Outcome是，虽然这3个feature只完成了两个，但是后期上线了以后，并没有出现任何需要返工才能完成的问题。
- 我现在还是主张认为，需要定期解决之前遗留的代码问题，而不是盲目赶工。赶工只会导致花费更多的时间，在测试出现问题以后，再返工。





































