
# DaoCloud助力黑客马拉松

2015年夏天，DaoCloud与七牛、云雀、数人科技等公司联合主办了中国首届Docker黑客马拉松。我作为参赛成员的一份子，也体验了Docker中国社区与Golang中国社区的活跃，来自ThoughtWorks、360、UnitedStack等专业团队都参与了，可以说是Docker近年来在国内快速发展以及得到大量开发者肯定的一个Snapshot。

我们团队由UnitedStack和Curiousity中国的成员组成，一大早就来到了比赛现场，DaoCloud和其他工作人员热情安排了早餐。至于黑客马拉松的过程可谓是枯燥而又有趣，各个团队积极讨论自己项目的设计，不时也会去其他小组搭搭讪，互相交流公司技术上的发展。期间DaoCloud社区经理Fiona和其他技术人员过来提供了容器镜像托管的服务，当然我们就用上了，和官方的Docker hub类似，只需在界面上选择项目就可以Automated build了，然后提供比官方更快的下载速度。一直忙活到晚上十点，活动组织方甚至安排了住宿，让“黑客们”可以好好准备第二天的正式演示。

当然我们并没有闲着，我们要实现的是国内首个基于Docker的持续集成系统，整个系统包含前端的UI、后端的执行测试的worker，当然还有分布式的调度系统和复杂的数据交互和存储。要实现这些，白天的12个小时显然是不够的，我们回到酒店后马不停蹄地继续加feature、修bug、补充document，大家最后看到的archci界面和kubernetes-worker都是在凌晨的北京完成的。最后我们的现场演示也很成功，一个“基于Docker比取代Jenkins比Drone更好的CI系统”也就是ArchCI，底层使用Docker运行测试，上层可以结合kubernetes分布式地调度，而且提供类似Travis的管理界面，我们一个晚上做了6个repository，当天还购买了域名上线到archci.com，对Docker和CI感兴趣的同学不妨关注一下。

补充一下，DaoCloud提供了免费的镜像托管服务，ArchCI的镜像也托管在这里 https://www.daocloud.io/

最后必须感谢这次黑客马拉松的组织者郝林@特接萝卜 ，还有非常专业的评委杨卫华@TimYang 、@摇摆巴赫 和七牛老大许式伟，活动组织者和赞助商数人科技、DaoCloud、七牛、云雀、ThoughtWorks，我们赢回来的Cherry键盘就是他们提供的哈哈，也诚邀大家关注和参加下一家Docker黑客马拉松。