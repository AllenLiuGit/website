+++
title= "敏捷实施经验贴"
subtitle= '关于敏捷路上那些大大小小的"坑"'
date= "2018-04-08"
author= "刘海螺"
tags= [
    "敏捷"
]
categories= [
    "技术类"
]
description= "敏捷转型并没有那么简单。敏捷是一个很强大的工具，运用得好确实可以收到很好的管理和交付效果，但是运用得不好，很可能就会事倍功半" 
img= "/img/blog/agile-implementation-experience/agile-1.jpg"
+++

摘要：敏捷转型并没有那么简单，不是把那一套运作模式运作起来就可以，毕竟每个公司的情况都有所差异，仅仅把敏捷那一套运作模式照搬过来是远远不够的。对于管理者来说，希望通过敏捷提升软件交付的效率和质量，并且希望通过敏捷转型打造一个高效、学习型的团队。其实，敏捷是一个很强大的工具，运用的好确实可以收到很好的管理和交付效果；但是运用的不好，很可能就会事倍功半。本文将总结在过去的一段时间里，我们自身在敏捷转型过程中踩过的坑，希望对大家在做敏捷转型或者实施的有一定借鉴意义和帮助。

![](/img/blog/agile-implementation-experience/agile-1.jpg)

随着互联网、大数据的发展和成熟，包括新零售等概念的提出、探索和落地，越来越多的企业开始进行敏捷转型，在软件开发过程中采用敏捷的方式，期望可以提升开发效率，改善交付质量。敏捷也不再局限于互联网行业，很多传统行业——包括银行、保险、电信、零售等等也逐渐开始认同敏捷的开发方式和流程，在企业内部的系统开发过程中把敏捷与原有的流程相互融合，以更好地适应高速、快节奏所带来的不确定性，进一步提升IT部门和系统更好地服务企业战略目的和满足市场需求的能力。

对于管理者来说，希望通过敏捷提升软件交付的效率和质量，并且希望通过敏捷转型打造一个高效、学习型的团队。其实，敏捷是一个很强大的工具，运用的好确实可以收到很好的管理和交付效果；但是运用的不好，很可能就会事倍功半。

![](/img/blog/agile-implementation-experience/agile-2.jpg)

## 为什么敏捷很好，但是我们却很难落地？

本文将总结在过去的一段时间里，我们在转型过程中踩过的坑，以作前车之鉴。也聊聊在转型过程中，哪些优秀的实践可以尝试，走上渐进变革的道路。

1. **敏捷是不是可以缩短项目周期，或者说“敏捷就是快”?**

    在接触敏捷之前，大家对敏捷都是一知半解，更多的停留在字面意思的理解上：“敏捷就是快”。一旦有人觉得不快时，就会发出质疑：我们的敏捷做对了吗？
    其实，敏捷并不意味着“快”，“敏捷”在百度字典中的解释是“反应迅速快捷”。在软件开发中，敏捷是使用各种管理的手段（例如，3个角色，5个事件）来确保软件开发人员能够对于外部或者内部的需求或者变化能够迅速的做出反应，保证软件系统的功能或者其他特性能够满足市场或者用户的要求。

    敏捷模型和瀑布式开发模型是对立的，瀑布式开发模型主要是“按部就班”的进行需求调研、系统设计、详细设计、功能开发、测试、上线，以及运维等，我相信大家对于瀑布式开发模型非常熟悉，现在大部分的甲方IT部门或者乙方公司都采用这样的交付管理手段。同样，大家和我也有相同的感触，系统的需求可能不断地在变化，或者是调研不清楚，亦或设计不能够满足用户需求，没有别的选择，只能硬着头皮加班加点修改，呵呵，这也是程序员经常吐槽的地方…本质上，瀑布式的开发模型是“非常害怕变化的”，一旦有“任何的风吹草动”整个项目组都紧绷神经，进而通宵达旦；而敏捷模型则是“拥抱变化的”，敏捷拒绝“一成不变”，崇尚软件系统功能“持续增强”，它是把整个软件交付周期“拆”成一个一个小的瀑布模型，每个瀑布模型持续一周或者两周，我们把它称作“冲刺”，在每一个冲刺中都要进行需求的讨论和确认，都要对交付的成果进行评审，并且项目组还要进行自身的反思和回顾，这样即使变化来了，我们通过敏捷模型能够“轻松的应对”。

    有一个例子，共享单车刚刚起步的时候，市场上共享单车的公司不多，共享单车的创新是通过互联网和手机支付的手段，帮助和方便用户完成 “最后一公里”的交通出行。起初共享单车业务逻辑是一辆自行车的成本大约200元人民币，设计寿命是3年，用户骑行一次大约需要支付1块钱，一辆自行车一年差不多可以收回200元的成本，第二年和第三年就可以实现盈利。但是，没有想到不到半年时间，其他的共享单车如雨后春笋般的出现，而且价格更低，并且有各种优惠活动。第一个吃螃蟹的共享单车企业原来的商业模式已经失效，但是他们发现他们有一个很大押金池子，如何有效的利用这笔资金成了他们“最后的救命蒿草”，他们的软件系统功能如何支撑“有效的利用这笔资金”成为了他们迫在眉睫要解决的问题。如果采用瀑布式的开发模型，按部就班，“3个月或者半年之后交付”，可能市场又不知道发生了什么变化。而敏捷的模型则可以在一定程度上很好的应对这样的突发情况。

    总之，敏捷的核心是快速地应对变化，本质上，它并不能缩短软件交付的周期。有时候我们感觉“敏捷快”是因为它能够快速的响应市场或者用户的需求变化，而不是以前瀑布模型中，用户和项目组都为“这个功能是这个样子的，而不是现在开发成的这个样子”而相互的扯皮，推诿…

    当然，我们在瀑布模型中也会主动或者被动地使用到“敏捷”，用户提出需求变更，今天晚上或者明天就可以看到结果。

2. **之前的项目管理一般先出文档，跟着文档来开发，现在实施敏捷之后，大家主要是以沟通为主，有些需求不是一定要有文档才能开发，可以说在开发过程中有些需求通过沟通取代了文档。是不是敏捷就不需要文档了？**

    在敏捷宣言中四个核心价值观：

    * 个体和互动 高于 流程和工具
    * 工作的软件 高于 详尽的文档
    * 客户合作 高于 合同谈判
    * 响应变化 高于 遵循计划

    其中，“工作的软件 高于 详尽的文档”，对于这句话的解读，以及根据实践获得的经验，并不是实施了敏捷之后，就不需要文档，俗话说“好记性不如烂笔头”，有很多的文档，还是必须要做的，例如功能设计文档，DDD设计文档，UI设计文档等。从敏捷的思路来说，只是认为相互沟通的效果会比文档去理解的效果要好，所以大部分的东西主张以沟通为主，文字为辅，如果沟通可以解决，那么文档如果没有什么附加价值就不写，但是如果它还是很有价值的，比方说功能设计，是以后需要看的，那就要写，所以做与不做看价值。

    有价值的我们做，没价值的不做，举个例子，某银行去做敏捷转型之前，非常重视文档，每个文档都要思考很久才提交，他们一个项目的立项到结项要写55份文档，实施敏捷之后，从内部把文档裁剪到17个，从55到17个，而不是从55到0。那保留些什么，不保留什么，要看这些文档是怎么用的，有没有价值。

    所以我们要自己判断一下要的是什么，不要的是什么。总的来说，你用了敏捷之后不是没有文档，而是把没有价值的文档删掉。

    根据我们的经验，文档的更新也是一个敏捷和持续的过程，例如UI设计文档，我们会不断地与用户或者利益相关者沟通UI界面，每个冲刺都要沟通碰撞，直到某一个功能的设计满足美观、易用的要求。在这过程中，我们的UI设计师会根据反馈设计出不同的版本，甚至前端工程师要先实现这些UI设计，根据实践的效果不断地调整，直到项目组满意，再跟用户沟通，如果用户不满意，我们回来继续修改，就这样不断的“反反复复”，持续地更新。

3. **敏捷倡导以沟通来代替文档，但是团队不是一成不变的，有成员走有成员进，这时候我们如何要做好经验的传递？**

    新人来直接看文档就可以很快了解融入到团队里面是很难的，大部分的敏捷团队是通过沟通融入进去的。

    比如：已经写好了一个文档，已经进行开发，突然间需求变更过来了，大部分的时候，需求突然变更，是不会先改文档再开发的，结果导致文档跟开发的情况不一致，新人看完文档后还是要再去理解代码，所以我们假设只要文档写好，后边的交接理解没有问题，新人都能理解文档里的内容，是不对的。

    团队人员的流动不会全部流动，可能是十个里面两三个的概率，团队的其他人和新人沟通交流就好，如果有些比较重要的系统设计等，那就把系统设计重要的几页写下来，比方说接口，如何调度等很紧要的东西写下来，不需要面面俱到。开发结束写文档，也不需要担心新人无法融入。

    如果真的觉得我们缺少了某些文档，应该在团队里说明，我们的开发过程应该做那份文档，比方说比较完整的测试用例，完整的需求场景描述等这些文档。

    还有一个做法，这个我们在新老交替经常使用，就是结对编程。我们会安排“师傅”带着新人，一起做一段时间，在这段时间，“师傅”会将我们这边的基本情况，系统架构，功能，技术栈，规范等教给新人。并且会分配给他一些编程的工作，这样持续1-2周左右，新人基本上能够融入到现有的团队。

    总之，通过纯文档的形式做新人的培训是很难的，应该采用沟通 + 文档的方式。

4. **敏捷过程中还是存在传统项目中项目经理这个角色？**

    如果用的是scrum模型，是没有定义项目经理这个角色，这个职责被PO和scrum master分摊掉，如果不是用scrum的模式，比如用看板模型，就没有说不要项目经理，而是继续引用现有角色。从广义的角度来说，敏捷中“没有项目经理”这句话不是完全正确的，但如果你用敏捷scrum模型，确实没有定义这个角色，但只是敏捷scrum模型而已，敏捷还有n多模型，项目经理的角色剔除或者不剔除要看我们使用的敏捷模型是什么。

    根据我们的经验，Scrum模型中可以没有项目经理，这个职责被PO和scrum master分摊掉。PO主要对产品负责，他以产品为引导驱动整个开发Team，类似“连长”“排长”的角色；而Scrum Master则是对整个软件生产经营活动中的“规章制度”“流程”等负责，类似“政治委员”的角色。但是 ，我们在实际的操作过程中，还需要另外一个角色“技术负责人”，虽然说Scrum模型中定义的开发团队，应该是一个自组织、跨职能的团队，但是对于产品的架构、系统设计、开发规范等，都需要一个有经验的技术牵头完成，包括代码质量保证等，我们尝试过没有这样的一个人（说起来都是泪），最后前后端代码的质量非常差，而且后端出现了严重的性能问题，原因就是没有一个相对来说有一定技术权威的人，来配合项目组管理整个技术设计和规范。敏捷的转型本质上是要为每一个人赋能，但是实际情况是，项目组内部的人员能力、经验等会出现参差不齐的情况，如果是按照Scrum模型教科书式地推进，大家认为开发团队是一个“自组织、跨职能”的团队，让他们“完全自我管理”，那么就特别容易失败。所以，不管是使用哪一个模型都是需要根据实际的情况来操作，而不是完全教科书式的转型，但是刚开始的时候总是有一个摸索期。

5. **多组之间依赖性强，敏捷小组之间的协调，有一些团队是依赖于某一个团队的，这个团队自己的任务和故事还没进行下去的时候，可能就要帮其他团队的任务，就阻塞自身的敏捷进行，团队之间的协作应该怎么更好去处理？**

    对于跨组协调，有很多模型可以使用，比如scrum的标配scrum scrum模型，scrum scrum模型能在跨组上面进行定期的沟通，以便沟通之后能尽快解决团队之间存在的问题，如果没有这样的机制，进行定时的沟通；请人吃饭，搞好关系也是可以的，呵呵…

    有跨组机制只是多一个方法和工具，无论你用新模型还是旧模型，跨组中肯定会存在协调问题。用了敏捷模型后，会给你一个沟通渠道，比如定时的会议，跟其他团队去协同沟通。在选择跨团队协作机制的时候，简单够好用就可以，不用太复杂。

6. **与传统的项目管理方式对比，客户方习惯了将开发拆分到任务层面并指定deadline，而且传统的项目往往瀑布式比较多，会有大量的文档，当以用户故事的方式驱动开发，客户方业务只能看到用户故事，看不到具体内容，心中没底，总是存在质疑。这样的情况，我们应该如何和客户进行沟通交流？**

    首先，我们要看当客户是不是很了解，敏捷方法的推行是客户方提出，还是我们推荐的。如果是客户提出的，必然会按照这个方法去做，如果是我们主张，我们团队有能力完成这样的交付，我们就要给客户解释，消除客户的质疑。

    我们可以把以前的工作方法写一个flow给他，新的方法也写一个flow给他，进行一个简单演示，之前的flow，从需求到PRD，PRD到设计的一系列流程，以前的flow流程，和新的flow进行对比，敏捷化之后我们都会有与之对应或者替代的环节，比如计划会对应需求到PRD这一过程，可能以前的flow你会看到PRD，现在敏捷化之后被用户故事替代，其他也是一样，你虽然看不到之前的，但是依然可以从某个方面获取到进度以及其它方面需要的信息。

    总体来说，遇到这种情况，我们自身先学一点这方面的能力，实施的技术人员和业务人员如果没有完成敏捷相关培训和教育，敏捷推行的时候，我们要帮助客户简单了解敏捷的意义，推行敏捷能够带来什么样的好处，但是归根到底我们是做交付的，未必能给出一个很好的解释。要让客户知道我们之间少了一方沟通交流的人来解释敏捷实施过程遇到的问题，关于敏捷的教育培训，客户方自身那边安排一下会更好。

    总的来说，敏捷转型不是一蹴而就的，而是一个持续的过程，在这过程中会有各种各样的问题出现，而且不同的公司，不同的文化，遇到的问题也不尽相同。遇到问题很正常，我们只要“咬定青山不放松”，在问题当中不断的解决问题，就一定能够发挥敏捷真正的威力，不断提升软件交付的效率和质量。

