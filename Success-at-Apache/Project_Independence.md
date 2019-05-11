# Success at Apache: Project Independence
# 赢在Apache：项目独立性

**原文：[https://s.apache.org/CE0V](https://s.apache.org/CE0V)**

**石墨：[https://shimo.im/docs/c7nkM4nD7cIOimMm](https://shimo.im/docs/c7nkM4nD7cIOimMm)**

**作者：By Mark Thomas**

**译者：bastamon**

I've been involved in The Apache Software Foundation (ASF) since 2003. I was using [Apache Tomcat](http://tomcat.apache.org/) at work and I hit a problem that needed a new feature to be implemented. There was already an enhancement request in Bugzilla so I submitted a patch. After some re-work by the [project committers](http://tomcat.apache.org/whoweare.html), the patch was applied and the feature available in the next release. I enjoy problem solving, so I started to take a look at the other open Tomcat [bug reports](http://tomcat.apache.org/bugreport.html) and my involvement grew from there to include [Apache Commons](http://commons.apache.org/), the [Infrastructure Team], the [Security Team](https://infrastructure.apache.org/) and, most recently, the [Board of Directors](http://apache.org/foundation/) to which I was elected in March 2016.

本人自从2003年起参与Apache软件基金会（The Apache Software Foundation, ASF）。当时我正在工作中使用[Apache Tomcat服务器](http://tomcat.apache.org/)，并遇到了一个问题，需要实现一种新特性才能够解决。因为已经有人在Bugzilla（开源的缺陷跟踪系统）中提出了该增强型请求，所以我很快地提交了针对这请求的补丁。后来[项目提交者](http://tomcat.apache.org/whoweare.html)在进行了一些重新工作之后，接受了我所提交的补丁并将其应用在下一个版本中增加了该新特性。因为本人喜欢解决问题，所以我之后开始查看其他公开的Tomcat [bug报告](http://tomcat.apache.org/bugreport.html)，自此我对Apache项目的涉猎程度也开始增加，包括[Apache Commons](http://commons.apache.org/)、[基础设施团队](https://infrastructure.apache.org/)、[安全团队](http://apache.org/security/)，还包括我最近在2016年3月入选[ASF董事会成员](http://apache.org/foundation/)。

Apache Tomcat has always been at the heart of my involvement and is where I spend most of my time. Tomcat started with a donation to the ASF by Sun in 1999 and, some seven major versions later, the project continues to be very successful. A significant part that success is due to the involvement of a wide range of individuals from different companies. The reason those companies are happy co-operating on Tomcat is because of the importance the ASF places on project independence.

Apache Tomcat一直是我参与的核心项目，也是我投入大部分时间研究的地方。Tomcat项目从1999年起就开始以Sun公司的名义向Apache软件基金会（ASF）进行捐赠，在Tomcat经过7个主要版本的更迭后，这个项目依然非常成功。成功的一个主要原因是来自不同公司的各种人才的参与。而这些公司之所以不反对员工在Tomcat上进行合作则是因为ASF非常重视项目独立性。

There are many aspects to project independence but, for me, the most important is that committers and [Project Management Committee (PMC)](http://apache.org/foundation/how-it-works.html#structure) members contribute to the project as individuals and do so with the intention of doing what is best for the community as a whole. Some committers contribute in their free time – I did for the first five years or so with Tomcat – and some are allowed /directed to spend time contributing to Apache projects by their employer. However, those committers contributing on their employer's time still need to act in the best interests of the community rather than the best interest of their employer.

项目独立性要涉及方面有很多，但就我而言，最重要的方面是提交者和项目管理委员会（[Project Management Committee, PMC](http://apache.org/foundation/how-it-works.html#structure)）成员在个人名义上对项目所做出的贡献多少，并且这样做的目的会有益于整个项目社区的发展。一些提交者利用他们的空闲时间为项目做贡献 - 我为Tomcat贡献的前5年就是以这种方式。另一些提交者则是因为他们的雇主允许或规定他们要为Apache项目贡献投入时间。然而，这些受雇提交者（在他们雇佣时间内）所做出的贡献依然要从社区发展的最大利益角度出发，而不是从雇主的最大利益上出发。

To give a specific example, my employer has a product that is built around Apache Tomcat. The sales folks at my employer asked if I could add a feature to this product. The problem was that this feature required access to low-level Tomcat internals in order to implement it effectively. For this to be possible, I would have needed to make some ugly API changes to Tomcat to provide the integration points required. Rather than try and push those changes through, I persuaded my employer that it would better to donate the entire feature to the Apache Tomcat project.

举个具体例子，我的雇主有一个需要Apache Tomcat构建的产品。雇主中销售人员问我可否为这个产品增加一个功能。但问题是，为有效地实现这一特性，产品需要访问Tomcat的底层组件。换言之，我需要对Tomcat的API做一些难看更改，以提供所需的接口（结合点）。但与其试着做这些难看的改动，我建议不如说服雇主，让他最好把整个特性捐赠给Apache Tomcat项目。

This feature also demonstrates other important elements of a successful ASF project: the ability to make decisions in public and always aiming to achieve community consensus with those decisions. As the development of this new feature progressed, the design evolved as the community reviewed the commits and suggested improvements. This isn't always the quickest way of working but the quality of the end result – both technically but more importantly in terms of community health - more than makes up for that.

新特性的加入也反应出促使该Apache软件基金会（ASF）项目成功的其他重要因素：公开决策的能力，以及始终贯彻实现社区决策一致性的努力。随着该项目中新特性的发展完善，社区的审查、提交和改进建议都会促进该项目的设计模式。虽然并不一定总能实现最有效率的工作方式，但项目最终成果的质量————无论是从在技术上，更是从社区良性发展上讲————总能弥补这一可能的缺陷。

The perception of project independence is as important as projects actually being independent. It is a key factor in many projects choosing the ASF as their home so projects need to ensure that the perception agrees with reality.

参与者对项目独立性的观念与实现项目独立性同样重要。这也是为什么许多项目选择ASF作为开发平台的一个主因，因为ASF能帮助项目确保项目参与者的观念与现实相符。

Things can and do go wrong. With [350 projects](https://projects.apache.org/) it is pretty much a given that there will be a handful of ongoing issues at any given time. For example, there might be an attempt to push a project in a particular direction or to suggest that some external entity controls / leads / manages the project. Typically these are self-corrected by the PMC. Sometimes the PMC needs help to resolve the issue e.g. from V.P. Brand Management or possibly the ASF Board.

事情也有可能，也确实会与期望的目标背道而驰。由于要运营[350个项目](https://projects.apache.org/)，几乎可以肯定的是，无论任何时间内都会有这样或那样一些待解决的问题。例如，项目会被某个团体或个人给推向特定的方向，项目也有可能被一些外部实体所控制、领导、管控。项目管理委员会(PMC)通常会自动纠正这些错误。但有时PMC也需要额外帮助才能解决问题，例如来自品牌管理副总裁的或来自Apache软件基金会（ASF）董事会的帮助。

Being a board member is often viewed as more significant than it is. I have no more status in Apache Tomcat, Apache Commons or any other project as a board member than I did before my election to the board. I can still have bad ideas and my fellow community members still point it out when it happens. I don't get to always have my way just because I am board member. It is the board as a whole, rather than the individual board members, whose voice carries significant weight. It is fairly rare for any board member to speak on behalf of the board. To give that some context, I've probably done it no more than once a month since joining the board. It is sufficiently rare that board members always include an explicit "on behalf of the board" when speaking for the board rather than as an individual. Sometimes this point isn't appreciated and the views of an individual board member are incorrectly taken to be the views of the board.

Apache董事会成员这一头衔的影响力其实被大家给过分夸大了。我的地位也只有在Apache Tomcat、Apache Commons以及其他在我入选董事会前参与的项目中才有影响力。我仍会犯一些错误，好在当我犯错时，我社区的成员们会为我指出错误。我不能因为我是Apache董事会的成员就随心所欲。拥有重要影响力的是整个董事会，而不是单个成员。Apache董事会成员很少会代表董事会发言。就我的亲身经历而言，自从我加入Apache董事会以来，我至多一个月也就发言一次。Apache董事会成员在代表董事会发言而非个人时，很少会明确表示该发言“代表董事会”。有时这一点会被大家误解，个别董事会成员的想法会被谬误成是代表整个董事会的观点。

The ASF board is also very different to a corporate board. The board manages the Foundation but it is the PMC that manages the project and sets the direction. The board has no role in the technical direction of a project. The board has responsibility for corporate governance, finance, legal etc., but its primary role is monitoring, mentoring and coaching our project communities to help keep them healthy. As part of this, the board reviews all projects on a regular basis. Newly graduated projects are reviewed monthly for typically 3 months before moving to quarterly reviews. The project V.P. (PMC Chair) is an important part of this. They are the eyes and ears of the board. While the board will look for warning signs as part of its regular review, the V.P. has much more in depth knowledge of the project and can flag specific issues early. Where issues are identified, the aim is to get the PMC to self-correct. The board will provide mentoring / coaching / guidance as necessary but it will be the PMC members who do the work to correct the issue.

Apache软件基金会（ASF）董事会与事业单位的董事会有很大不同。ASF的董事会负责管理基金会，但项目的管理和项目方向的设定则是由项目管理委员会（PMC）负责的。ASF董事会对项目的技术指导没有任何职能作用。ASF董事会真正的职责是企业的治理，财务的管控和法务的履行，等等，但它的主要任务还是负责监督、教导和培养我们的项目社区，以确保项目社区能良性地发展。作为ASF董事会职能的一部分，董事会要定期地审查所有项目。一个刚毕业的项目在转入季度评审之前，往往会需要接受连续3个月的审查。项目副主席（PMC主席）在其中起着至关重要的作用。ta们才是董事会的耳目。虽然ASF董事会在定期的审查中会去寻找项目的预警迹象，但项目副主席应该对该项目的了解更加深入，以便能提前指出其具体问题。一旦审查出问题，则需要让PMC实现自我纠正。ASF董事会将会为此提供必要的教导、培训、指挥，但最终还得交由PMC成员来纠正该问题。

As an example of the board working with a PMC, earlier this year the V.P. for a particular project became unavailable. The board became concerned because the regular reports were not being produced for the project. In this instance, no-else on the PMC had experience of being a project V.P so the board worked with the PMC to identify a new V.P. and to then mentor the new V.P. as they found their way in their new role.

举一个Apache软件基金会（ASF）董事会与项目管理委员会（PMC）合作的例子。今年早些时候，某位负责特定项目的项目副主席离职了，这导致没有人为该项目定期撰写报告，委员也为此感到很是担忧。在这种情况下，PMC中没人有过担任项目副主席职位的经验。因此，ASF董事会与PMC达成合作，从PMC中甄选了一名新的项目副主席，并凭借董事会的经验，对新项目副主席进行指导。

For the [last 17 years](https://blogs.apache.org/foundation/entry/celebrating_17_years_of_the), the ASF has provided a home for a large and diverse set of open source projects. Key to this success has been the importance the ASF places on project independence as part of the Apache Way. By continuing to adhere to the principles of the Apache Way, I am confident that the ASF will continue to be successful for another 17 years and a long way beyond.

在[过去的17年](https://blogs.apache.org/foundation/entry/celebrating_17_years_of_the)里，Apache软件基金会（ASF）为各种各样的开放源码项目提供了开发平台。成功的关键在于ASF能将项目独立性视作Apache原则的一部分。通过继续坚持Apache原则，我相信ASF将在未来的17年里将继续获得成功，并取得长足的进步。