# 开源软件的价值（哈佛商学院研究报告-初稿）中文版

原文：The Value of Open Source Software (Working Paper 24-038) by Harvard Business School

https://www.hbs.edu/faculty/Pages/item.aspx?num=65230

https://www.hbs.edu/ris/Publication%20Files/24-038_51f8444f-502c-4139-8bf2-56eb4b65c58a.pdf

作者：Manuel Hoffmann, Frank Nagle and Yanuo Zhou

译文（中英对照）：https://kaiyuanshe.feishu.cn/docx/KwdqdICiboWii9xLgQJcuUo9nZe

译者：刘天栋 Ted；审校：刘文涛 Leo
<br>
<br>

![哈佛商学院](https://hackmd.io/_uploads/r1lIRaFTa.png)

## 摘要

&nbsp;&nbsp;&nbsp;&nbsp; 非商业（免费）产品的价值本身就难以评估。一个普遍存在的例子是开源软件（OSS），它是一种全球公共产品，在经济中发挥着至关重要的作用，也是我们今天使用的大多数技术的基础。然而，由于开源软件的非金钱性质和缺乏集中的使用跟踪，很难衡量其价值。因此，在经济计量中，开源软件在很大程度上仍未被计算在内。尽管以前有一些研究已经估算了重新创建这种软件的供应方成本，但由于缺乏数据，无法估算开源软件创造的更大的需求方（使用）价值。因此，为了了解广泛使用的开源软件的全部经济和社会价值，我们利用了来自两个互补来源的独特全球数据，这些数据记录了全球数百万企业使用开源软件的情况。我们首先通过计算重新创建一次最广泛使用的开源软件的成本来估算供应方价值。然后，我们根据每个使用该软件的公司的替代价值来计算需求方价值，如果不存在开源软件，这些公司就需要在内部构建该软件。我们估计，广泛使用的开源软件的供应方价值为 41.5 亿美元，但需求方价值要大得多，为 8.8 万亿美元。我们发现，如果不存在开源软件，企业在软件方面的支出将是目前的 3.5 倍。在我们的样本中，排名前六位的编程语言占开源软件需求方价值的 84%。此外，96% 的需求方价值是由仅 5% 的开源软件开发人员创造的。

[经济文献杂志分类系统](https://zh.wikipedia.org/wiki/JEL%E5%88%86%E7%B1%BB%E7%B3%BB%E7%BB%9F)：[公共经济学](https://zh.wikipedia.org/wiki/%E5%85%AC%E5%85%B1%E7%B6%93%E6%BF%9F%E5%AD%B8) 4；[经济发展，技术变迁和增长](https://zh.wikipedia.org/w/index.php?title=%E6%8A%80%E6%9C%AF%E5%8F%98%E8%BF%81%E5%92%8C%E5%A2%9E%E9%95%BF&action=edit&redlink=1) 3；[劳动和人口经济学](https://zh.wikipedia.org/w/index.php?title=%E5%8A%B3%E5%8A%A8%E5%92%8C%E4%BA%BA%E5%8F%A3%E7%BB%8F%E6%B5%8E%E5%AD%A6&action=edit&redlink=1) 0

**关键词：开源软件、全球公益**

## 参考文献

Hoffmann, Manuel, Frank Nagle, and Yanuo Zhou. "The Value of Open Source Software." Harvard Business School Working Paper, No. 24-038, January 2024.
Copyright © 2024 by Manuel Hoffmann, Frank Nagle, and Yanuo Zhou.

工作文件为草稿。本工作文件仅供评论和讨论之用。未经版权所有人许可，不得复制。可向作者索取工作文件副本。

作者感谢 Linux 基金会提供的财务和行政支持，没有这些支持，普查数据就无法获得。我们非常感谢哈佛商学院研究计算服务部、哈佛创新科学实验室、Linux 基金会以及软件构成分析数据提供商 Snyk、Synopsys 网络安全研究中心和 FOSSA 的支持。我们感谢 Tianli Li 和 Misha Bouzinier 的出色研究协助。我们还要感谢软件开发人员 Boris Martinovic 以及微软公司的 Rich Lander 和 Scott Hanselman，他们为我们提供了对 .NET 生态系统的见解。我们从哈佛商学院价值与估值大会、哈佛商学院 D3 研究日和 2023 管理学院会议的与会者那里获得了有益的反馈。

本研究的部分经费由哈佛商学院提供。

## 1. 导言

2011 年，风险投资家马克-安德森（Mark Andreessen）提出了一个著名的观点："软件正在吞噬世界"（Andreessen，2011 年），今天很少有人会反对这种观点。最近，风险投资家约瑟夫-杰克斯（Joseph Jacks）认为，"开源吞噬软件的速度比软件吞噬世界的速度更快"（杰克斯，2022 年）。最近的其他研究也得出了类似的结论，表明开源软件（OSS）-- 其源代码可公开供检查、使用和修改，通常以去中心化的方式创建并免费发布--出现在 96% 的代码库中（Synopsys，2023 年），一些商业软件由高达 99.9% 的免费开源软件组成（Musseau 等人，2022 年）。尽管开源软件早期经常复制现有专有软件的功能，但如今开源软件已包含人工智能（AI）、量子计算、大数据和分析等各个领域的尖端技术。 然而，尽管开源软件对所有软件（进而对整个经济）的重要性与日俱增，但衡量其影响却一直难以实现。传统上，经济学家用价格（**_p_**）乘以销售数量（**_q_**）来衡量商品或服务所创造的价值。然而，在开源软件中，由于源代码是公开的，因此 **_p_** 通常为零，而 **_q_** 则是未知的，因为对代码复制和再利用的限制有限。例如，如果一家公司从公共代码库下载了一段开源软件，它可能会在内部（合法地）复制成千上万次，然后与供应商或客户共享（也是合法的），因此公共下载数据是不够的。尽管最近的一些研究试图估算 **_p_** 的价值（下文将讨论），除了少数开源软件包外，估算 **_q_** 的数据一直无法获得或难以获得。本文利用新收集的多种来源的数据，旨在提供 **_p_** 和 **_q_** 的估算值，并利用这些数据来揭示这个问题：”开源软件的价值是什么？”

&nbsp;&nbsp;&nbsp;&nbsp; 了解开源软件的价值至关重要，这不仅是因为它在经济中发挥的作用，而且还因为它是具有几百年历史的 "公地 "经济概念最成功、最具影响力的现代范例之一，而 "**_公地_**" 经济概念有可能遭遇被称为 "公地悲剧" 的命运。这一概念最早可以追溯到公元前 4 世纪的哲学家亚里士多德，他写道："最大多数人共有的东西得到的照顾最少。人们最关注的是自己的东西，而对共有的东西关心较少"。威廉-福斯特-劳埃德（William Forster Lloyd，1833 年）在现代经济思想中重新提出了这一观点，他强调了 3 个牧牛人共享土地放牧牛群的例子，每个牧牛人都有过度使用共享资源的动机。加勒特-哈丁（Garrett Hardin，1968 年）写了一篇题为 "公地悲剧” 的文章来讨论这一问题，从而将这一概念带入了更广泛的思潮。在此基础上，埃莉诺-奥斯特罗姆（Elinor Ostrom）获得了诺贝尔奖，她的研究强调了通过社区协调努力避免 “公地悲剧” 的途径，而无需政府强制执行法律来管理和保护公地（奥斯特罗姆，1990 年）。共享牧场与共享数字基础设施之间的相似之处是显而易见的--提供公共草地来喂养牛，进而喂养人，这对农业经济至关重要，而无需重新编写别人已经写好的代码的能力对现代经济也至关重要。此外，在这两种情况下，尽管知道草和代码是经济的关键投入，但衡量它们的实际价值却很困难。正如著名数学家和物理学家开尔文勋爵（Lord Kelvin - William Thomson）所说："如果无法测量，就无法改进。” 如果不能进行改进和维护，那么这些公共物品就可能会因过度使用和投资不足，而在成功的重压下崩溃（Lifshitz-Assaf 和 Nagle，2021 年）。因此，衡量开源软件创造的价值对于数字经济以及建立在数字经济之上的其他经济的未来健康发展至关重要。

&nbsp;&nbsp;&nbsp;&nbsp; 重要的是，最近的一些研究试图解决这些测量问题，但却无法同时把握开源软件使用的广度和深度--本文试图填补这一空白。例如，研究人员试图通过使用新颖的方法来获得广度，他们通过估算重写现有开源软件所需的劳动力成本，估算出美国在 2019 年创造的开源软件的劳动力替代价值为 380  亿美元（Robbins 等人，2021年），欧盟创造的开源软件的劳动力替代价值为  10 亿欧元（Blind 等人，2021年）。这些工作很好地估算了如果现有开源软件明天就消失，那么替换所有现有开源软件所需的成本。然而，这些估算结果依赖于两个重要的假设。首先，从使用的角度来看，所有开源软件都具有同等价值；其次，开源软件的概念仍然存在，社会只需重写一次代码即可，这样就解决了前面提到的 **_p_** 值（价格）缺失的问题，但仍然没有解决 **_q_** 值（数量）缺失的问题。在一个根本不存在开源软件的世界里，每一个开源软件都不只需要重写一次，而是每个使用它的公司都需要重写一次（假设公司可以在其范围内自由共享软件）。其他研究（Greenstein 和 Nagle，2014 年；Murciano-Goroff、Zhuo 和 Greenstein，2021 年）对这一假设进行了更深入的研究，但研究范围较窄，仅关注网络服务器（因其在互联网上面向公众，因此很容易测量）。这两项研究采用了不同的方法，对这一类型的软件进行 **_q_** 测量，并根据企业提供的闭源替代品的价格，采用 **_商品重置价值法_** 推算 **_p_**。美国的数据显示，2012 年开源软件 Apache 网络服务器的价值为 20 亿美元（Greenstein 和 Nagle，2014 年），2018 年 Apache 和日益流行的开源软件网络服务器 nginx 的总价值为 45 亿美元（Murciano-Goroff 等，2021 年）。然而，尽管网络服务器是开源软件生态系统的重要组成部分，但它们只占其中的一小部分。我们试图在现有研究的重要贡献基础上，从广度和深度两方面入手，对开源软件的价值进行更全面的衡量。

&nbsp;&nbsp;&nbsp;&nbsp; 为了从广度和深度两方面考虑开源软件的价值，我们使用了两个主要来源的数据，这些数据使我们能够深入了解全球数以万计的公司所使用的开源软件。第一个来源是 "[自由和开源软件普查 II -- 应用程序库](https://lish.harvard.edu/publications/census-ii-free-and-open-source-software-%E2%80%94-application-libraries)"（**_Census II_** of Free and Open Source Software – Application Libraries，Nagle 等人，2022 年）。**_Census II_** 项目利用与多家软件构成分析（SCA）公司的合作关系，创建了各种使用最广泛的开源软件列表。SCA 受雇于企业扫描其代码库，以确保他们没有违反任何开源软件许可，并附带地跟踪客户使用的所有开源软件代码及其构建的产品。Census II 项目汇总了来自多个 SCA 的数据，在数百万个数据点（开源软件使用情况观测点）的基础上，建立了数万家公司的开源软件使用情况数据集。第二个数据源是 [BuiltWith（内置）数据集](https://builtwith.com/)，我们利用该数据集对近 900 万个网站的扫描，确定这些网站部署的底层技术，包括开源软件库。**_BuiltWith_** 数据已被用于多项学术研究（DeStefano & Timmis 2023、Dushnitsky & Stroube 2021、Koning 等 2022)，但就我们所知，这是第一份侧重于开源软件使用情况的报告。**_Census II_** 数据和 **_BuiltWith_** 数据是互补的，前者关注的是公司销售软件中内置的开源软件，而后者关注的是公司网站中内置的开源软件，从而减少了数据集重复计算观测数据的可能性。总体而言，这两个数据集的组合创造了迄今为止对开源软件使用情况（**_q_**）最全面的测量。此外，通过关注被企业广泛部署和使用的开源软件，而不是考虑开源软件库中存在的所有项目，我们排除了那些实际上并未以任何实际方式被使用的开源软件项目，从而改进了先前研究的方法，并降低了测量误差的可能性。如果不考虑这种测量误差，就会高估开源软件的实际价值，因为被广泛使用的项目与根本未被使用的项目的价值会被当成是一样的。

&nbsp;&nbsp;&nbsp;&nbsp; 为了估算 **_p_**，我们根据上述文献，使用了劳动力替代值。首先，我们通过测量给定的开源软件包中的代码行数，然后应用 [构造性成本模型](https://zh.wikipedia.org/wiki/%E6%9E%84%E9%80%A0%E6%80%A7%E6%88%90%E6%9C%AC%E6%A8%A1%E5%9E%8B) II（COCOMO II，Boehm，1984 年；Boehm 等人，2009 年）-- 来估算从头开始编写代码所需的工时，从而计算出单个公司重新创建该开源软件包所需的人工成本。然后，我们利用 [Salary Expert](https://www.salaryexpert.com/) 提供的全球工资数据，准确估算出如果没有这部分开源软件，企业将产生的人工成本。这些成本可与上述开源软件包层面的 **_q_** 值相结合，从供需双方估算出所有开源软件的综合价值。

&nbsp;&nbsp;&nbsp;&nbsp; 假设我们决定从供给面重新创建所有广泛使用的开源软件，我们发现其投入成本将从 12.2 亿美元到 62.2 亿美元不等。然而，考虑到开源软件的实际使用情况，如果每个使用开源软件包的公司都必须从头开始重新创建（例如，开源软件的概念并不存在），那么需求方的价值就会大很多个数量级，从 2.59 万亿美元到 13.18 万亿美元不等。我们记录了不同编程语言在企业内部（如商业软件产品的生产）与对外（如网站）的编程工作方面，开源软件价值的巨大差异。此外，我们还发现，程序员的价值贡献存在很大的异质性，因为 5% 的程序员创造了供需双方 90% 以上的价值。我们使用的数据可以说是目前衡量企业使用开源软件所创造价值的最全面的数据来源。然而，对于任何项目来说，证据都是不完整的，我们认为我们仍然低估了开源软件的价值，因为我们的数据不包括操作系统，而操作系统是开源软件中被遗漏的一个重要类别。

&nbsp;&nbsp;&nbsp;&nbsp; 本研究为学术文献、从业人员和政策制定者做出了四项重要贡献。首先，它提供了迄今为止对广泛使用的开源软件价值的最完整估算，本研究报告不仅考虑了开源软件的供应方（创建价格），也考虑了使用/需求方，其规模之大前所未有。以前对开源软件价值的估算要么是广度（估算大量开源软件的供应方成本），要么是深度（估算某一特定类型的开源软件创造的价值），而本研究通过使用独特的数据集，更好地了解开源软件使用的广度和深度。此外，本研究没有衡量所有开源软件的价值，而是重点关注企业用于创建其产品和网站的开源软件的价值，从而降低了对那些无法解释生产中实际使用了哪些开源软件的研究中出现的衡量误差。本研究报告的贡献建立在一些重要研究（如 Blind 等人，2021 年；Greenstein 和 Nagle，2014 年；Murciano-Goroff 等人，2021 年；Robbins 等人，2021 年）的基础之上，并对其进行了扩展。尽管精确衡量极为困难，但我们仍试图确定开源软件这个对现代经济做出巨大贡献的重要资源的价值。在此过程中，它为有关信息技术（IT）对生产力影响的长期讨论（Brynjolfsson，1993；Brynjolfsson 和 Hitt，1996；Nagle，2019a；Solow，1987）增添了新的见解，该讨论被称为 "生产力悖论"，即信息技术投资对生产力统计数据的影响有限。这一争论一直延续到新兴的人工智能领域（Brynjolfsson、Rock 和 Syverson，2018 年）。我们的工作通过强调开源软件的存在为社会节约了大量成本（从而提高了生产力），为这一讨论做出了贡献。

&nbsp;&nbsp;&nbsp;&nbsp; 其次，我们的研究通过强调与开源软件投资相关的新数据来源，为无形资本研究的方法论进步做出了贡献。先前的研究表明，无形资本在经济增长（Corrado、Hulten 和 Sichel，2009 年）和企业价值（Peters 和 Taylor，2017 年）中发挥着越来越重要的作用，但它往往未被测量或被曲解（Eisfeldt 和 Papanikolaou，2014 年）。此外，我们还展示了如何利用这些数据源来了解企业在软件方面的真实投资，以及在不存在开源软件的情况下企业必须进行的投资。这一点很有价值，因为软件投资是一种日益重要的无形资本，它正在推动创新（Branstetter、Drev 和 Kwon，2019 年）和绩效（Krishnan 等人，2000 年）。

&nbsp;&nbsp;&nbsp;&nbsp; 第三，我们的研究结果有助于向企业和管理者强调开源软件对其生产的重要性，并为开源软件用户不应只是搭便车，还应为开源软件的创建和维护做出贡献的论点增添砝码（例如，Henkel，2008；Nagle，2018）。这种贡献只是企业在没有开源软件的情况下所需成本的一小部分，而开源软件用户积极参与帮助维护他们所使用的开源软件，对于开源软件生态系统的健康和未来福祉至关重要（Lifshitz-Assaf 和 Nagle，2021 年；Zhang 等人，2019 年）。

&nbsp;&nbsp;&nbsp;&nbsp; 第四，也是最后一点，我们的研究有助于为政策制定者提供信息，他们最近开始认识到开源软件对经济日益增长的重要性，并采取行动支持生态系统（欧盟委员会，2020 年；[美国总统办公室第 14028 号行政命令，2021 年](https://www.gsa.gov/technology/it-contract-vehicles-and-purchasing-programs/information-technology-category/it-security/executive-order-14028)）。然而，这些努力大多与确保现有开源软件生态系统的安全有关，这一点相当重要，但并没有进一步支持创建新的开源软件。我们的研究结果有助于揭示开源软件对整体经济的重要性，并进一步呼吁全社会为这一重要资源提供更多支持。我们的研究结果进一步表明，开源软件创造的大部分价值是由少数贡献者创造的。尽管人们早已知道，开源软件的大部分工作是由少数贡献者完成的，我们补充了新的见解，表明对于广泛使用的开源软件项目的价值创造而言，情况更是如此，而社会对这些贡献者的支持对于开源软件未来的成功，进而对经济的成功至关重要。

&nbsp;&nbsp;&nbsp;&nbsp; 本文的其余部分安排如下。第 2 节介绍了实证背景和数据。第 3 节讨论包括测量挑战在内的方法。在第 4 节中，我们估算了开源软件的价值。第 5 节为结论。

## 2. 实证背景和数据

尽管自由开放软件的概念早在 20 世纪 50 年代就已存在，但由于理查德-斯托尔曼（Richard Stallman）的努力以及他发起的 GNU 项目和自由软件基金会，这一概念在 20 世纪 80 年代变得更加流行（Maracke，2019）。然而，开源软件是在 20 世纪 90 年代 Linus Torvalds 发布了 Linux 内核之后才起飞的，Linux 内核是现在被广泛采用的开源软件操作系统（Tozzi，2016）。如今，开源软件被认为是数字经济的关键基石，被软件开发人员广泛应用于从手机、汽车、冰箱到尖端人工智能等一切领域（Lifshitz-Assaf and Nagle, 2021）。

&nbsp;&nbsp;&nbsp;&nbsp; 我们使用两个互补的主要数据来源来估算开源软件的价值。第一种是 “**_普查 (Census)_**”，它是内向型的。通过它，我们可以确定进入企业创造的产品中的开源软件代码。第二个数据集是 "**_内置 (BuiltWith)_**”，它是外向型的，使我们能够识别消费者通过企业网站直接与之互动的开源软件代码。由于这两个数据集的原始数据只包含软件包名称、版本号和软件包管理器名称，不包含任何源代码相关信息，因此我们首先获取每个软件包的公开代码库，其中包括代码行数和所用编程语言等软件包级信息。有人可能会担心，由于使用了两个不同的数据集，在计算数值时会出现重复计算。然而，”**_普查 (Census)_**” 与 "**_内置 (BuiltWith)_**” 样本的重叠率非常小：两个数据集中只有 18 个软件包是重叠的。此外，重复计算不太可能造成问题，因为这两个数据集捕捉的是开源软件使用情况的不同方面：**_普查_** 捕捉的是面向内部的软件包使用情况，而 **_BuiltWith_** 捕捉的是面向外部的网站使用情况。最后，作为补充数据集，我们使用了 GHTorrent，这是 GitHub 上开源软件相关活动的详细历史记录。GitHub 是最受欢迎的开源软件托管平台，也是开源软件研究的常用数据源（如 Burton 等人，2017；Conti、Peukert 和 Roche，2023；Fackler、Hofmann 和 Laurentsyeva，2023；Kim，2020；Tang、Wang 和 Tong，2023）。通过这些详细的历史数据，我们可以更好地了解开源软件开发者个人贡献的分散性，从而更深入地了解开源软件的价值是如何创造的。我们将在下文中介绍这三种数据源的详细信息及其估算准备工作。

### 普查

《**_[自由与开源软件普查 II](https://lish.harvard.edu/publications/census-ii-free-and-open-source-software-%E2%80%94-application-libraries)_**》（以下简称《**_普查_**》）由 Linux 基金会和哈佛大学创新科学实验室联合开展（Nagle 等人，2022 年）[^1]。该 **_普查_** 是通过汇总三大 SCA（软件构成分析）公司的数据而创建的，这些公司在全球拥有数千名客户。这些 SCA 公司受雇对其客户的代码库进行扫描，收集其专有软件中嵌入的开源软件使用情况，以确保客户不违反任何开源软件许可协议 [^2]。通常，这是与并购相关的尽职调查过程的一部分。与其他公开来源的开源软件需求测量方法（如软件包下载次数和代码变更）不同，该数据的收集方式确保我们能够观察到企业内部开源软件使用的精确数量和类型。此外，它允许我们跟踪每个软件包依赖的对象，这样我们可以观察到间接使用开源软件的情况，这种情况通常比较隐蔽，难以获取 [^3]。 结果是，在 2020 年（2020 年 1 月 1 日至 12 月 31 日），我们观察到这些 SCA 公司的客户所创建的产品中使用了超过 270 万个开源软件包 [^4]。

&nbsp;&nbsp;&nbsp;&nbsp; **_普查_** 项目根据 libraries.io 的命名系统对软件包名称进行了标准化。libraries.io 是由 Tidelift 维护的一个广泛使用的网站，该网站整理了 800 多万个开源软件包的信息。根据三家最著名的 SCA 供应商报告的使用情况，普查 重点关注排名前 2,000 位的软件包，以确定使用最广泛的开源软件，而不是使用分布的长尾。这导致使用量少于 5 次的软件包被剔除。由于 JavaScript 编程语言编写的软件包通常托管在 [Node 软件包管理器（NPM）](https://www.npmjs.com/)上，通常比其他语言的软件包小（代码行数较少），因此使用率通常较高（因为开发人员必须包含许多小软件包，而不是几个大软件包），普查 分别选择了前 1,000 个 NPM 软件包和前 1,000 个非 NPM 托管软件包。

&nbsp;&nbsp;&nbsp;&nbsp; 这一最终数据集涵盖了 **_普查_** 原始数据中观察到的开源软件总使用量的 70% [^5]。对于 **_普查_** 中这 2,000 个开源软件包中的每一个，我们都确定了在 GitHub（最广泛使用的开源软件托管平台）上维护的原始代码 [^6]。 我们首先尝试从 libraries.io 获取每个软件包的 GitHub 代码库 URL。通过这种初步方法，我们将 1,657 个软件包与其 GitHub 代码库进行了匹配 [^7]。对于没有匹配到 GitHub 代码库的 URL，我们大致按照 Singh（2020 年）的方法进行了 Google 搜索。更具体地说，对于每个未匹配到的软件包，我们使用 Google API 搜索软件包名称和 "GitHub 仓库"，并将搜索结果中的第一个 GitHub 代码仓库 URL 作为其最佳匹配的 GitHub URL [^8]。 这样又有 174 个软件包匹配到了代码仓库。最后，我们手动搜索了其余 169 个软件包的 URL，以确定其相关的代码库。整个过程的结果是，在 2,000 个 **_普查_** 软件包中，有 1,840 个软件包与带有原始源代码的代码库相匹配。未匹配的软件包要么已从 GitHub 上删除，要么已成为专有软件（因此原始源代码已不可用），因此，通过手动搜索，我们根据较高的可信度从分析中删除了这 160 个未匹配的软件包（不到 2,000 个 **_普查_** 样本的 8%）。

### 内置

[内置数据库（BuiltWith）](https://builtwith.com/)包含对全球所有公共网站的扫描，并识别它们使用的技术。与侧重于开源软件使用情况的内向型 **_普查_** 数据不同，**_BuiltWith_** 数据扫描了公司网站中专有软件和开源软件的使用情况，但没有明确区分。为了在 **_BuiltWith_** 中将开源软件与专有软件区分开来，我们在技术类别中选取了所有开源的网络开发软件的子集，其中包括 "JavaScript 及其库"，这样就产生了 778 个观测值，与 **_普查_** 数据中的 NPM 开源软件类别相对应。这种抽**_样选择有两个原因。首先，这个给定类别是由 _**BuiltWith**_ 构建的，我们用它作为开源软件的代理，将其与付费软件区分开来。其次，JavaScript 作为构建网站的核心技术之一，是 GitHub 上使用率最高的编程语言（GitHub，2022 年），因此我们能够从需求方的角度捕捉到最重要的开源软件。扫描包括 880 万个不同的网站和 7,280 万个相应的开源软件使用观测数据，时间跨度为 2020 年 1 月 1 日至 11 月 16 日。此外，为了确保我们衡量的是由私营部门产生的开源软件使用价值，我们将 _**BuiltWith\*\*\* 中 JavaScript 相关开源软件的采用域名与 Orbis、Compustat 和 PitchBook 中记录的公司网站进行了匹配。进行这种匹配可确保我们的分析不包括非商业网站（如个人网站）使用的开源软件。因此，匹配率为 38.6%，相当于约 340 万个不同公司的网站。

&nbsp;&nbsp;&nbsp;&nbsp; 对于 **_BuiltWith_** 数据，我们无法采用 **_普查_** 中使用的第一种方法（使用 libraries.io 来帮助识别代码库的 URL），因为 **_BuiltWith_** 只提供了与软件包相关的技术名称，而不包括其他信息（如软件包和软件包管理器名称）[^9]。因此，我们首先使用上文提到的谷歌搜索方法，结果有 695 个软件包与软件源匹配。然后，我们手动搜索了剩余未匹配软件包中 83 个软件包的 GitHub URL，结果新增了 46 个软件包。总之，对于 **_BuiltWith_** 数据，我们能够识别 778 个软件包与软件仓库匹配中的 741 个。与 **_普查_** 数据一样，剩余的 37 个未匹配软件包（不到 5%）因已从 GitHub 上删除而被我们从分析中剔除。

### GHTorrent 数据库

为了衡量开源软件价值创造的分散程度，我们使用了 [GHTorrent 数据库](https://github.com/ghtorrent)，该数据库通过 GitHub 的 REST API 取得了 GitHub 上的全部活动历史。我们利用其中的 GitHub 仓库记录、开发人员级别的提交记录和开发人员公共档案信息来估算每位开发人员的贡献。我们分两步缩小了开发人员贡献分析的样本范围。首先，我们根据 **_Census-BuiltWith_** 联合样本的 GitHub 代码库 URL，从 GHTorrent 中筛选出 GitHub 代码库及其提交 [^10]。其次，我们剔除了约八千名（12%）我们认为是机器人的 GitHub 贡献者，将重点放在人类对开源软件的贡献上 [^11] 。最终样本包含约 6 万名开发人员和 230 万次提交。

&nbsp;&nbsp;&nbsp;&nbsp; 为了对这三个数据集进行估算，我们首先使用开源软件包 [pygount](https://pypi.org/project/pygount/)（计算代码行数）和 [linguist](https://github.com/github-linguist/linguist)（识别编程语言）[^12] 确定了每个软件包的代码行数和使用的编程语言。我们将每种不同的语言分为三个不同的区间，从更可能是人工编写到更可能是机器编写（见 [表 A1](#表A1))。**_区间 1_** 包含编程和标记语言（最有可能是人工编写的），**_区间 3_** 包含数据（最有可能是机器编写的），**_区间 2_** 包含介于两者之间的任何内容，如配置文件和批处理（有时是人工编写的，有时是机器编写的，但很难纯粹根据查看代码来判断）[^13]。在主要估算中，我们只使用了 **_区间 1_**，同时在附录中对 **_区间 2_** 和 **_区间 3_** 进行了稳健性检验，因此我们的结果代表了一个宽裕的下限值。最后，对于某些分析，我们进行了更深入的挖掘，并展示了排名前五的编程语言（我们的数据来自于 GitHub 2022 年分类里所提供的 2020 年的数据）。排名前 5 的编程语言包括 C（包括 C# 和 C++）、Java、JavaScript、Python 和 Typescript。由于 Go 在开源软件中的使用日益广泛，我们还将其添加到这一顶级语言列表中。

## 3. 研究方法论

我们首先采用 [劳动力市场方法](https://kaiyuanshe.feishu.cn/docx/KwdqdICiboWii9xLgQJcuUo9nZe#SmlrdmxMsozzvOxWqTac0WPYnph)，通过考虑开源软件的供需双方来衡量开源软件的价值 [^14]。这个思想实验是，我们生活在一个开源软件不存在的世界里，每家使用特定开源软件的公司都必须重新创建开源软件。利用劳动力市场方法，我们计算出每个开源软件包的劳动力替代成本。为了估算每个软件包的价值，我们使用 [构造性成本模型](https://zh.wikipedia.org/wiki/%E6%9E%84%E9%80%A0%E6%80%A7%E6%88%90%E6%9C%AC%E6%A8%A1%E5%9E%8B) II（COCOMO II，Boehm，1984 年；Boehm 等人，2009 年）对单个软件包进行估算，然后将所有软件包的价值相加，得出供应方劳动力市场替代价值。然后，我们用企业使用每种软件包的次数来衡量供应方的价值，同时剔除每个企业内部的多次使用，从而得出需求方的价值。

&nbsp;&nbsp;&nbsp;&nbsp; 其次，除了总量之外，我们也检查了价值创造过程中的不平等现象。在开源软件中，与许多创造性工作一样，常见的情况是，一小撮人做出了大部分贡献，而其他许多人则做出很小的贡献（有时被称为 80/20 规则，意指 80% 的工作由 20% 的人完成）。研究表明，这些经常做出贡献的人往往由于他们的努力而在开源软件社区中获得有影响力的地位（Hanisch 等人，2018）。因此，为了更好地了解开发者价值创造的分散性，我们首先使用 [GHTorrent](https://github.com/ghtorrent) 数据，并通过两种方式识别开发者的个人贡献：a）开发者对开源软件直接的价值贡献；b）开发者贡献的代码库总数。然后，我们测试了这两种贡献衡量标准的集中程度，以更好地了解对我们衡量的总价值做出贡献的开发者是多是少。我们将在下文解释劳动力市场方法和估值不平等的具体细节。

### 3.1 劳动力市场方法

对于劳动力市场方法，我们通过计算软件包的替换价值来估算开源软件的价值。我们想了解如果雇用一名程序员并向其支付具有竞争力的市场工资，那么重制该软件包需要多少成本。为了估算这一 **_供应方价值_**

<div style="margin-right: auto; width: 10%">

![image](https://hackmd.io/_uploads/BJeVMdp6p.png)

</div>

，我们采用了上文讨论的开源软件包的完整列表，然后计算每个特定软件包中的代码行数 [^15]。我们计算每个特定软件包 **_i_** 的价值，然后将所有这些价值相加，得出总值：

![image](https://hackmd.io/_uploads/B1lng_app.png)

&nbsp;&nbsp;&nbsp;&nbsp; 在这一计算中，我们隐含地不纳入任何生产的外部效应，因为我们假设从一个软件包到下一个软件包不存在会降低编程成本的外溢知识 [^16]。这一方法与其他估算开源软件供应方成本的论文（Blind 等，2021；Nagle，2019b；Robbins 等，2021）所使用的方法类似。然后，我们结合每个软件包的使用信息 (**_Q_**) 计算开源软件的需求方价值：

![image](https://hackmd.io/_uploads/ryGlMOTpa.png)

&nbsp;&nbsp;&nbsp;&nbsp; 在此，我们也同样地不考虑消费的外部效应，也就是说，我们不允许在创建软件包时给公众带来利益，我们还进一步确保每个公司只替换他们使用过一次的软件包，因为被替换的软件包可以作为[俱乐部商品](https://zh.wikipedia.org/wiki/%E6%BA%96%E5%85%AC%E5%85%B1%E8%B2%A1)在公司内部使用（例如，见 Cornes 和 Sandler，1996 年）。

<div style="margin-right: auto; width: 10%">

![image](https://hackmd.io/_uploads/BJeVMdp6p.png)

</div>

**_供给方劳动价值_** 反映了将所有广泛使用的开源软件重写一次的成本（例如，开源软件的概念仍然存在，但所有这些软件包都需要从头开始重写），而

<div style="margin-right: auto; width: 10%">

![image](https://hackmd.io/_uploads/BJTev_6Ta.png)

</div>

**_需求方劳动价值_** 则反映了使用这些开源软件包的每家公司支付开发人员重写这些软件包的成本（例如，开源软件本身不再存在）。

&nbsp;&nbsp;&nbsp;&nbsp; 对于供需模型，我们通过 "[建设性成本模型](https://zh.wikipedia.org/wiki/%E6%9E%84%E9%80%A0%E6%80%A7%E6%88%90%E6%9C%AC%E6%A8%A1%E5%9E%8B) II"（COCOMO II，Boehm，1984 年；Boehm 等，2009 年）获得每个软件包的美元价值（𝑃i）。该模型曾被美国国防部用于估算软件项目成本，也曾用于估算开源软件价值的前期研究（Blind 等，2021；Nagle，2019b；Robbins 等，2021）。这是一个高度灵活的模型，允许我们将代码行数与美元价值进行非线性转换。它使用以下建模方程：

![image](https://hackmd.io/_uploads/Sk6KsOapp.png)

&nbsp;&nbsp;&nbsp;&nbsp; 其中，**_𝐿_** 表示以千为单位的代码行数，**_E_** 表示以人月为单位的每个项目 **_i_** 的工作量。与 Blind 等人（2021 年）的做法一致，我们使用了 **_𝛼、𝛽_** 和 **_𝜂_** 的默认参数值。参数 **_𝛼_** 和 **_𝜂_** 分别为非线性调整系数 2.94 和 1.0997。参数 **_𝜂_** 是一个[作用力调整系数](https://zh.wikipedia.org/wiki/%E6%9E%84%E9%80%A0%E6%80%A7%E6%88%90%E6%9C%AC%E6%A8%A1%E5%9E%8B)，可根据对产品、硬件、人员和项目属性的主观评估进行修改。由于我们没有每个项目的先验值，因此将 **_𝜂_** 设为默认值 1。为了得到每个开源软件项目的价格（**_𝑃i_**），我们将等式（3）的结果乘以普通程序员在公开市场上可获得的加权全球工资。为了计算全球工资，我们采用了 [Salary Expert](https://www.salaryexpert.com/) 提供的 2021 年 GitHub 开发者数量排名前 30 的国家的软件开发者基本月薪（Wachs 等，2022 年）[^17]。我们通过使用低工资（印度）和高工资（美国）劳动力市场来进一步创建工资界限，以更好地了解用于重新创建所有开源软件的程序员池的价值变化 [^18]。

### 3.2 贡献测算

&nbsp;&nbsp;&nbsp;&nbsp; 为了更好地了解价值是如何创造的，以及创造的价值是平等还是不平等，我们分三步绘制了一幅图。第一步，我们测量开发人员的价值贡献。第二步，我们获得开发人员贡献的代码库数量。最后，我们使用众所周知的洛伦兹曲线概念对两者进行图解，以更好地了解贡献的不平等程度。我们将在下文中详细介绍。

&nbsp;&nbsp;&nbsp;&nbsp; **_价值贡献_**。我们计算了每个开发人员贡献的开源软件的供需价值。在代码库层面，我们通过计算每个开发者在代码库提交总数中所占的份额，量化了他们的工作贡献比例。然后将这一份额分别乘以代码库的需求值和供应值，得出该个人贡献者对代码库的增值贡献。最后，我们汇总每个开发者在所有代码库中的价值贡献。特定开发者 **_Dev_** 的个人价值贡献可表示为：

![image](https://hackmd.io/_uploads/Bk_b6qT66.png)

其中

<div style="margin-right: auto; width: 10%">

![image](https://hackmd.io/_uploads/rJQlCcT6a.png)

</div>

是焦点开发者在代码库 **_i_** 中的提交份额，以及

<div style="margin-right: auto; width: 6%">

![image](https://hackmd.io/_uploads/S1yGC5a66.png)

</div>

是等式 (1) 和 (2) 中特定的整个代码库 **_i_** 的需求或供给值，而 **_j_** 是需求值 (**_D_**) 与供给值 (**_S_**) 组成的集合

<div style="margin-right: auto; width: 15%">

![image](https://hackmd.io/_uploads/BJeV0qTpa.png)

</div>

，**_N_** 是主要样本（即 **_Census_** 和 **_BuiltWith_** 样本的总和）中代码库的数量。

&nbsp;&nbsp;&nbsp;&nbsp; **_代码库贡献_**。简单地说，这就是某个开发者所贡献的代码库数量，其表示方法如下：

![image](https://hackmd.io/_uploads/S1cN7aaap.png)

其中，

![image](https://hackmd.io/_uploads/BkIKNK80a.png)

是指标函数，当开发者向代码仓库 **_i_** 提交的次数不为零时，该指标函数等于 1。与价值贡献度一起，它们有助于我们了解整体产生的价值是否集中在少数开发者身上。一般来说，如果单个开发者参与了多个代码库，而不仅仅是少数几个代码库，那么对于整个开源软件生态系统及其多样性来说，可能会更加理想。

&nbsp;&nbsp;&nbsp;&nbsp; **_测量贡献的分散程度_**。为了从图形上考察开发者贡献值的分散性，我们利用了[洛伦兹曲线](https://zh.wikipedia.org/wiki/%E6%B4%9B%E4%BC%A6%E5%85%B9%E6%9B%B2%E7%BA%BF)（Lorenz，1905 年），同时考察了需求方和供应方的贡献值。洛伦兹曲线是表示不平等的一种行之有效的方法，因此，它能让我们更好地理解开发者对私营经济中开源软件贡献的分散程度。根据开发者对开源软件需求和供给的贡献，开发者按升序排列，如 **_等式 (7)_** 所示。随后，这些等级被归一化为 0 至 100 百分位数，作为 **_洛伦兹曲线_** 的 **_x_** 轴值。**_y_** 轴则表示相应的价值贡献

<div style="margin-right: auto; width: 8%">

![image](https://hackmd.io/_uploads/rJc-VaTTa.png)

</div>

。结果部分的图表将阐明开发者之间价值贡献的不平等程度。作为分析的补充，我们还通过绘制 **_等式 (8)_** 进一步研究了代码库贡献

<div style="margin-right: auto; width: 8%">

![image](https://hackmd.io/_uploads/rk7GBpT6a.png)

</div>

的分散程度。这使我们能够确定，是否存在任何实质性的价值不平等，是由于顶级贡献者主要集中于少数特别受欢迎的代码库，还是由于他们参与了更广泛的成功代码库。

## 4. 结果

在使用 [COCOMO](https://zh.wikipedia.org/wiki/%E6%9E%84%E9%80%A0%E6%80%A7%E6%88%90%E6%9C%AC%E6%A8%A1%E5%9E%8B) II 的劳动力市场方法后，我们得到了关于开源软件价值的全球估计值。开源软件的价值。要计算总体价值，我们首先需要基础代码行数（以计算供应方价值），然后需要使用统计数据（以计算需求方价值）。由于不同编程语言的价值可能存在很大差异，我们还在下表中列出了调查期间使用率最高的编程语言。

<a id="表1"><a/>

### 表 1：代码行数和使用情况的描述性统计

![Tab-1 stats on lines of code & usage](https://hackmd.io/_uploads/r1o_XOlRa.png)

注：统计数据基于不同代码库的代码行数。小组 A（B）描绘了**_普查（BuiltWith）_** 数据的总和、平均值、标准差和观测值的数量，涉及代码行数和 **_区间 1_** 中所有软件包的使用情况（见 [表 A1](#表A1))。

&nbsp;&nbsp;&nbsp;&nbsp; **表 1** 分别显示了两个数据集的描述性统计数据。内向**_普查_**（小组 A）包含略多于 2.617 亿行代码，其中 72% 属于顶级编程语言。软件包平均包含 14.2 万行代码，顶级语言子集的平均代码行数略低，为 11.3 万行。在考虑需求（使用）方面时，我们注意到 **_普查_** 软件包的使用次数超过 270 万次，其中 92% 来自顶级语言。软件包的平均使用次数为 1,472.4 次，其中顶级语言的使用率更高，约为 1,497.5 次。我们在面向外部的 **_BuiltWith_** 数据中发现了类似的模式，但程度不同。来自 **_BuiltWith_** 的软件包包含超过 8,200 万行代码，其中 71% 使用的是顶级编程语言。**_BuiltWith_** 样本中的软件包平均有 11.1 万行代码，而顶级语言的平均代码行数较少，约为 8 万行。这是因为我们的 **_BuiltWith_** 数据主要由基于 JavaScript 的软件包组成，这些软件包通常比用其他语言编写的软件包要小。**_BuiltWith_** 软件包的使用次数超过 14.2 万次，其中 99.97% 属于顶级语言。接下来，我们利用这些原始观测数据，通过 **_劳动力市场方法_** 计算出所有开源软件的价值，并估算出供需双方创造的价值。

<a id="表2"><a/>

### 表 2：开源的劳动力市场价值

|                | 供给方劳动力市场价值 | 需求方劳动力市场价值 |
| -------------- | -------------------- | -------------------- |
| 工资：低       | $12.2 亿美元         | $2.59 万亿美元       |
| 工资：全球平均 | $41.5 亿美元         | $8.80 万亿美元       |
| 工资：高       | $62.2 亿美元         | $13.18 万亿美元      |

注：高工资方案基于美国的平均工资，低工资方案为 2020 年印度程序员的平均工资。全球工资是[表 A4](https://hackmd.io/7O2fpfsAQGiFfYFEPN4eNQ?view#%E8%A1%A8-A4%EF%BC%9A%E4%BD%BF%E7%94%A8%E5%8C%BA%E9%97%B4-1%E3%80%812-%E5%92%8C-3-%E8%AF%AD%E8%A8%80%E7%9A%84%E5%BC%80%E6%BA%90%E7%9A%84%E5%8A%B3%E5%8A%A8%E5%8A%9B%E5%B8%82%E5%9C%BA%E4%BB%B7%E5%80%BC) 中各国的平均工资，根据其对开源软件的贡献进行加权。这些估算仅包括软件分类 **_区间 1_** 中的语言（见 [表 A1](#表A1)）。

&nbsp;&nbsp;&nbsp;&nbsp; **表 2** 显示了基于与企业相关的 **_普查_** 和 **_BuiltWith_** 之联合样本对开源软件价值的估算。**表 2** 中的所有估计值仅基于 [表 A1](#表A1) 中归入 **_区间 1_** 的软件语言，这些语言最有可能由人类而非机器编写 [^19]。第一列分别包含低收入国家（印度）、全球平均工资和高收入国家（美国）的工资估计值（如上所述）。要将所有广泛使用的开源软件重制一次（例如，开源软件的理念仍然存在，但目前所有的开源软件都被删除，需要从头开始编码），使用印度开发人员平均工资的程序员需要投资 12.2 亿美元。相比之下，如果我们使用美国开发人员的平均工资，重制所有广泛使用的开源软件将需要投资 62.2 亿美元。根据上述对开源软件的现有地域贡献来权衡，使用来自世界各地的程序员池，将导致介于低收入国家和高收入国家之间的 41.5 亿美元投资。将这些数字与类似研究中的数字进行比较，有助于了解所有开源软件（以前的研究）与广泛使用的开源软件（我们的研究）的估值差异。Robbins 等人（2021 年）和 Blind 等人（2021 年）使用了与我们类似的方法，估计 2019 年美国创造的开源软件价值为 380 亿美元，2018 年欧盟创造的开源软件价值为 10 亿欧元。Wachs 等人（2022 年）的研究表明，大约 50% 的开源软件贡献来自美国和欧盟。总体而言，这些研究得出的全球开源软件价值为 780 亿美元。因此，我们仅对面向企业并被广泛使用的开源软件的供应方价值进行了 41.5 亿美元的中间估计，这是一个可信的下限，并突出表明，在不考虑特定开源软件包是否被广泛使用的情况下，对开源软件供应方总价值的估计更高。这进一步表明，使用最广泛的开源软件的供应方价值约占所有开源软件供应方价值的 5.5%。

&nbsp;&nbsp;&nbsp;&nbsp; **表 2** 的第二列是基于 **_劳动力市场方法_** 的需求方估算。我们发现，如果企业必须重新创建它们使用的所有开源软件包（例如，开源软件本身不复存在，每个使用开源软件包的企业都必须重新创建它），那么仅使用低工资国家或高工资国家的劳动力，整个成本将分别达到 2.59 万亿美元到 13.18 万亿美元。全球的程序员可以重新创建所有被广泛使用的开源软件，成本约为 8.80 万亿美元。对这一数字的解读稍显复杂，但仍然可行。根据 Statista（2023 年）的报告，2020 年（与我们的数据同年）全球软件收入为 5,317 亿美元。然而，这代表的是软件的流量，而不是存量。根据政府关于软件三年完全折旧的估算，我们可以进行反向计算，将 2020 年使用的全部套装软件存量的购买价值视为 2018 年至 2020 年售出软件的总和，即 1.54 万亿美元。此外，这仅代表套装软件的支出，不包括定制购买或内部开发的软件。在此，对私营部门软件投资总体情况的最佳估算来自美国国民收入和产品账户数据（NIPA 2023）。国民账户数据显示，2020 年美国私营企业在软件方面的支出为 4,792 亿美元，其中 45% （2155 亿美元）为套装软件。如果我们假定世界其他地区的比例也是如此，那么 2020 年企业在软件使用上的支出总额为 3.4 万亿美元（=1.54 万亿美元/0.45）。将这一粗略估算与需求方根据全球平均工资对开源软件价值的估算（8.8 万亿美元）相结合，这表明如果企业需要支付内部开发人员编写目前免费使用的开源软件，那么企业将花费 12.2 万亿美元（=3.4 万亿美元 + 8.8 万亿美元），即目前花费的三倍半。

### 图 1. 开源软件的价值：顶级语言

| 小组 A. 供应方                                                         | 小组 B. 需求方                                                         |
| ---------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| ![Fig-1 Panel A Supply Side](https://hackmd.io/_uploads/H1flhNgCa.png) | ![Fig-1 Panel B Demand Side](https://hackmd.io/_uploads/r1v5aNgA6.png) |

注：这些数字显示了 GitHub 和 Go 提供的前 5 种语言的劳动力市场价值。小组 A 显示的是供应方，小组 B 显示的是需求方。在劳动力方面，我们使用了我们估算的全球程序员平均工资，详见方法论部分。

**图 1** 显示了开源软件的价值在顶级编程语言中的异质性。小组 A 显示的是供应方价值，纵轴显示的是劳动力价值。我们发现用 Go 创建的开源软件包价值最高，达 8.03 亿美元，如果没有这些开源软件包，就必须从头开始创建。紧随 Go 之后的是 JavaScript 和 Java，价值分别为 7.58 亿美元和 6.58 亿美元。C 和 Typescript 的价值分别为 4.06 亿美元和 3.17 亿美元，而 Python 的价值在顶级语言中最低，约为 5,500 万美元。JavaScript 不仅至少从 2014 年起就是 GitHub 上的顶级语言（GitHub，2022 年），而且还是我们数据中价值最高的语言之一。相比之下，Python 随着时间的推移变得越来越流行，在 GitHub 上的所有开源软件包中，从第四位上升到 2020 年的第二位，而在我们的顶级语言中则排在最后一位。

&nbsp;&nbsp;&nbsp;&nbsp; 小组 B 显示了顶级编程语言的需求方价值。根据使用产生的价值，Go 的价值是排名第二的 JavaScript 的四倍多。Typescript（一种扩展了 JavaScript 的语言）的增长势头迅猛，从 2017 年十大语言的第十位上升到 2020 年的第四位，这也反映在我们的数据中，Typescript 是需求方第三大语言。紧随这两种网络语言之后的是 C 语言，远远落后的是 Java 和 Python。

### 图 2. 五大语言 + Go 和各种数据源的开源价值

| 小组 A.普查.供应方                                                            | 小组 B.普查.需求方                                                            |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| ![Fig-2 Panel A.Census.Supply Side](https://hackmd.io/_uploads/BkabawgC6.png) | ![Fig-2 Panel B.Census.Demand Side](https://hackmd.io/_uploads/BJlSpDlAa.png) |

| 小组 C.内置.供应方                                                               | 小组 C.内置.需求方                                                               |
| -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| ![Fig-2 Panel C.BuiltWith.Supply Side](https://hackmd.io/_uploads/r1ADpwxCa.png) | ![Fig-2 Panel D.BuiltWith.Demand Side](https://hackmd.io/_uploads/S1pt6PgAT.png) |

注：本图显示了排名前五的语言（根据 GitHub）+ Go 的劳动力和商品市场价值，按内向型（**_普查_**）和外向型（**_BuiltWith_**）数据源划分。小组 A 和 B 显示 **_普查_** 的供应方和需求方数值，小组 C 和 D 显示 **_BuiltWith_** 的供应方和需求方数值。

**图 2** 按面向内部（**_普查_**）和面向外部（**_BuiltWith_**）的数据源，对每种语言的开源软件价值估算进行了划分。小组 A 和小组 B 侧重于**_普查_** 的供需估算。尽管 JavaScript 的影响要小得多，但我们在汇总两种数据源时 **图 1** 发现了类似的模式。在小组 A 中的 **_普查_** 供应方中，Java 的值位居第二，而 **_普查_** 中的 JavaScript 代码对总体的贡献值要低得多。同样的，C、Python 和 Typescript 的供应方价值也主要由 **_普查_** 驱动。从小组 B 的需求方来看，我们发现 Go 是内向代码中最受欢迎的语言，而所有其他语言相对而言似乎都微不足道。

&nbsp;&nbsp;&nbsp;&nbsp; **图 2** 的小组 C 和小组 D 显示了 **_BuiltWith_** 数据集的供应方和需求方数值。小组 C 中的供应方数值清楚地表明，来自 **_BuiltWith_** 样本的数值是由 JavaScript 代码驱动的，这是一个很好的合理性检查，因为如上所述，我们在 **_BuiltWith_** 样本中主要使用 JavaScript 包来代表开源软件。第二高值由 TypeScript 创建，这一点令人放心，因为 TypeScript 是 JavaScript 的超集。小组 D 显示了使用方面的类似模式，其中大部分价值来自 JavaScript，而 TypeScript 也排在第二位。其他语言对供需方价值的贡献微乎其微。总体而言，这些发现与各种语言的主要使用情况（网络编程与应用编程）基本一致，而大众使用的语言与产生价值的语言则不一定相同。

### 图 3. 各行业网站的开源价值

![Fig-3 OSS Value from Industry Websites](https://hackmd.io/_uploads/S1m7ldlCp.png)
注：本图中显示的是使用 "**_BuiltWith_**" 数据计算的 NAICS 2 位数代码行业的需求方劳动力价值。对于与多个行业相关的企业（领域），我们取其平均值并在各行业间进行分配。

&nbsp;&nbsp;&nbsp;&nbsp; **图 3** 显示了使用 "**_BuiltWith_**" 在线数据按 NAICS 2 位数代码划分的各行业开源软件的需求方价值 [^20]。这可以解释为每个行业因开源软件的存在而获得的价值。使用价值最高的行业是 "专业、科学和技术服务"，约为 430 亿美元。"零售业" 以及 "行政和支持以及废物管理和补救服务" 分别占开源软件需求方对外价值的另一大部分，分别为 360 亿美元和 350 亿美元。相比之下，"采矿、采石、石油和天然气开采"、"公用事业" 和 "农业、林业、渔业和狩猎" 等行业的产值只占很小一部分。 后一类行业属于典型的非服务业行业，因此，软件在其中发挥的作用预计会较小。

### 图 4. 开源价值创造的分散性

| 小组 A. 供应方                                                         | 小组 B. 需求方                                                         |
| ---------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| ![Fig-4 Panel A Supply Side](https://hackmd.io/_uploads/ryJc-dlRa.png) | ![Fig-4 Panel B Demand Side](https://hackmd.io/_uploads/BJPibOeAp.png) |

注：图中显示了每位开发者贡献的劳动力市场价值的洛伦兹曲线（蓝色），以及部分程序员贡献的代码库数量（黄色）。小组 A 显示的是供应方，小组 B 显示的是使用方。

&nbsp;&nbsp;&nbsp;&nbsp; **图 4** 显示了洛伦兹曲线以及部分程序员为供应方（小组 A）和需求方（小组 B）贡献的代码库数量。如果洛伦兹曲线直接位于 45 度线上，则意味着各程序员的贡献值分布非常均匀。相反，小组 A 显示的洛伦兹曲线几乎是一条平线，程序员的最终份额急剧增加。这意味着供应价值的分布极不均匀，比 80/20 标准要集中得多。事实上，最后 5% 的程序员，即 3,000 名程序员，创造了 93% 以上的供应方价值。同样，小组 B 显示，如果考虑到使用情况，最后 5% 的程序员创造了 96% 以上的需求方价值。总体而言，这表明只有极少数程序员创造了大量的开源软件代码，而这些代码在很大程度上被企业用来创造自己的代码。在小组 A 和小组 B 中，我们还可以看到贡献价值最高的最后 10-15% 的程序员的代码库数量在增加，这意味着少数程序员产生的不均衡价值不仅仅是由于少数几个极具价值的代码库，而是由于这些少数贡献者对大量代码库的贡献。

## 5. 结论（Conclusion）

&nbsp;&nbsp;&nbsp;&nbsp; 在本研究中，我们利用两个独特的数据集：开源软件 **_普查_** 和 **_BuiltWith_** 数据，估算了全球广泛使用的开源软件的价值。我们不仅能估算现有代码的供应方价值（例如，重写每一个广泛使用的开源软件一次所需的成本），还能估算私营经济的需求方价值（例如，每一个使用开源软件的公司重写该软件所需的成本）。虽然我们没有关注开源软件的长尾，但我们认为这是我们研究的另一个贡献，因为关注被广泛使用的开源软件可以让我们更准确地了解开源软件创造的价值，而不是仅仅衡量所有开源软件的重置成本（这会高估实际价值，因为许多开源软件项目并没有用于生产代码）。然而，尽管我们根据广泛的使用数据强调了开源软件在我们社会中的巨大价值，但要确定全世界 100% 的开源软件使用情况是不可行的，因此，我们的需求方估算很可能低估了真正的价值。

&nbsp;&nbsp;&nbsp;&nbsp; 根据使用情况进行调整后，我们发现，当使用来自世界各地的程序员时，开源软件的需求方价值高达 8.8 万亿美元，但也存在一些差异，这取决于我们只从低收入国家还是高收入国家雇用程序员。不同编程语言的价值以及代码是面向内部（即用于创建销售产品）还是面向外部（即在公司网站上使用）存在很大差异。前 6 种编程语言创造了 84% 的需求方价值。我们还显示了各行业之间的巨大差异，以及程序员自身价值贡献的差异。超过 95% 的需求方价值是由仅 5% 的程序员创造的，而这些程序员不仅为少数几个广泛使用的项目做出了贡献，而且比处于价值分布低端的程序员对更多的项目做出了贡献。

&nbsp;&nbsp;&nbsp;&nbsp; 总体而言，我们的研究结果表明，开源软件对经济的贡献价值巨大，尽管由于价格等于零，而数量又很难仅通过公共数据来衡量，因此通过直接测量，这一价值通常显示为零。我们的研究为今后研究开源软件、所有信息技术及其对全球经济日益增长的影响做出了铺垫基础的工作。

## 参考资料（References）

- Almeida, D. A., Murphy, G. C., Wilson, G., & Hoye, M. (2017, May). Do software developers understand open-source licenses? In 2017 IEEE/ACM 25th International Conference on Program Comprehension (ICPC) (pp. 1-11). IEEE.
- Andreessen, M. (2011). Why Software Is Eating The World. Accessed May 1, 2023. Source: https://www.wsj.com/articles/SB10001424053111903480904576512250915629460
- Aristotle. (1981). Politics. Book 2, Chapter 3. T.A. Sinclair translation. Penguin Books, London.
- Blind, K., Böhm, M., Grzegorzewska, P., Katz, A., Muto, S., Pätsch, S., & Schubert, T. (2021). The impact of Open Source Software and Hardware on technological independence, competitiveness, and innovation in the EU economy. European Commission, Ed.
- Blind, K., & Schubert, T. (2023). Estimating the GDP effect of Open Source Software and its complementarities with R&D and patents: evidence and policy implications. The Journal of Technology Transfer, 1-26. Boehm, B. W. (1984). Software engineering economics. IEEE Transactions on Software Engineering, (1), 4-21.
- Boehm, B. W., Abts, C., Brown, A. W., Chulani, S., Clark, B. K., Horowitz, E., Madachy, R., Reifer, D., & Steece, B. (2009). Software cost estimation with COCOMO II. Prentice Hall Press.
- Branstetter, Lee G., Matej Drev, and Namho Kwon. (2019). “Get with the program: Softwaredriven innovation in traditional manufacturing.” Management Science 65, no. 2: 541-558.
- Brynjolfsson, E. (1993). The productivity paradox of information technology. Communications of the ACM, 36(12), 66-77.
- Brynjolfsson, E., & Hitt, L. (1996). Paradox lost? Firm-level evidence on the returns to information systems spending. Management Science, 42(4), 541-558.
- Brynjolfsson, E., Rock, D., & Syverson, C. (2018). Artificial intelligence and the modern productivity paradox: A clash of expectations and statistics. In The economics of artificial intelligence: An agenda (pp. 23-57). University of Chicago Press.
- Burton, R. M., Håkonsson, D. D., Nickerson, J., Puranam, P., Workiewicz, M., & Zenger, T. (2017). GitHub: exploring the space between boss-less and hierarchical forms of organizing. Journal of Organization Design, 6, 1-19.
- Conti, A., Peukert, C., & Roche, M. |(2023). "Beefing IT up for your Investor? Open Sourcing and Startup Funding: Evidence from GitHub." Harvard Business School Working paper No. 22-001.
- Cornes, R., & Sandler, T. (1996). The theory of externalities, public goods, and club goods. Cambridge University Press.
- DeStefano, T., and J. Timmis (2023). Demand Shocks and Data Analytics Diffusion, working paper.
- Dushnitsky, G., & Stroube, B. K. (2021). Low-code entrepreneurship: Shopify and the alternative path to growth. Journal of Business Venturing Insights, 16, e00251.
- Eisfeldt, A. L., & Papanikolaou, D. (2014). The value and ownership of intangible capital. American Economic Review, 104(5), 189-194.
- European Commission. (2020). Open Source Software Strategy 2020-2023. Luxembourg: Office for Official Publications of the European Communities.
- Executive Order No. 14028. (2021). Executive Order on Improving the Nation’s Cybersecurity. May 2021.
- Fackler, T., Hofmann, M., & Laurentsyeva, N. (2023). Defying Gravity: What Drives Productivity in Remote Teams? (No. 427). CRC TRR 190 Rationality and Competition.
- Greenstein, S., & Nagle, F. (2014). Digital dark matter and the economic contribution of Apache. Research Policy, 43(4), 623-631.
- GitHub (2022). “Octoverse: The state of open source software.” Accessed November 3, 2023. https://octoverse.github.com/2022/top-programming-languages.
- Hanisch, M., Haeussler, C., Berreiter, S., & Apel, S. (2018, July). Developers’ progression from periphery to core in the Linux kernel development project. In Academy of Management Proceedings (Vol. 2018, No. 1, p. 14263). Briarcliff Manor, NY 10510: Academy of Management.
- Hardin, G. (1968). “The Tragedy of the Commons”. Science. 162 (3859): 1243–1248.
- Henkel, J. (2009). Champions of revealing—the role of open source developers in commercial firms. Industrial and Corporate Change, 18(3), 435-471.
- Jacks, J. (2022). Open Source Is Eating Software FASTER than Software Is Eating The World. Accessed May 1, 2023. Source: https://www.coss.community/cossc/open-source-iseating-software-faster-than-software-is-eating-the-world-3b01
- Kim, D. Y. (2020). Product Market Performance and Openness: The Moderating Role of Customer Heterogeneity. In Academy of Management Proceedings (Vol. 2020, No. 1, p. 21309). Briarcliff Manor, NY 10510: Academy of Management.
- Koning, R., Hasan, S., & Chatterji, A. (2022). Experimentation and start-up performance: Evidence from A/B testing. Management Science, 68(9), 6434-6453.
- Krishnan, M. S., Kriebel, C. H., Kekre, S., & Mukhopadhyay, T. (2000). An empirical analysis of productivity and quality in software products. Management Science, 46(6), 745-759.
- Lerner, J., & Tirole, J. (2005). The scope of open source licensing. Journal of Law, Economics, and Organization, 21(1), 20-56.
- Lorenz, M. O. (1905). "Methods of measuring the concentration of wealth". Publications of the American Statistical Association. Publications of the American Statistical Association, Vol. 9, No. 70. 9 (70): 209–219. Bibcode:1905PAmSA...9..209L. doi:10.2307/2276207. JSTOR 2276207.
- Lifshitz-Assaf, H., & Nagle, F. (2021). The digital economy runs on open source. Here's how to protect it. Harvard Business Review Digital Articles. https://hbr.org/2021/09/the-digitaleconomy-runs-on-open-source-heres-how-to-protect-it.
- Lloyd, W. F. (1833). Two lectures on the checks to population: Delivered before the University of Oxford, in Michaelmas Term 1832. JH Parker.
- Maracke, C. (2019). Free and Open Source Software and FRAND‐based patent licenses: How to mediate between Standard Essential Patent and Free and Open Source Software. The Journal of World Intellectual Property, 22(3-4), 78-102.
- Murciano-Goroff, R., Zhuo, R., & Greenstein, S. (2021). Hidden software and veiled value creation: Illustrations from server software usage. Research Policy, 50(9), 104333.
- Musseau, J., Meyers, J. S., Sieniawski, G. P., Thompson, C. A., & German, D. (2022, May). Is open source eating the world’s software? Measuring the proportion of open source in proprietary software using Java binaries. In Proceedings of the 19th International Conference on Mining Software Repositories (pp. 561-565).
- Nagle, F. (2018). Learning by contributing: Gaining competitive advantage through contribution to crowdsourced public goods. Organization Science, 29(4), 569-587.
- Nagle, F. (2019a). Open source software and firm productivity. Management Science, 65(3), 1191- 1215.
- Nagle, Frank (2019b). “Government Technology Policy, Social Value, and National Competitiveness.” Harvard Business School Working Paper, No. 19-103, March 2019.
- Nagle, F., Dana, J., Hoffman, J., Randazzo, S., & Zhou, Y. (2022). Census II of Free and Open Source Software—Application Libraries. Linux Foundation, Harvard Laboratory for Innovation Science (LISH) and Open Source Security Foundation (OpenSSF). https://www.linuxfoundation.org/research/census-ii-of-free-and-open-source-softwareapplication-libraries.
- NIPA (2023). Bureau of Economic Analysis, NIPA Table 5.6.5. accessed: 2023-11-14, source: https://apps.bea.gov/iTable/?reqid=19&step=3&isuri=1&select*all_years=0&nipa_table* list=331&series=q&first_year=2013&last_year=2023&scale=-9.
- Nordhaus, William D., 2006, “Principles of National Accounting for Nonmarket Accounts,” in A New Architecture for the US National Accounts, editors, Dale W. Jorgenson, J. Steven Landefeld, and William D. Nordhaus, University of Chicago Press.
- Ostrom, Elinor (1990). Governing the commons: The evolution of institutions for collective action. Cambridge: Cambridge University Press.
- Peters, R. H., & Taylor, L. A. (2017). Intangible capital and the investment-q relation. Journal of Financial Economics, 123(2), 251-272.
- Robbins, C., Korkmaz, G., Guci, L., Calderón, J. B. S., & Kramer, B. (2021). A First Look at Open-Source Software Investment in the United States and in Other Countries, 2009-2019.
- Singh, Shivendu Pratap (2020) Products, Platforms, and Open Innovation: Three Essays on Technology Innovation. Doctoral Dissertation, University of Pittsburgh. (Unpublished)
- Solow, R. (1987). “We Better Watch Out.” New York Times Book Review, July 1987, p. 36. Statista (2023).
- Statista Software Worldwide, accessed 2023-11-14, source: - https://www.statista.com/outlook/tmo/software/worldwide#revenue, accessed November 2023.
- Synopsys (2023). 2023 OSSRA: A deep dive into open source trends. Accessed May 1, 2023. Source: https://www.synopsys.com/blogs/software-security/open-source-trends-ossrareport/
- Tang, S., Wang, Z., & Tong, T. (2023). Knowledge Governance in Open Source Contributions: The Role of Gatekeepers. In Academy of Management Proceedings (Vol. 2023, No. 1, p. 17622). Briarcliff Manor, NY 10510: Academy of Management.
- Tozzi, C. (2016). “Open Source History: Why Did Linux Succeed?” Channel Futures, August, 2016. Accessed November 3, 2023. https://www.channelfutures.com/open-source/opensource-history-why-did-linux-succeed
- Wachs, J., Nitecki, M., Schueller, W., & Polleres, A. (2022). The geography of open source software: Evidence from GitHub. Technological Forecasting and Social Change, 176, 121478.
- Williamson, S. (2006). Notes on macroeconomic theory. University in St. Louis. Department of Economics.
- Zhang, Y., Zhou, M., Mockus, A., & Jin, Z. (2019). Companies’ participation in oss development– an empirical study of openstack. IEEE Transactions on Software Engineering, 47(10), 2242-2259.

## 在线附录

<a id="表A1"><a/>

### 表 A1：各区间内的语言

| 类型                                                                             | 语言                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| -------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 小组 A：区间 1                                                                   | 语言                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| 标记语言（Mark -Up Language）                                                    | BIBTEX <br> COLDFUSION HTML <br> DOCBOOK <br> XML <br> HAML <br> HTML <br> HXML <br> JAVAEE XML <br> MARKDOWN <br> MXML <br> RELAX-NG COMPACT <br> RHTML <br> TEX <br> XML <br> XQUERY <br> YAML                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| 编程语言 （Programming Language）                                                | ABNF <br> ACTIONSCRIPT <br> ADA <br> APPLESCRIPT <br> ARDUINO <br> ASPECTJ <br> ASPX-CS <br> ASPX-VB <br> AWK <br> C <br> C# <br> CHARMCI <br> CLOJURE <br> COFFEESCRIPT <br> COMMON LISP <br> CSS <br> CUDA <br> CYTHON <br> D <br> DART <br> DELPHI <br> EASYTRIEVE <br> EC <br> ELIXIR <br> ELM <br> EMACSLISP <br> ERLANG <br> F# <br> FISH <br> FORTH <br> FORTRAN <br> FORTRANFIXED <br> GAP <br> GHERKIN <br> GLSL <br> GO <br> GRAPHVIZ <br> GROOVY <br> HASKELL <br> HAXE <br> IDL <br> JAVA <br> JAVA SERVER PAGE <br> JAVASCRIPT <br> KOTLIN <br> LESSCSS <br> LIQUID <br> LIVESCRIPT <br> LLVM <br> LOGOS <br> LUA <br> MATHEMATICA <br> MINISCRIPT <br> MODULA - 2 <br> NASM <br> NIX <br> OBJECTIVE - C <br> OBJECTIVE - J <br> OCAML <br> OPENEDGE ABL <br> PAWN <br> PERL <br> PHP <br> PL/PGSQL <br> POSTSCRIPT <br> POVRAY <br> PROLOG <br> PROPERTIES <br> PUPPET <br> PYTHON <br> REASONML <br> REBOL <br> REDCODE <br> REXX <br> RUBY <br> RUST <br> S <br> SASS <br> SCALA <br> SCILAB <br> SCSS <br> SLIM <br> SMALLTALK <br> SOLIDITY <br> STANDARD ML <br> SWIFT <br> SWIG <br> TADS 3 <br> TCL <br> THRIFT <br> TRANSACT-SQL <br> TREETOP <br> TYPESCRIPT <br> VB.NET <br> VBSCRIPT <br> VCL <br> VIML <br> WEB IDL |
| 小组 B：区间 2                                                                   | 辅助语言                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| 汇编器/编译器/解释器/宏处理器（Assembler/Compiler/Interpreter/Macro Processors） | GAS <br> M4 <br> RAGEL IN RUBY HOST                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| 配置语言（Configuration）                                                        | CMAKE <br> INI <br> MAKEFI <br> NX CONFIGURATION FILE <br> NSIS <br> SQUIDCONF <br> TERRAFORM <br> TOML                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| 文本格式化语言（Formatting）                                                     | GROFF                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| 集成开发环境（IDE）                                                              | NETBEANS PROJECT                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| 模板引擎（Template Engine）                                                      | CHEETAH <br> GENSHI <br> PUG <br> SMARTY <br> VELOCITY                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| 终端/批处理（Terminal/Batch）                                                    | ANT <br> APACHECONF <br> BASH <br> BATCHFILE <br> MAVEN <br> POWERSHELL <br> RPMSPEC <br> SINGULARITY <br> TCSH <br>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| 多语种国际化服务（Translational）                                                | GETTEXT CATALOG                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| 小组 3：区间 3                                                                   | 数据                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| 数据格式语言（Data）                                                             | BNF <br> DIFF <br> DTD <br> E-MAIL <br> JSON <br> PROTOCOL BUFFER <br> RESTRUCTUREDTEXT <br> TEXT ONLY <br> XSLT <br>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |

<a id="表A2"><a/>

### 表 A2：列入全球工资的前 30 个国家

| 国家/地区（Country/Region）                                                                                                                                                                                                                                                                                                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| United States <br> China <br> Germany <br> India <br> United Kingdom <br> Brazil <br> Russia <br> France <br> Canada <br> Japan <br> South Korea <br> Netherlands <br> Spain <br> Poland <br> Australia <br> Sweden <br> Ukraine <br> Italy <br> Switzerland <br> Indonesia <br> Taiwan <br> Colombia <br> Argentina <br> Mexico <br> Norway <br> Belgium <br> Denmark <br> Finland <br> Vietnam <br> Austria <br> |

注：前 30 个国家/地区按 GitHub 用户份额升序排序，其中包括 2020 年 88% 的 GitHub 活动。

<a id="表A3"><a/>

### 表 A3：使用区间 1 和 2 语言的开源的劳动力市场价值

|                | 供给方劳动力市场价值 | 需求方劳动力市场价值 |
| -------------- | -------------------- | -------------------- |
| 工资：低       | $12.3 亿美元         | $2.60 万亿美元       |
| 工资：全球平均 | $41.8 亿美元         | $8.84 万亿美元       |
| 工资：高       | $62.6 亿美元         | $13.24 万亿美元      |

注：高工资情景基于美国的平均工资，低工资情景基于 2020 年印度程序员的平均工资。全球工资是[表 A4](https://hackmd.io/7O2fpfsAQGiFfYFEPN4eNQ?view#%E8%A1%A8-A4%EF%BC%9A%E4%BD%BF%E7%94%A8%E5%8C%BA%E9%97%B4-1%E3%80%812-%E5%92%8C-3-%E8%AF%AD%E8%A8%80%E7%9A%84%E5%BC%80%E6%BA%90%E7%9A%84%E5%8A%B3%E5%8A%A8%E5%8A%9B%E5%B8%82%E5%9C%BA%E4%BB%B7%E5%80%BC) 中各国的平均工资。估计值仅包括第 1 和第 2 区间的语言（见 [表 A1](#表A1)）。

<a id="表A4"><a/>

### 表 A4：使用区间 1、2 和 3 语言的开源的劳动力市场价值

|                | 供给方劳动力市场价值 | 需求方劳动力市场价值 |
| -------------- | -------------------- | -------------------- |
| 工资：低       | $18.8 亿美元         | $3.52 万亿美元       |
| 工资：全球平均 | $64.1 亿美元         | $11.96 万亿美元      |
| 工资：高       | $95.9 亿美元         | $17.91 万亿美元      |

注：全球工资是 **_表 A4_** 中各国的平均工资。估计值仅包括 **_区间 1、2 和 3_** 的语言（见 [表 A1](#表A1)）。

<a id="表A5"><a/>

### 表 A5：商品篮--等效的开源软件和专有软件

| 开源软件           | 专有软件               |
| ------------------ | ---------------------- |
| Apache HTTP Server | Windows Server 2008    |
| Audacity           | Adobe Audition         |
| Blender            | Autodesk Maya          |
| Elasticsearch      | Amazon Kendra          |
| FileZilla          | SmartFTP               |
| FreeCAD            | AutoCAD                |
| GIMP               | Adobe Photoshop        |
| GNU Octave         | MATLAB                 |
| GnuCash            | QuickBooks             |
| KeePass            | 1Password              |
| LibreOffice        | Microsoft Office Suite |
| MariaDB server     | Microsoft SQL Server   |
| Metabase           | Tableau                |
| MySQL              | Oracle MySQL           |
| OpenVPN            | ExpressVPN             |
| PSPP               | SPSS                   |
| Redis              | Redis Enterprise       |
| TensorFlow         | TensorFlow Enterprise  |
| VirtualBox         | VMware Workstation     |
| VLC Media Player   | CyberLink PowerDVD     |

<a id="表A6"><a/>

### 表 A6：使用区间 1、2 和 3 类语言的开源的商品市场价值

|                | 商品-需求区间 1 | 商品-需求区间 1-2 | 商品-需求区间 1-3 |
| -------------- | --------------- | ----------------- | ----------------- |
| 工资：低       | $1.77 亿美元    | $1.79 亿美元      | $2.42 亿美元      |
| 工资：全球平均 | $1.77 亿美元    | $1.79 亿美元      | $2.42 亿美元      |
| 工资：高       | $1.77 亿美元    | $1.79 亿美元      | $2.42 亿美元      |

注：高工资情景基于美国的平均工资，低工资情景基于 2020 年印度程序员的平均工资。全球工资是 [表 A4](https://hackmd.io/7O2fpfsAQGiFfYFEPN4eNQ?view#%E8%A1%A8-A4%EF%BC%9A%E4%BD%BF%E7%94%A8%E5%8C%BA%E9%97%B4-1%E3%80%812-%E5%92%8C-3-%E8%AF%AD%E8%A8%80%E7%9A%84%E5%BC%80%E6%BA%90%E7%9A%84%E5%8A%B3%E5%8A%A8%E5%8A%9B%E5%B8%82%E5%9C%BA%E4%BB%B7%E5%80%BC) 中各国的平均工资。估计值仅包括 **_区间 1、2 和 3_** 的语言（见 [表 A1](#表A1)）。

## 附录 A）： 商品市场估值法

作为另一种估算方法，我们不使用人工重置成本，而是使用商品重置价值法。我们找出几个有类似闭源商业替代品的开源软件包，并考虑如果免费开源软件的所有商业用户都必须用付费替代品取代该软件所需的成本（类似于 Greenstein 和 Nagle（2014 年）以及 Murciano-Goroff 等人（2021 年）对网络服务器进行的计算）。然后，我们可以使用 **_p_** 的替代值，结合上述 **_q_** 值，估算出开源软件的商品替代值。这种方法基于 Nordhaus（2006 年，第 146 页）的建议，他说："……市场和非市场商品和服务的价格应根据可比市场商品和服务来估算。我们并不指望这两种方法得出的估算值会相似。恰恰相反，这两种方法的价值差别很大，因为后一种商品-市场方法假定了一种商品多次销售的固定价格，而这一固定价格通常低于劳动力方面重新创造所有软件包所估算的总价值。这些估算值之间的差异主要是由于一家公司介入重制缺失的开源软件包，然后以商用价格出售，而不是所有公司都需要从头开始重制这些软件包。

&nbsp;&nbsp;&nbsp;&nbsp; 采用商品市场法的思想实验是，我们生活在一个不存在开源软件的世界里，所需软件必须通过一家公司重新创建，然后由该公司为目前免费的商品定价。为了通过商品市场法对开源软件进行估值，我们创建了一篮子在公开市场上定价的等价替代专有商品，作为开源软件产品的替身。这种方法与之前文献（Greenstein 和 Nagle，2014 年；Murciano-Goroff 等人，2021 年）中使用的方法一致，不过这两项研究都只使用了单一商品而不是一篮子商品，因为它们只关注一种开源的网络服务器软件。由于没有现成的开源软件与专有软件等价物数据库，我们根据对开源软件受欢迎程度的主观感受进行搜索，然后再搜索这些开源软件的闭源软件商业替代品。结果，由 20 个开源软件包和专有商业替代品组成的一篮子软件很好地代表了开源软件的多样性。这些软件包括媒体和设计软件、统计分析程序、数据库管理和网络服务器软件等 [^21]。

&nbsp;&nbsp;&nbsp;&nbsp; 根据我们的开源软件等价替代专有商品篮子，我们获得了每个专有软件等价物的价格，并计算了篮子中每个开源软件产品的 COCOMO 劳动力市场供给方价值，在缺乏专有软件代码的情况下，我们用它来替代专有软件的 COCOMO 劳动力供给方价值（例如，支付一名程序员从头开始编写该专有软件所需的成本）。然后，我们计算出篮子的平均 COCOMO 劳动力供给方价值

<div style="margin-right: auto; width: 10%">

![image](https://hackmd.io/_uploads/BJHuH9gRa.png)

</div>

和篮子的平均价格

<div style="margin-right: auto; width: 10%">

![image](https://hackmd.io/_uploads/HJoYrqxCp.png)

</div>

[^22]。由于我们知道所有开源软件的劳动力市场供给方价值

<div style="margin-right: auto; width: 10%">

![image](https://hackmd.io/_uploads/r195BcxAa.png)

</div>

，因此我们可以设置以下等式，并通过简单的比例变换得到所有开源软件在商品市场上的价格 **_Ps_**：

![image](https://hackmd.io/_uploads/rJa-85lCa.png)

这就产生了以下商品市场供给方价值：

![image](https://hackmd.io/_uploads/H13QU9x0p.png)

这样，我们就可以得到需求方商品市场的等值如下：

![image](https://hackmd.io/_uploads/SkPII9lRT.png)

&nbsp;&nbsp;&nbsp;&nbsp; 从商品市场方面来看，我们考虑的是，如果一家公司生产了所有现有的广泛使用的开源软件，然后将其出售给客户，那么它将收取的同等价格。

&nbsp;&nbsp;&nbsp;&nbsp; [表 A6](#表A6) 第 3 栏显示，不同类别的需求价值在 1.77 亿美元到 2.44 亿美元之间，与程序员的原籍国 无关。当然，商品市场价值将大大小于劳动力需求价值，因为这家假想的公司将以相对较低的价格生产软件，然后销售给许多客户，从而获利。此外，Greenstein 和 Nagle（2014 年）以及 Murciano-Goroff 等人（2021 年）只关注一种特定类型的软件（网络服务器），而我们试图将他们的方法扩展到多种商品。然而，在这种情况下，数据限制成为一个更重要的制约因素，这使得通过这种方法估算价值变得更加困难，同时需要更多的假设。与纯粹的商品市场方法相比，这需要劳动力市场方法在估算比例方面提供帮助，最终导致对开源软件价值的大幅低估。此外，专有软件同行的定价策略对市场需求非常敏感。由于商品-市场方法可扩展到多种商品，因此一个强有力的隐含假设是，我们一篮子软件和样本开源软件的市场需求是相似的，因此它们会导致相称的价格。

&nbsp;&nbsp;&nbsp;&nbsp; 另一种更简化的商品市场回溯计算方法是将参考商品的价格与使用量相乘，这种方法不考虑代码行数，也不依赖劳动力市场方法的比例。我们可以将参考价格向量 **_p_** = (69.99, 1610.17, 5800) 中的一篮子专有商品的最低价、平均价和最高价与 **_普查_** 和 "**_BuiltWith_**" 联合样本（[表 1](#表1)）中的使用量相乘。根据这些推算出的专有价格假设，商品市场需求方的价值范围为 0.2 - 16.5 万亿美元（最低价格 - 最高价格），平均价格的价值估计为 4.5 万亿美元。然而，与劳动力市场方法相比，这种估算方法产生的差异略大。然而，由于假定每个开源产品的估算价格都与参考价格相同，因此这种估算方法存在固有缺陷。我们还认为，这种非常简单的 "反包络法 "是一种 "橘子与苹果" 的比较，因为我们篮子中的商品是功能齐全的独立软件包，而 **_普查_** 和 "**_BuiltWith_**" 数据集中的软件包是由应用程序库组成的，这些应用程序库通常比这种独立软件包小。

&nbsp;&nbsp;&nbsp;&nbsp; 由于缺乏商品市场法的数据，我们必须做出各种复杂的假设，因此我们强调正文中强调的劳动力成本法。不过，为了完整起见，我们还是在此介绍这种方法。

## 相关阅读

【[如何使开源项目增长 10 倍，收入增长 5 倍](https://https://mp.weixin.qq.com/s/GQVNAy9nUwPq6nHRpN3n1w)】
【[Cloudstack 证明了：基金会是创建自由和开放源码软件社区的途径](https://https://mp.weixin.qq.com/s/apNdPsYh3sr5g8_OzIeypw)】
【[重新审视开源治理模式](https://https://mp.weixin.qq.com/s/K3xwrWleWHG5_yS0qAJThA)】

[^1]: 数据收集和汇总的具体方法详见 Nagle 等人的 **_普查_** 报告（2022 年）。

[^2]: 开源软件的使用许可证有很大差异，有些许可证非常开放，允许以任何方式重复使用代码，包括在以非零价格出售的专有代码中重复使用，而另一些许可证则限制重复使用，只有在产生的代码根据相同的开源软件许可证发布时才允许重复使用（称为 copyleft -- "公共版权" 或 "著佐权"）。关于开源软件许可证的详细讨论，可参见 Lerner and Tirole (2005) 和 Almeida 等人 (2017)。

[^3]: 间接使用开源软件的情况通过依赖性分析来捕捉，这对于准确衡量一家公司所依赖的开源软件的全部范围是必要的。例如，如果一家公司的专有代码调用了开源软件包 A，而软件包 A 又调用了软件包 B，那么只看直接调用就会发现软件包 B 是该公司专有代码所需的构件。

[^4]: **_普查_** 将开源软件包定义为 "可由软件包管理器安装和管理的软件单元"，并将软件包管理器定义为 "自动安装和管理软件包的软件"（Nagle 等人, 2022）。

[^5]: 在长尾使用分布中，占完整 **_普查_** 数据其余 30% 的软件包未在最终报告中共享，因此无法纳入我们的分析。

[^6]: GitHub 是一个托管和协作平台，贡献者可以用它来协调开源软件项目的开发和发布。GitHub 成立于 2008 年，现已成为全球最大的开源软件开发中心。2023 年 1 月，GitHub 拥有超过 3.7 亿个软件仓库和超过 1 亿名开发人员。除个人用户外，众多私营企业也在积极使用 GitHub 平台，其中包括微软（2018 年收购了 GitHub）、Facebook、谷歌以及其他众多大小公司。

[^7]: 作为健全性检查，我们尝试访问获得的所有代码库 URL，以确保它们处于正常工作状态。对于那些在 GitHub 上无法访问的代码库，我们手动找到了正确的 URL。

[^8]: 作为稳健性检查，我们随机抽取了 50 个从谷歌搜索方法中得出的软件包-代码库匹配结果，并进行了人工检查。所有匹配结果都经人工确认无误，为自动匹配方法提供了额外支持。

[^9]: 由于缺少软件包和软件包管理器名称，因此无法使用 libraries.io 进行精确匹配。技术名称是面向客户的产品名称，与用于内部开发的软件包名称相比，其技术性和精确性可能较低。因此，在 libraries.io 搜索中使用技术名称可能会造成严重的歧义。

[^10]: 匹配率超过 96%，未匹配的代码库仅占我们以下讨论的计算的开源软件需求值的 0.15%。

[^11]: 过滤基于 [GHTorrent](https://github.com/ghtorrent) 的 "虚假用户 "分类，以及任何包含 "机器人" 字样并用特殊字符包围的用户名。这种方法比其他僵尸检测方法（如 [GitHub Innovation Graph](https://innovationgraph.github.com/) 中使用的方法）更为保守，后者依赖于每月提交频率阈值。

[^12]: https://pypi.org/project/pygount/ 以及 https://github.com/github-linguist/linguist

[^13]: 请注意，我们的重点是人工重新编写而非机器人编写的开源软件代码的成本。然而，直接删除机器人账户的所有开源软件贡献在这里是不可行的，因为我们无法观察到机器人账户在 GitHub 上所写代码的确切行数。

[^14]: 在另一个版本中，我们使用了劳动力市场和商品市场的混合方法，这与 Greenstein 和 Nagle（2014 年）和 Murciano-Goroff 等人（2021 年）的研究更为接近。然而，由于数据限制，在我们的环境中应用这种方法需要许多额外的假设。为简单起见，我们将其称为商品市场法，并在 [附录 A](https://hackmd.io/7O2fpfsAQGiFfYFEPN4eNQ?view#%E9%99%84%E5%BD%95-A%EF%BC%89%EF%BC%9A-%E5%95%86%E5%93%81%E5%B8%82%E5%9C%BA%E4%BC%B0%E5%80%BC%E6%B3%95) 中提供了该方法的详细信息、统计数据以及局限性。

[^15]: 我们只使用代码行，不包括文档行和空行。因此，我们低估了重新创建每个软件包的真正价值。

[^16]: 与代表性代理模型类似（如 Williamson 2006），我们可以认为每个软件包都是由不同的程序员创建的，这些程序员是彼此的相同复制品（因此具有相同的技能水平，但不会通过学习提高效率）。

[^17]: 在 Wachs 等人（2022 年）的研究中，共有 179 个国家，但排名前 30 的国家占全球积极贡献国的 88% 以上，其余每个国家所占份额不到 0.6%。[表 A2](#表A2) 列出了前 30 个国家。

[^18]: 我们根据活跃的 GitHub 开发人员数量和软件开发人员的平均基本年薪来选择高薪和低薪参考国家。

[^19]: 附录中的表格显示了 [表 2](#表2) 中包括软件语言**_区间 1 和 2_**（[表 A3](#表A3)）以及所有三个软件语言区间（[表 A4](#表A4)）时的等效值。

[^20]: 由于 **_普查_** 包含专有的客户信息，因此没有显示整个数据集里的行业情况，所以我们只能使用 **_BuiltWith_** 的外向数据来显示各行业的价值。我们将 BuiltWith 网站与 Orbis 和 Compustat 数据集中的行业信息进行匹配。通过这一过程，94.6% 的 BuiltWith 网站与行业信息进行了匹配。对于与多个行业相关的公司（域），我们取其平均值并在各行业间进行分配。

[^21]: [表 A5](#表A5) 显示了我们使用的一篮子开源软件及其专有等同软件。为了建立这个篮子，我们寻找在总体功能和特征集上具有类似开源软件等同物的专有软件，并设法确定软件对，这些软件总体上反映了现有开源软件类型的广泛代表性。

[^22]: 我们使用软件的 3 年使用寿命，即 1/(1-0.66)，得到了商品市场专有篮子的平均价格，因此折旧系数为 0.33。这符合美国国税局（IRS）关于软件折旧的规定，即 "如果你可以折旧计算机软件的成本，请在 36 个月的使用寿命内使用直线法"。https://www.irs.gov/publications/p946#en_US_2022_publink1000107354。
