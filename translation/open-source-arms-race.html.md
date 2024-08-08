---
title: Open Source Arms Race
date: 2020-05-05T00:00:00.000Z
authorURL: ""
originalURL: https://www.yegor256.com/2020/05/05/open-source-arms-race.html
translator: ""
reviewer: ""
---

Please, cite this blog post via [BibTeX][1] as such:

<!-- more -->

@misc{bugayenko2020blog0505,
author = {Bugayenko, Yegor},
title = {{Open Source Arms Race}},
howpublished = {\\url{https://www.yegor256.com/200505.html}},
year = {2020},
month = {may},
note = {\[Online; accessed 08-07-2024\]}
}

Some companies massively invest in open source software projects, while others still remain skeptical and stay away from this trend. What’s in it for those philanthropists, like Google, IBM or Microsoft? Why spend money on something that doesn’t belong to them and is shared among all of us developers? Don’t they understand that the code they write may be used by their competitors? It seems they do understand, but can’t do anything about it.

![Filth (2013) by Jon S. Baird](/images/2020/05/filth.jpg)

Filth (2013) by Jon S. Baird

As David Mytton [noted][2], individuals release open source projects out of altruism, while companies have real, strategic reasons hidden behind the warm and fuzzy glow of open source. We don’t mean just using open source products, which is what every business [does][3] nowadays, but building them so that everybody can use them, for free.

First, let’s see exactly how, among [other methods][4], companies invest in open source:

- **Committers**. Google, for example, encourages its employees to open their code, and even has an [approval procedure][5] for it. It seems that others do something similar. Some recently published [research][6] demonstrates that thousands (!) of employees from [Microsoft][7] (4.3k visible GitHub contributors), [IBM][8] (2.3k), [Google][9] (1.2k), and [others][10] actively contribute to their GitHub-hosted repositories. In other words, being paid by Google these people write code that doesn’t belong to Google.
- **Events**. Aside from [Google Cloud Next][11], [AWS re:Invent][12], and [Microsoft Ignite][13], which are pure promotional events, tech giants sponsor community-driven conferences, like [DockerCon][14], [KubeCon][15], [FOSDEM][16], and so on.
- **Foundations**. [Apache][17], [Linux][18], [Eclipse][19], [GNOME][20], [OSI][21] and [others][22] are sponsored by Google, IBM, Huawei, Microsoft, Oracle, and others.
- **Acquisitions**. They [acquire][23] startups that make open source products, e.g. [RedHat][24] (acquired by IBM for [$32b][25]), [MongoDB][26] ([$4b][27]), [Docker][28] ([$1b][29]), [Elastic][30] ([$6b][31]), [Ansible][32] ([$100m][33]), [MySQL][34] ([$1b][35]), [Nginx][36] ([$670m][37]), and [so on][38]. The market is [booming][39], by the way.
- **Donations**. Google, for example, [donates][40] to [Fastlane][41] and [Kubernetes][42]; IBM [donates][43] to [Node.js][44] and [TensorFlow][45]; Amazon sponsors [Rust][46]; and [so on][47].

Next, the question is how this helps Google and others make their business more profitable. For example, how is Google Cloud Platform planning to beat Amazon AWS using open source as a weapon? Here is how, among [other reasons][48]:

- **Selling**. The products they sponsor gather large communities of users, who know how to work with them. Some of those users are decision-making people. For example, [Google’s Container Engine][49] is a hosted version of [Kubernetes][50], an open source product. Kubernetes users, when they need a hosted version of it, will most likely become Google customers. [TensorFlow][51], yet another example, also runs on [Google Cloud Platform][52].
- **Influencing**. In the modern software development world open source is the key media, where programmers learn new ideas, design principles, and architectural solutions. They listen to open source projects, because they trust them much more than they trust Google, IBM or Microsoft. Tech companies are smart, but their decisions are based on monetary reasons, while open source projects are much freer to do what is right, instead of what is profitable. And programmers usually get very skeptical when open projects are acquired by large enterprises, like [Java by Oracle][53] or [GitHub by Microsoft][54] (not really an open source story, but very close). Thus, for companies it’s much wiser to sponsor open source and stay behind the curtain rather than talking directly to developers through corporate media like [MSDN][55] or [OPN][56].
- **Branding**. Being part of open source is a direct contribution to the public image of a company. Google is no longer an [Ad-selling monopoly][57], with [questionable reputation][58], but one of the largest software [philanthropists][59]. Microsoft is [catching up][60] with its massive [code opening][61] and the [purchase][62] of GitHub.

- **Retaining**. Being an active participant of a visible open source software product is a great [intrinsic motivator][64] for the best software engineers. When your company is involved in open source business, you are much more loyal and interested in staying longer with the company. I can’t prove this assertion, but it’s my personal observation.
- **Training**. It’s [no secret][65] that the [best technologies][66] nowadays are being created in open source projects by people contributing for free (they get their salaries somewhere else). It’s also a [well-known fact][67] that in order to be a better engineer one has to work with the best. Open source projects are [exactly][68] the best place to meet more experienced and very often more talented programmers, and learn from them. Companies, by sending people there, boost their skills without doing any internal training programs.

Thus, it seems that open source is a very powerful instrument in the war for tech markets and for talent. Smart companies develop their open source muscles, earning reputation and acquiring our trust. I predict this trend not only to continue but also to escalate. We programmers are their driving force; they need us as users, promoters, influencers, and makers of the products.

They were [not paying attention][69] to the open source territory for ages and [now][70] they are fighting for it, trying to acquire the largest pieces.

We software developers are the territory!

Thus, if you are a coder, make your own project now. Sooner or later Google will knock on the door and offer you a big check, just to do it earlier than Microsoft.

> Why don't you have your own super popular [#opensource][71] product yet?
>
> — Yegor Bugayenko (@yegor256) [December 13, 2020][72]

[1]: https://www.bibtex.org/
[2]: https://www.infoworld.com/article/3028600/whats-the-real-reason-microsoft-and-google-are-releasing-open-source.html
[3]: https://thenewstack.io/survey-open-source-programs-are-a-best-practice-among-large-companies/
[4]: https://opensource.com/article/19/4/ways-support-sustain-open-source
[5]: https://opensource.google/docs/releasing/approval/
[6]: https://www.infoworld.com/article/3253948/who-really-contributes-to-open-source.html
[7]: https://github.com/microsoft
[8]: https://github.com/IBM
[9]: https://github.com/google
[10]: https://www.zdnet.com/article/its-an-open-source-world-78-percent-of-companies-run-open-source-software/
[11]: https://cloud.withgoogle.com/next/sf/
[12]: https://reinvent.awsevents.com/
[13]: https://www.microsoft.com/en-us/ignite
[14]: https://docker.events.cube365.net/docker/dockercon/
[15]: https://events.linuxfoundation.org/kubecon-cloudnativecon-europe/
[16]: https://fosdem.org/2020/
[17]: https://www.apache.org/foundation/thanks
[18]: https://www.linuxfoundation.org/membership/members/
[19]: https://www.eclipse.org/membership/exploreMembership.php#allmembers
[20]: https://www.gnome.org/foundation/
[21]: https://opensource.org/sponsors
[22]: https://opensource.com/resources/organizations
[23]: https://techcrunch.com/2019/01/12/how-open-source-software-took-over-the-world/
[24]: https://github.com/RedHatOfficial
[25]: https://www.technologyreview.com/the-download/612353/ibms-34-billion-purchase-of-red-hat-is-a-mega-bet-on-a-coding-revolution/?via=indexdotco
[26]: https://github.com/mongodb/mongo
[27]: https://www.marketwatch.com/story/mongodb-shares-rally-above-already-elevated-ipo-price-2017-10-19
[28]: https://github.com/docker
[29]: https://venturebeat.com/2015/06/13/docker-now-valued-at-1b-paid-someone-799-for-its-logo-on-99designs/
[30]: https://github.com/elastic
[31]: https://techcrunch.com/2018/10/05/search-company-elastic-pops-90-on-nyse-after-raising-252m-at-a-2-5b-market-cap-in-its-ipo/
[32]: https://github.com/ansible/ansible
[33]: http://venturebeat.com/2015/10/15/source-red-hat-is-buying-ansible-for-more-than-100m/
[34]: https://github.com/mysql
[35]: https://techcrunch.com/2008/01/16/sun-picks-up-mysql-for-1-billion-open-source-is-a-legitimate-business-model/
[36]: https://github.com/nginx/nginx
[37]: https://techcrunch.com/2019/03/11/f5-acquires-nginx-for-670m-to-move-into-open-source-multi-cloud-services/
[38]: https://index.co/market/open-source/acquisitions
[39]: https://a16z.com/open-source-from-community-to-commercialization/
[40]: https://opensource.google/docs/growing/funding/
[41]: https://github.com/fastlane/fastlane
[42]: https://github.com/kubernetes/kubernetes
[43]: https://www.ibm.com/opensource/
[44]: https://xomino.com/2015/06/18/ibm-is-a-platinum-sponsor-of-the-new-node-js-foundation/
[45]: https://conferences.oreilly.com/tensorflow/tf-ca-2019/public/schedule/detail/81284
[46]: https://aws.amazon.com/blogs/opensource/aws-sponsorship-of-the-rust-project/
[47]: https://github.com/ossfriendly/open-source-supporters
[48]: https://simplabs.com/blog/2019/11/11/why-companies-invest-in-oss/
[49]: https://cloud.google.com/kubernetes-engine/
[50]: https://github.com/kubernetes/kubernetes
[51]: https://github.com/tensorflow/tensorflow
[52]: https://cloud.google.com/tensorflow-enterprise
[53]: https://www.reddit.com/r/linux/comments/2e2c1o/what_do_we_hate_oracle_for/
[54]: https://www.theverge.com/2018/6/18/17474284/microsoft-github-acquisition-developer-reaction
[55]: https://docs.microsoft.com/en-us/
[56]: https://developer.oracle.com/
[57]: https://www.theverge.com/2019/9/9/20857440/google-antitrust-investigation-attorneys-general-advertising-search
[58]: https://www.androidauthority.com/googles-reputation-is-becoming-its-biggest-problem-1055381/
[59]: https://ssir.org/articles/entry/open_source_software_is_philanthropy
[60]: https://www.businessinsider.de/international/microsoft-reputation-institute-soaring-research-2019-11/?r=US&IR=T
[61]: https://www.techrepublic.com/article/whats-really-behind-microsofts-love-of-open-source/
[62]: https://blogs.microsoft.com/blog/2018/10/26/microsoft-completes-github-acquisition/
[63]: https://www.youtube.com/watch?v=D12gi1x6Cdw
[64]: https://opensource.com/article/19/11/why-contribute-open-source-software
[65]: https://www.wired.com/insights/2013/11/open-source-a-platform-for-innovation/
[66]: https://www.techrepublic.com/article/the-best-open-source-innovations-of-the-last-decade/
[67]: https://hackernoon.com/how-to-become-the-best-programmer-in-the-world-ef9f584c81fa
[68]: https://www.techrepublic.com/article/10-tips-for-becoming-a-better-programmer/
[69]: https://hbswk.hbs.edu/item/microsoft-vs-open-source-who-will-win
[70]: https://www.computerworld.com/article/3144063/open-source-has-won-and-microsoft-has-surrendered.html
[71]: https://twitter.com/hashtag/opensource?src=hash&ref_src=twsrc%5Etfw
[72]: https://twitter.com/yegor256/status/1338048990907076609?ref_src=twsrc%5Etfw
