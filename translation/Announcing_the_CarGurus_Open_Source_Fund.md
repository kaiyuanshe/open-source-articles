![BG](https://cdn-images-1.medium.com/max/1600/1*2ZQvt3M72k6t6TAi1SHjPQ.jpeg)
# Announcing the CarGurus Open Source Fund
# 宣布创立CarGurus开源基金

![Seth Woodworth](https://cdn-images-1.medium.com/fit/c/100/100/0*IqfAInZtWk20Q_u_.jpg)
by:[Seth Woodworth](https://medium.com/@seth.woodworth)

原文：[https://medium.com/cargurus-engineering-blog/announcing-the-cargurus-open-source-fund-519f97d9898](https://medium.com/cargurus-engineering-blog/announcing-the-cargurus-open-source-fund-519f97d9898)

I’m very pleased to announce a new initiative to support Free and Open Source Software (FOSS): the CarGurus Open Source Fund (OSF).

我很高兴地宣布一项能帮助解决自由开源软件(FOSS)的新方案:CarGurus公司开源基金(OSF)。

CarGurus engineers rely on FOSS projects to power our infrastructure. It runs our servers, lints our code, compiles our assets, and lets us build more, faster. And like all engines, FOSS projects need maintenance and support to continue running.

CarGurus公司的工程师们一直以来都在依赖自由开源软件项目为我们的基础设施提供基础建设。自由开源软件帮助我们维护服务器，优化代码，编译资源库，并为我们建造更多，更快的设施。但就像所有的引擎一样，自由开源软件项目也需要长久维护和支持才能继续保持良好运作。

## Open Source Fund
## 开源基金

Here at CarGurus, Senior Software Engineer Wei Croteau proposed giving back to these projects with an Open Source Fund. She organized an OSF committee of engineers experienced with FOSS projects. The group asked CarGurus engineers to submit FOSS projects; that were used at CarGurus, non-profit, and/or worked on by a CarGurus employee. From this list, the OSF Committee vetted the projects, and narrowed it down to nine projects to support in Q1 of 2019.

而在最近，CarGurus公司的高级工程师Wei Croteau提议要为维护这些项目而设立一项基金。目前，她已经组织了一群对自由开源软件项目具有丰富经验的工程师。该团队要求CarGurus公司的工程师们提交一些自由开源软件项目；这些项目都是CarGurus公司正在使用的非盈利的项目，或是由CarGurus公司员工参与的项目。开源基金委员会审查了这份项目列表，并将要捐助维护的目标项目锁定在2019年第一季度里的9个项目中。

![image](https://cdn-images-1.medium.com/max/1200/1*WxuD-182jc7KC4a8299yzA.jpeg)

In the spirit of collaboration and bottom-up participation, a pool of $15,600 was dispersed across the 156 members of our engineering organization. Each engineer choose which project received their individual contribution of $100. On top of the pool of engineering directed funds, the OSF committee highlighted one project to give an additional $10,000. As the OSF continues, the pool available the engineering directed funds will increase. Each engineer will continue to choose a project to receive $100 per quarter.

秉着自下而上的合作参与精神，15,600美元已经分配到我们工程师团队中的156名成员手里，每位工程师都可以为他们的个人贡献而分得100美元。除了工程指导资金之外，开源基金委员会还强调要为另一个项目捐助10,000美元。随着开源基金的发展，可用的工程指导基金空间还会继续增加。工程师每选择一个项目，他/她每个季度将多挣100美元。

## Projects we’re funding in the first quarter of 2019
## 我们在2019年第一季度捐助的项目

Here are first projects we’re supporting as part of the CarGurus Open Source Fund:

以下是我们用CarGurus开源基金捐助维护的第一批项目:

    Babel — Ensuring that our JS libraries are forward and backward compatible for all of our users.
    FreeBSD — CarGurus doesn’t use much FreeBSD directly, but we benefit from the security and stability it provides the internet infrastructure, and we have engineers who volunteer for the project.
    GIT — Our distributed version control system of choice.
    Homebrew — The foremost package management platform for MacOS.
    Linux Kernel — The OS for over 1000 virtual machines running at CarGurus.
    Open Web Application Security Project (OWASP) — An unbiased source for best practices for web application security.
    RuboCop — A linter for ensuring our Ruby code quality.
    Webpack — The best solution for bundling JS, CSS, and other asset files.

    Babel — 确保我们的JS库对所有用户都是前后版本兼容的。
    FreeBSD — CarGurus公司并非过分依赖FreeBSD系统，但FreeBSD系统能为我们搭建的安全和稳定的互联网基础设施,并且我们还有一批工程师帮助维护这个系统。
    GIT — 我们选择使用的分布式版本控制系统。
    Homebrew — MacOS系统上最重要的包管理平台。
    Linux Kernel — 一款能为CarGurus公司运行1000个虚拟机的操作系统。
    Open Web Application Security Project (OWASP) — 部署安全web应用程序的最好源码。
    RuboCop — 一款保证我们Ruby代码质量的代码检查器
    Webpack — 捆绑JS，CSS和其他资源的最佳解决方案。

## Highlight Project: Apache Software Foundation
## 重点捐助项目:Apache软件基金会

And the highlight project for this quarter is the **Apache Software Foundation**.

本季度的重点捐助项目是**Apache软件基金会**。

Many engineering teams at CarGurus use projects maintained by the Apache Software Foundation (ASF). When polling the engineering teams about what FOSS projects have the most impact, a large number of those projects were from Apache. The ASF was officially organized 20 years ago to facilitate support and development of the Apache web server. It has since grown significantly, and now organizes hundreds of FOSS projects. A number of these projects are critical to our daily operations here at CarGurus, and we want to highlight the following two:

CarGurus公司的许多工程团队都在使用由Apache软件基金会(ASF)所维护的项目。当我们让工程团队投票选出哪些自由开源软件项目最具影响力时，我们发现选票结果中大部分的项目都来自Apache。Apache软件基金会正式成立于20年前，其成立目的是促进工程师对Apache web服务器的支持和开发。自那时起，Apache软件基金会的发展就惊为天人，现在管理着数百个自由开源软件项目。其中一些项目对我们CarGurus公司的日常运营至关重要，因此我们想重点强调以下两个项目:

**Apache Kafka** is a massively scalable, fault-tolerant, distributed streaming platform used at CarGurus to process dealer inventory, site events, and site analytics. After having outgrown jgroups, Kafka allows us to reliably transport massive amounts of data, scale in response to demand, and facilitate low-latency access to data across the organization.

**Apache Kafka**是一款可伸缩的、可容错的分布式流媒体平台，它在CarGurus用于处理经销商库存、站点事件和站点分析。在Apache Kafka战胜JGroups之后，它还支持让我们进行可靠地大量数据传输，支持对响应需求进行扩展，并实现降低整个组织对数据访问的延迟。

**Apache Airflow** is the DAG-based ETL scheduling framework that enables our data engineering teams to centralize the company’s data assets in timely, reliable fashion. It provides complex dependency management for modeling across hundreds of data sources, enables detailed introspection into status and timing, and powers our highly-concurrent distributed etl architecture.

**Apache Airflow**是一款基于DAG的ETL调度框架，它能使我们的数据工程团队能够及时、可靠地集中管理公司的数据资产。它为跨数百个数据源的复杂的依赖关系管理提供调度模拟，它也提供对状态和时间的详细自检，最后它也有助于我们搭建高并发、分布式的ETL体系结构。

Due to the massive amount of software and libraries from Apache that power CarGurus, the OSF committee has chosen them as our highlight project, and granted them an additional $10,000 on top of our engineers’ votes.

由于CarGurus公司的强劲发展势头离不开Apache所提供的这些大量软件和库，所以开源基金委员会选择它们作为我们捐助的重点项目，并根据我们的工程师的投票结果，为这些项目额外捐助10,000美元。

## On-going support
## 持续不断的支持
This isn’t the end for the Open Source Fund, but just the beginning. The OSF is engineer founded and engineer run. We have commitment and support from management for continued funding, and the amount we give each quarter will increase as we grow the size of our engineering team. We’ll be running another round of funding next quarter as part of our ongoing commitment to give back to the engineering community at large.

这些并不是开源基金要做的的全部，而仅仅只是开始。开源基金是由工程师们创立并运营的。我们得到管理层的承诺和支持，将继续为其提供资金支持，而且随着我们工程团队规模的扩大，我们每个季度捐赠的资金将会继续增加。我们将在下个季度进行另一轮融资，向世界兑现我们将持续回馈工程界的部分诺言。