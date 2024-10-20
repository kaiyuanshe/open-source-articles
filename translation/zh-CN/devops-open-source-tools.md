---
title: DevOps 团队如何从开源工具中获得更多收益
author: 德里克·斯马特
authorURL: "https://enterprisersproject.com/user/derek-smart"
originalURL: "https://enterprisersproject.com/article/2020/7/devops-open-source-tools"
translator: ''
reviewer: ''
---

[跳至主要内容]

<!-- more -->

[](https://www.redhat.com/en?intcmp=701600000011jKuAAI)![Supported by Red Hat](/themes/tep/assets/img/l_supported-by-redhat-white.png "由 Red Hat 支持")

用户帐户菜单

- [登录](/user/login?current=/article/2020/7/devops-open-source-tools)
- [RSS](/rss "订阅")

[]![家](/themes/tep/logo.png)[](https://www.redhat.com/en?intcmp=701600000011jKuAAI)![](/themes/tep/assets/img/red_hat_supported_by_red.svg)

帮助 CIO 和 IT 领导者解决问题的社区

主导航

- [文章]
    - [数字化转型]
    - [企业技术]
        - [混合云]
    - [信息技术战略]
    - [资讯科技人才]
    - [Kubernetes：你需要知道的一切]
- [首席信息官研究]
    - [HBR文章]
    - [研究/报告]
    - [资源]
    - [圆桌会议]
    - [什么是数字化转型？]
    - [自动化：IT 领导者指南]
    - [DevOps：IT 领导者指南]
    - [混合云：IT 领导者指南]
    - [终极 DevOps 招聘指南]
- [什么是企业家？]
    - [见见企业家]
    - [认识团队]
- [关于此项目]

# DevOps 团队如何从开源工具中获得更多收益

为了充分利用 DevOps，请从两个维度处理您的开源策略：水平和垂直。请考虑以下关于有效工具和方法的建议

经过

[德里克·斯马特]

2020 年 7 月 2 日 | %t 分钟阅读时间

![](/themes/tep/assets/img/icon-printer.svg)

![Devops gears laptop](data://image/svg+xml;charset=utf-8,%3Csvg%20xmlns%3D'http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg'%20viewBox%3D'0%200%201%201'%2F%3E "DevOps 齿轮笔记本电脑")

[开源](https://www.redhat.com/en/about/open-source?intcmp=701f2000000tjyaAAA)软件开发正迅速成为[DevOps]团队工具包中不可或缺的一部分。开源软件 (OSS) 可让组织（尤其是在其起步阶段）避免昂贵的专有软件成本，这些软件可能无法随业务扩展或随着时间的推移而过时。虽然节省成本是明显的吸引力，但实际上开源的灵活性使其非常适合 DevOps。

**[ 需要向其他人解释关键的 DevOps 术语？获取我们的备忘单： [DevOps 术语表。](https://enterprisersproject.com/cheat-sheet-devops-glossary?intcmp=70160000000h0aXAAQ) ]**

如今，软件团队的任务是跨多种 DevOps 工作流实现[自动化]。他们必须支持广泛的应用程序和工具组合，同时还要满足不同角色的需求，包括开发人员、SRE 和 QA 测试人员。开源软件的特性非常适合应对这些挑战，因为与其他解决方案相比，OSS 可以更轻松（且更便宜）地与管道中的元素集成。

这就是为什么[整个社区]现在团结起来，为其他人的旅程提供必要的指导和支持。

**[ 访问我们的姊妹网站[Opensource.com] ，获取开源和 Linux 教程、建议和资源。 ]**

无论您需要将持续集成服务器与配置管理工具还是其他工具连接起来，可能都已经有了相应的策略。这些协同作用促成了许多开源 DevOps 工具的诞生，其中许多工具现已被广泛采用和使用（全面披露：我在[Delphix]工作，该公司有自己的开源项目）。

**[另请阅读： [IT 领导者现在应该了解的 5 种开源工具]和[DevOps 工程师：有关该角色的常见误解](https://enterprisersproject.com/node/14161?intcmp=70160000000h0axaaq)。]**

通过与财富 500 强公司的数十个 DevOps 团队合作，以及我们自己内部使用 OSS 工具，我发现团队需要从两个维度来制定开源战略：水平和垂直。我的意思是：

## 横向构建：注重自动化和速度

持续集成和持续交付或部署 ( [CI/CD](https://www.redhat.com/en/topics/devops/what-is-ci-cd?intcmp=701f2000000tjyaAAA) ) 是软件的圣杯——许多人都在寻找它，但很少有人找到它。开源工具可能是 DevOps 实现软件开发涅槃状态的关键第一步，但只有当团队在流程的各个步骤中实现自动化和速度时才行。这就是为什么专业人士会提到支持软件“管道”（交付软件的过程）的 DevOps“工具链”（您使用的产品）——并以水平方式直观地描绘这些元素。

在整个组织中水平覆盖端到端工具是实现高度功能化、成熟的 DevOps 实践的关键。然而，这说起来容易做起来难——而且传统上对企业来说既昂贵又困难。今天的好消息是，在软件交付生命周期 (SDLC) 的每个连续步骤中都有更多开源选项。从管理源代码到存储构建工件、发布监控，最后到部署——如果您知道在哪里可以找到，就会有一个 OSS 解决方案。

我们的 DevOps 团队使用[Review Board] 、 [Artificatory] 、 [Jenkins]和 Terraform 等工具来实现开发自动化和速度，从而更快地发布。

**[另请阅读： [5 个让 Kubernetes 更加出色的开源项目](https://enterprisersproject.com/article/2020/5/kubernetes-5-open-source-projects-improve?intcmp=70160000000h0aXAAQ)。]**

## 垂直化：为 DevOps 的每一层添加控制

一旦你利用开源工具来提高整个组织的 SDLC 的速度和自动化程度，下一步是什么？也许不太明显的是，DevOps 团队必须考虑垂直堆栈的工具覆盖范围和仪表，从基本层面上讲，垂直堆栈可分为代码、基础架构和数据层。虽然这些元素的实例在 SDLC 的不同阶段有所不同，但这些层几乎以某种形式存在于 DevOps 实践的每一步中。

例如，在 SDLC 的早期阶段，堆栈可能由几行代码组成，运行在笔记本电脑和包含虚拟数据的小型 MySQL 数据库中。然而，在生命周期的后期，堆栈可能相当于在云基础设施即服务上完全构建的生产应用程序，并与 TB 级数据进行通信。无论其组成如何，团队都需要在 SDLC 中的所有垂直堆栈元素中实现控制和自动化。

同样，好消息是，有大量 OSS 工具可以提供帮助，从[Git] （代码）到[Ansible]和 Salt（基础设施）再到[Liquibase] 、 [Flyway]和[Titan] （数据）。这很重要，因为团队必须将速度、控制和自动化带到 DevOps 实践的每一层，以免其中一个成为阻碍整个进程的瓶颈。

再举一个例子，能够在几分钟内自动调配和配置基于云的测试基础架构的构建是很棒的。但如果仍需要几天时间才能将测试数据传送到该云环境，那么您可能会产生速度的假象，但速度本身却不是。

这就是为什么必须解决 DevOps 操作的每一层（从上到下）的问题，以确保开发过程从一个步骤顺利流向下一个步骤，而不会出现拖延。

## 开源心态

有关 DEVOPS 的更多信息

- [Agile 与 DevOps：有什么区别？]
- [DevOps 文化：您需要问的 5 个问题]
- [DevOps 指标：您是否在衡量重要的事情？]

无论您是 DevOps 新手还是经验丰富的老手，寻找合适的工具集来构建现代软件交付管道都是一件令人生畏的事情。OSS 可以提供您需要的所有组成部分，让集成变得不那么令人生畏，但您也必须有正确的心态。

请记住，您不仅仅是在填充一组开源工具 — 您实际上是在构建一个数组。从两个维度而不是一个维度来考虑自动化和速度，并解决可能在 DevOps 流程的每个步骤中减慢您速度的瓶颈。这样做，您就能使用开源来实现高度自动化、闪电般快速的 CI/CD 管道。

**[ 自动化如何让员工有更多时间进行创新？获取免费电子书： [通过自动化管理 IT](https://www.redhat.com/en/engage/automated-enterprise-ebook-20171115?intcmp=701f2000000tjyaAAA) 。]**

主题

[信息技术战略]

[DevOps]

[开源]

![](/sites/default/files/styles/150x150/public/pictures/derek-smart.jpg?itok=Tnr1xNDS)

Derek Smart 是 Delphix 的高级工程师。Derek 是一位经验丰富的软件开发人员，技能涵盖 API 设计、架构、用户体验、PHP、TDD 和 DevOps。他曾帮助各行各业的公司过渡到 CI/CD。

[更多关于我]

## 相关内容

[]![Harvard Business Review How to Keep Your Top Talent CIO](/sites/default/files/styles/222x125/public/images/How_To_Keep_Your_Top_Talent_HP.png?itok=CPayBNgE "哈佛商业评论 如何留住顶尖人才 CIO")

[重新构想员工保留：4 个技巧]

[]![Harvard Business Review Top 5 articles for October 2015](/sites/default/files/styles/222x125/public/images/Harvard%20Business%20Review%20Top%205.png?itok=qoxmFIPl "《哈佛商业评论》 2015 年 10 月最佳 5 篇文章")

[5 篇《哈佛商业评论》文章将立即引起 CIO 的共鸣]

[]![](/sites/default/files/styles/222x125/public/images/cio_managing_remote_teams.png?itok=JbBeXFfG)

[远程工作：3 个优点和 3 个缺点]

## 评论

埃克塔加尔格 | 2020 年 7 月 6 日

好文章！

## 关于本网站

企业家项目是一个在线出版物和社区，旨在帮助 CIO 和 IT 领导者解决问题。

本网站表达的观点均为作者本人的观点，而非作者所在雇主或 Red Hat 的观点。Enterprisers [Project](http://enterprisersproject.com "企业家计划")希望根据[知识共享许可](http://creativecommons.org/licenses/ "知识共享许可")发布所有内容，但可能无法在所有情况下都这样做。您有责任确保您拥有重复使用本网站上任何作品所需的权限。Red Hat 和 Red Hat 徽标是 Red Hat, Inc. 在美国和其他国家/地区注册的商标。

企业家项目虽然欢迎社区成员[投稿]，但不接受在网站或任何时事通讯上刊登广告的邀请。

## 连接

[RSS订阅]

版权所有 ©2022 Red Hat, Inc.

合法的

- [隐私声明]
- [使用条款]
- [接触]


[跳至主要内容]: #main-content
[]: /
[文章]: /
[数字化转型]: /tags/digital-transformation
[企业技术]: /tags/enterprise-technology
[混合云]: /tags/hybrid-cloud
[信息技术战略]: /tags/it-strategy
[资讯科技人才]: /tags/it-talent
[Kubernetes：你需要知道的一切]: /article/2020/4/kubernetes-everything-you-need-know
[首席信息官研究]: /cio-research
[HBR文章]: /cio-research/hbr-articles
[研究/报告]: /cio-research/researchreports
[资源]: /cio-research/resources
[圆桌会议]: /cio-research/roundtables
[什么是数字化转型？]: /what-is-digital-transformation
[自动化：IT 领导者指南]: /it-automation
[DevOps：IT 领导者指南]: /devops
[混合云：IT 领导者指南]: /hybrid-cloud
[终极 DevOps 招聘指南]: /ultimate-devops-hiring-guide
[什么是企业家？]: /what-enterpriser
[见见企业家]: /meet-enterprisers
[认识团队]: /meet-contributors
[关于此项目]: /about-this-project
[德里克·斯马特]: /user/derek-smart
[DevOps]: https://enterprisersproject.com/taxonomy/term/76
[自动化]: https://enterprisersproject.com/taxonomy/term/66
[整个社区]: https://www.reddit.com/r/devops/
[Opensource.com]: https://opensource.com/
[Delphix]: https://www.delphix.com/
[IT 领导者现在应该了解的 5 种开源工具]: https://enterprisersproject.com/article/2020/5/5-open-source-tools-it-leaders
[Review Board]: https://www.reviewboard.org/
[Artificatory]: https://jfrog.com/artifactory/
[Jenkins]: https://www.jenkins.io/
[Git]: https://git-scm.com/
[Ansible]: https://www.ansible.com/
[Liquibase]: https://www.liquibase.org/
[Flyway]: https://flywaydb.org/
[Titan]: https://titan-data.io/
[Agile 与 DevOps：有什么区别？]: https://enterprisersproject.com/article/2019/1/agile-vs-devops-whats-difference
[DevOps 文化：您需要问的 5 个问题]: https://enterprisersproject.com/article/2020/1/devops-culture-5-questions
[DevOps 指标：您是否在衡量重要的事情？]: https://enterprisersproject.com/article/2017/7/devops-metrics-are-you-measuring-what-matters
[信息技术战略]: /tags/it-strategy
[DevOps]: /tags/devops
[开源]: /tags/open-source
[更多关于我]: /user/derek-smart
[]: /article/2023/4/employee-retention-tips
[重新构想员工保留：4 个技巧]: /article/2023/4/employee-retention-tips
[]: /article/2023/4/5-hbr-articles-cios
[5 篇《哈佛商业评论》文章将立即引起 CIO 的共鸣]: /article/2023/4/5-hbr-articles-cios
[]: /article/2023/4/remote-work-pros-cons
[远程工作：3 个优点和 3 个缺点]: /article/2023/4/remote-work-pros-cons
[投稿]: https://enterprisersproject.com/how-contribute
[RSS订阅]: http://www.enterprisersproject.com/rss
[隐私声明]: /privacy
[使用条款]: /terms-and-conditions
[接触]: /contact