### Tell me about a time you failed / The biggest mistake you made / Miss deadline / Tell me a time you solved a complex problem

> → 对应的是 earn trust, customer obsession
>
> https://hbr.org/2023/01/how-to-answer-tell-me-about-a-time-you-failed-in-a-job-interview

- Situation：White CIDR，使用 Spark 防误报，预估数据量级后选择了网段展开法，初期开发时小规模测试有效。开发完成后最终测试宕机，分析日志确认数据量级超过预估（Reserved IP），导致整个方案无效。
- Task：尽可能减少错误带来的影响，包括排期等，重新实现方案。幸运的是在测试时发现问题，没有影响整个数仓的数据。
- Action：分析问题，在于没有对数据量级正确预估，重新设计基于前缀树的方案，预估排期需要额外的一周，及时与mentor沟通问题，一起讨论分析，并向项目组反馈了遇到的问题、新的方案和排期。基于之前的方案，已经足够熟悉大数据处理的流程，仅花半周就重新实现了更复杂性能更优的方案。
- Result：推翻整个方案重写，原本的两周排期延长至三周才上线，但新方案不仅能够解决亿级数据规模，也在保证常数级时间复杂度的情况下大量减少空间开销，获得了更好的效果。作为实习期间接手的第一个大数据需求，熟悉了整套开发技术，深刻体验了大规模数据带来的挑战。

### Take a risk, or do not have much time, to make a decision 

> → 对应的是 Bias for action, Ownership.
> 是行动优先，而且是要突出当仁不让，有责任自己能顶上的意识。比如customer找不到人刚好你在，你能主动做些事。

- Situation：短信验证服务夜间被攻击
- Task：需要迅速做出决定，避免损失
- Action：暂时关闭短信服务，避免持续发送垃圾短信并被扣费；查看日志，锁定UA与IP进行拉黑，同时通知负责短信验证服务的伙伴，加入熔断措施后恢复服务。
- Result：分析此次攻击的根源问题在于接口未引入防御措施，迅速开发并接入人机验证，防止再次被攻击。

### Tell me about a time when you had to work on a project with unclear responsibilities.

- Situation：作为校园技术团队队长时，积极参与每个团队正在开发的项目，即使自己在项目中不担任开发或是任何角色。<例子…>
- Task：在不担任明确角色时，更需要洞察问题，从更大的角度去观察整个项目的走向与发展。<例子…>
- Action：把握项目整体排期、人力协调、产品建议、review 开发架构与设计方案
- Result：

### Disagree with teammate or manager

> → 对应的是earn trust
> 这个很多人没对准，记住不是强行说服或者没什么理由的顺应别人, 为了customer或者最重要目的所以不同意别人。都是好说辞，和事佬的说法是偏题。
> 介绍背景，说出分歧。然后说自己怎么做，可以是讨论trade off, 可以是坚持高标准..等 结局一定说最后的选择是对的。 It proved to work well.

这个从头到尾都是编的

- Situation：校园论坛的APP端即将上线，由于功能很多，尚未开发完全。在暑假，PM 想要将功能全部开发完成后上线，认为开学时无法上线；我认为应该抓住新生入学的时机，配合团队招新进行推广，来达到更好的启动效果，未开发完成的功能并不影响核心使用。

- Task：
- Action：与产品组、运营组同学讨论，坚持自己的想法。当前产品的痛点便是活跃用户少，而开学的团队招新由于有学校官方的宣传渠道，覆盖面非常广，这样或许能够解决这个产品当前的困境；而附加的产品功能并不影响整个论坛的核心功能。最终说服其他同学
- Result：推广期间用户新增1000+，提前上线的收益大于功能不全面的负面影响

### Most challenging project

> → 对应的是hi‍‍‌‌‍‌‍‌‌‌‌‍‍‍‌‌‍‌‍‌ghest standards, think big
> 要讲自己怎么走出comfort zone, 当然舒适区本身也是一道题。
> 扣题，怎么复杂，是deadline 紧，还是技术复杂，你怎么做的，学习了新技术，use my priavte time to work on it 等等 最后说结果或者说通过这个process 你学到了什么

- Situation：大一暑假第一个独立负责后端开发并完成上线的项目
- Task：
- Action：经验不足 & 较短排期实现功能 & 第一次独立上线 & 团队合作
- Result：获得了3000+用户，遇到了许多平时遇不到的线上挑战，存在不足，留下经验

### Most proudest project

在寻找第一份实习时，开发了一个目前 2000+ Star 的开源项目。这个项目并没有什么太难的技术挑战，我认为这个项目成功的根源在于洞察了用户的需求与痛点。-> customer obsession

- Situation：从自身的体验出发，察觉当前并没有一个足够便利的简历编辑方案，要么需要熟悉冗长的 latex，要么在修改内容时需要不断手动地适配修改排版
- Task：编写简历是一个很费心力的事情，是否有一个能够让用户只需专注简历本身，无需关心排版或是语法的方案
- Action：开发了这个开源项目，基于当前主流的Markdown编辑器与定制化CSS，使得用户可以像平时写Markdown一样简单地编辑实时渲染的简历，并导出一份简历PDF
- Result：customer obsession，so…

### Tell me a time when you received negative feedback

> 先介绍背景,别人对你哪里不满意了, 简单说以下就行, 不要说很多别人如何对你不满, 也不要sugar coat 说自己其实没错。重点放在自己怎么解决这个问题，以及学到了什么。结果一定是好结果

- Situation：实习第一周接手一个配置复杂的项目，花了较多时间来配置环境并运行项目，~~没情商~~ leader 表示不满
- Task：
- Action：分析反馈，花费时间较多的原因是没有及时与 mt 沟通及寻求帮助。
- Result：在后续的项目需求开发中更加注意把握时间与及时沟通，高效地完成了较多需求，重新获得 leader 的信任

### Tell me about a time when you gave a simple solution to a complex problem / Find a new way to do something

> 这个问题一定要让面试官信服你说的例子。先说一般的方法很耗时，自己找到一个方法很快就完成并且Deliver 了，而且很稳定，没出过问题，结果要是好的。

- Situation：校园巴士，校方需要开发包车预约功能
- Task：需要权衡当前的解决方案，避免非必要的人力支出
- Action：分析整体需求，该模块需要实现提交预约、可视化管理等功能，需要产品设计、UI设计、前后端预计6人周。但另一方面，提交预约、可视化管理这两个功能实际上完全可以由接入外部问卷实现，用户只需跳转提交问卷，校车方管理问卷后台即可。接入问卷的优势是稳定且功能全面，同时减少人力投入。与项目组商量方案可行性并与校方对齐。
- Result：满足用户需求，且减少了开发与维护的人力开销。最终只消耗了1人周时间进行校方对接与问卷接入