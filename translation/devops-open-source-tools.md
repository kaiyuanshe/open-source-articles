---
title: How DevOps teams can get more from open source tools
author: Derek Smart
authorURL: https://enterprisersproject.com/user/derek-smart
originalURL: https://enterprisersproject.com/article/2020/7/devops-open-source-tools
translator: ""
reviewer: ""
---

[Skip to main content][1]

<!-- more -->

[![Supported by Red Hat](/themes/tep/assets/img/l_supported-by-redhat-white.png "Supported by Red Hat")][2]

User account menu

- [Log in][3]
- [RSS][4]

[![Home](/themes/tep/logo.png)][5][![](/themes/tep/assets/img/red_hat_supported_by_red.svg)][6]

A community helping CIOs and IT leaders solve problems

Main navigation

- [Articles][7]
  - [Digital Transformation][8]
  - [Enterprise Technology][9]
    - [Hybrid Cloud][10]
  - [IT Strategy][11]
  - [IT Talent][12]
  - [Kubernetes: Everything You Need to Know][13]
- [CIO Research][14]
  - [HBR Articles][15]
  - [Research/Reports][16]
  - [Resources][17]
  - [Roundtables][18]
  - [What is Digital Transformation?][19]
  - [Automation: The IT Leader's Guide][20]
  - [DevOps: The IT Leader's Guide][21]
  - [Hybrid Cloud: The IT Leader's Guide][22]
  - [The Ultimate DevOps Hiring Guide][23]
- [What is an Enterpriser?][24]
  - [Meet the Enterprisers][25]
  - [Meet the Team][26]
- [About This Project][27]

# How DevOps teams can get more from open source tools

To get the best from DevOps, tackle your open source strategy in two dimensions: horizontal and then vertical. Consider this advice on tools and approaches that work

By

[Derek Smart][28]

July 2, 2020 | %t min read

![](/themes/tep/assets/img/icon-printer.svg)

![Devops gears laptop](data://image/svg+xml;charset=utf-8,%3Csvg%20xmlns%3D'http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg'%20viewBox%3D'0%200%201%201'%2F%3E "Devops gears laptop")

[Open source][29] software development is rapidly becoming a staple in [DevOps][30] teams’ toolkits. Open source software (OSS) allows organizations to — especially at the beginning of their journey — avoid the cost of expensive proprietary software that might not scale with the business or become obsolete as time goes on. While cost savings are an obvious draw, it’s actually the flexibility of open source that makes it such a great fit for DevOps.

**\[ Need to explain key DevOps terms to others? Get our cheat sheet: [DevOps Glossary.][31] \]**

Software teams today are tasked with delivering [automation][32] across a diverse set of DevOps workflows. They must support a broad portfolio of applications and tools, while also serving the needs of different personas, inlcuding developers, SREs, and QA testers. The characteristics of open source software very much lend themselves to meeting these challenges, as OSS can be much easier (and cheaper) to integrate with elements in your pipeline than other solutions.

That’s why [entire communities][33] have now coalesced around these tools, and can provide essential guidance and support for others’ journeys.

**\[ Check out our sibling site, [Opensource.com][34], for open source and Linux tutorials, advice, and resources. \]**

Whether you need to connect your continuous integration server with your configuration management tool or something else, there’s probably already a playbook for that. These synergies have led to the creation of many open-source DevOps tools, many of which are now widely adopted and used (full disclosure: I work for [Delphix][35], which has its own open source project).

**\[ Read also: [5 open source tools IT leaders should know about now][36] and  [DevOps engineers: Common misconceptions about the role][37]. \]**

From working with dozens of DevOps teams across Fortune 500 companies — as well as our own internal use of OSS tools — I’ve found that teams need to approach open-source strategy in two dimensions: horizontal and then vertical. Here’s what I mean:

## Build horizontal: Focus on automation and speed 

Continuous integration and continuous delivery or deployment ( [CI/CD][38]) is the holy grail of software — many are seeking it, but few have found it. Open source tools can be a key first step on the DevOps path to achieving software development’s nirvana state, but only when teams bring automation and speed across the various steps of the process. That’s why professionals refer to a DevOps “toolchain” (the products you use) that supports the software “pipeline” (the process of delivering software) — and visually depict these elements as unfolding in a horizontal fashion.

End-to-end tool coverage horizontally across an organization is the key to highly functional, mature DevOps practices. However, that’s easier said than done — and has traditionally been both expensive and difficult for businesses to do. The good news today is that there are many more open-source options across every sequential step of the software delivery lifecycle (SDLC). From managing source code, to storing build artifacts, release monitoring and finally to deployment — there’s an OSS solution for that if you know where to look.

Our DevOps team uses tools like [Review Board][39], [Artificatory][40], [Jenkins][41], and Terraform to bring automation and speed to development for faster releases.

**\[ Read also: [5 open source projects that make Kubernetes even better][42]. \]**

## Go vertical: Add control to every layer of DevOps

Once you’ve leveraged open source tools to build speed and automation across the organization’s SDLC, what’s next? Perhaps less obvious is the notion that DevOps teams must think about tool coverage and instrumentation for a vertical stack, which at a basic level breaks down into code, infrastructure, and data layers. While the instantiation of these elements varies across different phases of the SDLC, these layers exist in one form or another at nearly every step of your DevOps practice.

For example, early in the SDLC the stack may be composed of a few lines of code, running on a laptop and tiny MySQL database containing dummy data. However, later in the life cycle the stack may equate to a fully-built production application on cloud infrastructure-as-service, and talking to a terabyte of data. Regardless of its composition, teams need to bring control and automation across all vertical stack elements in the SDLC.

Again, the good news is that there’s a preponderance of OSS tools that can help, from [Git][43] (code) to [Ansible][44] and Salt (infrastructure) to [Liquibase][45], [Flyway][46], and [Titan][47] (data). This is important because teams must bring speed, control, and automation to every layer of their DevOps practice, lest one becomes a bottleneck that holds up the entire train.

To add another example, it’s great to be able to automatically provision and configure your build on cloud-based test infrastructure in a matter of minutes. But if it still takes days to deliver test data to that cloud environment, you risk creating the illusion of speed but not speed itself.

That’s why each layer of the DevOps operation — from top to bottom — must be addressed to ensure the development process flows from one step to the next, without drag.

## Open source state of mind

MORE ON DEVOPS

- [Agile vs. DevOps: What’s the difference?][48]
- [DevOps culture: 5 questions to ask about yours][49]
- [DevOps metrics: Are you measuring what matters?][50]

Whether you’re brand new to DevOps or a savvy veteran, solving for the right toolset to build out a modern software delivery pipeline can be intimidating. OSS can provide all the constituent pieces you need to make integration less daunting, but you must also have the right mindset.

Remember, you’re not just populating an array of open source tools — you’re actually building an array of arrays. Think about automation and speed in two dimensions instead of one, and address bottlenecks that can slow you down in each step of the DevOps process. Do that, and you’ll be right on your way to using open source for a highly-automated, lightning fast CI/CD pipeline.

**\[ How can automation free up more staff time for innovation? Get the free eBook: [Managing IT with Automation][51]. \]**

Topics

[IT Strategy][52]

[DevOps][53]

[Open Source][54]

![](/sites/default/files/styles/150x150/public/pictures/derek-smart.jpg?itok=Tnr1xNDS)

Derek Smart is a Senior Staff Engineer with Delphix. Derek is an experienced software developer with a skill set that ranges in API design, architecture, user experience, PHP, TDD, and DevOps. He has a demonstrated history of helping companies across industries transition to CI/CD.

[More about me][55]

## Related content

[![Harvard Business Review How to Keep Your Top Talent CIO](/sites/default/files/styles/222x125/public/images/How_To_Keep_Your_Top_Talent_HP.png?itok=CPayBNgE "Harvard Business Review How to Keep Your Top Talent CIO")][56]

[Reimagining employee retention: 4 tips][57]

[![Harvard Business Review Top 5 articles for October 2015](/sites/default/files/styles/222x125/public/images/Harvard%20Business%20Review%20Top%205.png?itok=qoxmFIPl "Harvard Business Review Top 5 articles for October 2015")][58]

[5 Harvard Business Review articles that will resonate with CIOs right now][59]

[![](/sites/default/files/styles/222x125/public/images/cio_managing_remote_teams.png?itok=JbBeXFfG)][60]

[Remote work: 3 pros and 3 cons][61]

## Comments

ekta garg | July 6, 2020

Nice article!

## About This Site

The Enterprisers Project is an online publication and community helping CIOs and IT leaders solve problems.

The opinions expressed on this website are those of each author, not of the author's employer or of Red Hat. [The Enterprisers Project][62] aspires to publish all content under a [Creative Commons license][63] but may not be able to do so in all cases. You are responsible for ensuring that you have the necessary permission to reuse any work on this site. Red Hat and the Red Hat logo are trademarks of Red Hat, Inc., registered in the United States and other countries.

While The Enterprisers Project welcomes [proposals for contributed articles][64] from community members, it does not accept solicitations for advertising on the site or in any of its newsletters.

## Connect

[RSS Feed][65]

Copyright ©2022 Red Hat, Inc.

Legal

- [Privacy Statement][66]
- [Terms of use][67]
- [Contact][68]

[1]: #main-content
[2]: https://www.redhat.com/en?intcmp=701600000011jKuAAI
[3]: /user/login?current=/article/2020/7/devops-open-source-tools
[4]: /rss "rss"
[5]: /
[6]: https://www.redhat.com/en?intcmp=701600000011jKuAAI
[7]: /
[8]: /tags/digital-transformation
[9]: /tags/enterprise-technology
[10]: /tags/hybrid-cloud
[11]: /tags/it-strategy
[12]: /tags/it-talent
[13]: /article/2020/4/kubernetes-everything-you-need-know
[14]: /cio-research
[15]: /cio-research/hbr-articles
[16]: /cio-research/researchreports
[17]: /cio-research/resources
[18]: /cio-research/roundtables
[19]: /what-is-digital-transformation
[20]: /it-automation
[21]: /devops
[22]: /hybrid-cloud
[23]: /ultimate-devops-hiring-guide
[24]: /what-enterpriser
[25]: /meet-enterprisers
[26]: /meet-contributors
[27]: /about-this-project
[28]: /user/derek-smart
[29]: https://www.redhat.com/en/about/open-source?intcmp=701f2000000tjyaAAA
[30]: https://enterprisersproject.com/taxonomy/term/76
[31]: https://enterprisersproject.com/cheat-sheet-devops-glossary?intcmp=70160000000h0aXAAQ
[32]: https://enterprisersproject.com/taxonomy/term/66
[33]: https://www.reddit.com/r/devops/
[34]: https://opensource.com/
[35]: https://www.delphix.com/
[36]: https://enterprisersproject.com/article/2020/5/5-open-source-tools-it-leaders
[37]: https://enterprisersproject.com/node/14161?intcmp=70160000000h0axaaq
[38]: https://www.redhat.com/en/topics/devops/what-is-ci-cd?intcmp=701f2000000tjyaAAA
[39]: https://www.reviewboard.org/
[40]: https://jfrog.com/artifactory/
[41]: https://www.jenkins.io/
[42]: https://enterprisersproject.com/article/2020/5/kubernetes-5-open-source-projects-improve?intcmp=70160000000h0aXAAQ
[43]: https://git-scm.com/
[44]: https://www.ansible.com/
[45]: https://www.liquibase.org/
[46]: https://flywaydb.org/
[47]: https://titan-data.io/
[48]: https://enterprisersproject.com/article/2019/1/agile-vs-devops-whats-difference
[49]: https://enterprisersproject.com/article/2020/1/devops-culture-5-questions
[50]: https://enterprisersproject.com/article/2017/7/devops-metrics-are-you-measuring-what-matters
[51]: https://www.redhat.com/en/engage/automated-enterprise-ebook-20171115?intcmp=701f2000000tjyaAAA
[52]: /tags/it-strategy
[53]: /tags/devops
[54]: /tags/open-source
[55]: /user/derek-smart
[56]: /article/2023/4/employee-retention-tips
[57]: /article/2023/4/employee-retention-tips
[58]: /article/2023/4/5-hbr-articles-cios
[59]: /article/2023/4/5-hbr-articles-cios
[60]: /article/2023/4/remote-work-pros-cons
[61]: /article/2023/4/remote-work-pros-cons
[62]: http://enterprisersproject.com "The Enterprisers Project"
[63]: http://creativecommons.org/licenses/ "Creative Commons license"
[64]: https://enterprisersproject.com/how-contribute
[65]: http://www.enterprisersproject.com/rss
[66]: /privacy
[67]: /terms-and-conditions
[68]: /contact
