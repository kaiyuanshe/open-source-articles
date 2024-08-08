---
title: Feross
date: 2019-08-28T00:00:00.000Z
authorURL: ""
originalURL: https://feross.org/funding-experiment-recap/
translator: ""
reviewer: ""
---

# [Feross][1]

<!-- more -->

# [Recap of the \`funding\` experiment][2]

By [Feross Aboukhadijeh][3] Tagged with

- [node.js][4]
- [javascript][5]

I’m ending the `funding` experiment I [introduced][6] a few days ago.

The idea was this: whenever users install open source software, the `funding` package would display a message from a company that supports open source. The sponsorship would pay directly for maintainer time. That is, writing new features, fixing bugs, answering user questions, and improving documentation.

![npm install funding](/images/funding-screenshot.png)

I appreciate the thoughtful discussion and feedback from the community. I’d like to share some thoughts about how the experiment went from my perspective.

## The problem

Open source maintainers need income to fund their work.

### Where did this start?

My objective was to try a new way to fund open source beyond just asking for donations. I’ve spent over 3,000 unpaid hours over the last four years maintaining some popular open source packages.

More broadly, I wanted to start a conversation about cultural norms around open source consumption.

Right now, the status quo is that **maintainers create massive amounts of value and then for-profit companies and SaaS startups [capture almost all of it][7].**

As a case in point, let me tell you a story from the [Open Source Summit][8] conference I attended last week. While walking through the vendor area, I asked one of the startup reps “how much did you pay for this sponsor booth?” They weren’t sure if it was $10,000 or $20,000. This startup’s product is a `package.json` checker that tells companies if the open source software they’re using is permissively licensed (i.e. MIT, BSD, or Apache). They charge $50 per developer per month for this.

So this means that they charge a 50-person startup a whopping $30,000 per year to help them feel safe using code that open source authors like me have _given away for free_.

Meanwhile, the median startup likely contributes $0 per year to support open source maintainers.

I hold no grudge against this company – it seems like they’ve built a good product. But you have to admit, **the fact that businesses will pay thousands of dollars for some SaaS software while ignoring the maintainers who write _the actual open source code itself_ seems a bit unfair.**

Maintainers do critical work which enables companies to create billions of dollars in value, yet we capture none of that value for ourselves.

Does it have to be like this?

I’m not arguing that maintainers should start capturing _all_ of the value that we create. But we shouldn’t capture literally _none_ of the value either. The status quo is not tenable.

I would love to find a way to help maintainers capture at least _a bit_ of the value we create so that we can happily continue to write new features, fix bugs, answer user questions, improve documentation, and release innovative new software.

### “Sustainability” only means subsistence

Increasingly, maintainers are starting to go through a mindset shift. We don’t want to ask politely for donations anymore – donations that often never come, or when they do they’re usually only enough for maintainers to _sustain_ themselves but never enough to actually _thrive_.

_Sustainability_ is another way to say _subsistence_. This is why the common phrase “open source sustainability” isn’t ideal.

I like what Kyle Mitchell wrote in [Profit for Us, Sustainability for You][9]:

> “Profit” has a bad rep, in part because we don’t sully wages and fees for honest work by individuals with the term, even when they exceed immediate needs. **It’s possible to profit without exploiting anyone. In fact, profit tends to show that you yourself aren’t being exploited.** Your abilities, not your patron or your donors, should decide what kind and quality of life you can manage, and where. Value is leverage.

We should set our goals higher than _subsistence_. Folks who work on open source have a right to _thrive_ and to be fairly compensated for our labor.

Remember: most open source maintainers can get a six-figure job relatively easily (in the SF bay area) where they’re just helping one company instead of helping the public. The opportunity cost is huge. We should be able to do what we want to help the public without making such a difficult choice.

### Do we dare to hope for something better?

As long as significant personal sacrifice is a prerequisite for open source participation, we’ll continue to exclude a lot of smart and talented folks. This isn’t good for anyone.

And we’re forcing the folks who _are_ able to participate to make extreme sacrifices that [inevitably lead to burnout][10]. Freeloading companies think they benefit from the current state of affairs. But maintainer burnout results in abandoned packages, ignored issues, unpatched security bugs, ecosystem churn, and more work for all of us. This is classic tragedy of the commons.

**The dirty secret of open source is that much of it is powered by maintainer guilt.**

As [Dominic Tarr][11] said after the `event-stream` [compromise][12]:

> If it’s not fun anymore, you get literally nothing from maintaining a popular package.

But what if this weren’t the case?

What if anyone could make a living working on open source without needing to [move to Thailand for lower cost-of-living][13], or needing to [sell their startup and use the proceeds to work on open source full-time for four years][14], or needing to [move to Hawaii to create a solar-powered farm and live frugally with near-zero income][15]?

How much healthier and vibrant would the ecosystem be if less self-sacrifice was required? How many more people would be able to join in the fun and opportunity of open source?

## What I’ve already tried

Starting in 2018, I began trying lots of different ways to raise funding so I could justify continuing to do open source full-time. The opportunity cost of forgoing a six-figure tech job are huge, especially when you live in the SF bay area.

Here are a few of the things I tried:

- [`thanks`][16]
- [Patreon][17]
- [Tidelift][18]
- [GitHub Sponsors][19]
- Paid consulting

With all these put together, I can make it work. But it still feels like a precarious solution. If even I – with my fortunate position – can’t make a _comfortable_ living working on open source, then how is anyone else supposed to make it work?

Lots of maintainers struggle to reach a barely [livable wage][20] via donations. Of course, there are [notable exceptions][21]. But most maintainers are eventually forced to get a job making proprietary software, or at least split their time between open source and proprietary work which is far less beneficial to society. It’s unfortunate, but [GitHub stars won’t pay the rent][22].

[![](https://staltz.com/img/poverty-popularity.png)][23]

A lucky few manage to land day jobs that allow them to work on open source. But most folks have to be more creative – squeezing in time after work, secretly doing open source maintenance at work, or opting out of normal society completely. `#solarpunk`

I’m hopeful that [GitHub Sponsors][24] will make giving donations to maintainers more common. But I still worry a lot about folks who maintain packages that no one installs directly, i.e. transitive dependencies of popular packages. These maintainers have the hardest time.

The most common funding models – donations, README sponsors, or paid consulting – only work if a maintainer can get their appeal in front of users. This [usually][25] goes in a README or on a website.

But reliable, error-free transitive dependencies are invisible. Therefore, the maintainers are invisible, too. And, the better these maintainers do their job, the more invisible they are. No one ever visits a GitHub repository for a transitive dependency that works perfectly – there’s no reason to do so. But a developer investigating an error stack trace might visit the repository if for no other reason than to file an issue. At least then there’s a small chance they’ll see the maintainer’s plea in the README.

We need solutions that work for these folks too.

Maybe ads aren’t the answer – fine. **But telling maintainers to bury their appeals where no one bothers to look is not the answer, either.**

## The story of `funding`

### The seeds of an idea

When trying something new, you can’t plan for everything in advance. Sometimes the quickest way to learn if an idea is good or not is to just try it.

So, here was the rough idea for the `funding` experiment:

At a high level, an open source maintainer should be able to `npm install funding` into their project and start receiving money for their maintenance work.

Maintainers shouldn’t need to pitch fifty companies to find the rare one that is open to the idea of supporting open source financially. This is not work that most maintainers enjoy doing, are actually good at, or should need to do.

Rather than appeal to companies or users for donations – donations that often never come, and when they do, are never enough – `funding` lets maintainers take matters into their own hands. They can directly capture a small portion of the value that they’ve created. Not very much value, but at least not _no value_.

What if someone new to open source could adopt an abandoned package, quickly `npm install funding`, and start earning money for maintaining a package?

Suddenly formerly abandoned packages have a monetary value, and, therefore, a reason to be maintained. Bug fixes, security fixes, and pull requests would be less likely to be ignored. Folks who want to quit their day job to work full-time on open source now have a plausible means to do so. We all win.

What about when tons of sponsor messages start appearing in the terminal? How would this scale?

I had a plan for this. As more folks added `funding` to their packages, many copies of it might end up in the dependency tree. But `funding` de-duplicates the post-install message so it only ever prints one message.

As more maintainers join, `funding` ends up in more dependency trees so the single post-install message has more opportunities to be shown, bringing in more income for everyone. At some point, adding additional maintainers doesn’t help the message appear more times since it’s already showing in almost every install, so adding further maintainers only causes the total income to be split among more maintainers. We’d have to see how this played out. No one knows the value of a sponsor message in the terminal since this has never been tried before. That’s why this was an experiment.

Note that `funding` funnels funds to transitive dependencies much more effectively than any of the current funding approaches! That was an explicit design goal. There are lots of transitive dependencies that are “unpopular” in terms of mind share and GitHub stars, but which are used pervasively and yet invisibly. If this experiment worked, these “invisible maintainers” would have had a way to be rewarded for the value they provide.

### Yuck. How would ads works?

Ads let us leverage the attention of the users of our software. They’re an imperfect solution because they extract value (in the form of a few seconds of attention) from all users equally – both from the open source “makers” as well as the “takers”.

For the record, **`funding` had absolutely no tracking, no data collection, and no code from untrusted third parties.** It was a `console.log` with some fancy formatting. Think of it like a newspaper classified ad. We just print it and hope that maybe some folks will see it.

But even when ads don’t track or collect data, they still feel “icky” to many users.

> Oooo light bulb! Perhaps I should write a script that puts ads on the desktop wallpaper while installing ;) <evil laugh>
>
> I'm all for sponsoring open source but ads during install are just annoying. Please don't. [https://t.co/2knajtL0ay][26]
>
> — James M Snell (@jasnell) [August 25, 2019][27]

Personally, I’m not a huge fan of ads. I wish we could get away from ads as a funding model for free content. I use an ad blocker in my web browser, I install ad blockers on all my family’s computers, and I hope you do too. And yet, I’m pragmatic. I run ads on some of the websites that I’ve built and it helps fund ongoing maintenance work.

I supported anyone who wanted to block the sponsor messages from showing up. Which is why I added an environment variable `OPEN_SOURCE_CONTRIBUTOR=true` so that folks who support open source, whether through direct contributions or financially, could permanently silence the output. Obviously, even “takers” could use the flag, but hopefully the variable name makes them feel at least a little guilty.

## The launch

I quietly launched this on August 19, 2019 without much fanfare. People who I know got in touch to express support.

### The community reaction

Fellow open source maintainers and open source contributors have, by and large, been supportive of the experiment. Open source “consumers”, not so much.

[Paolo Fragomeni][28] said it best:

> No one cool was upset by what [@StandardJS][29] did.
>
> — Paolo F (@heapwolf) [August 27, 2019][30]

Folks who have spent time maintaining a popular open source project know how much time it takes to keep a project “healthy”. There are a constant stream of bugs to fix, new features to consider adding, pull requests to review, security issues in dependencies to resolve, user questions to answer, and underlying platform changes to deal with. Even for simple single-purpose packages, there’s a non-trivial ongoing maintenance burden. Especially when you’re maintaining hundreds of packages, as many in the Node.js community do.

> good
>
> — substack (@substack) [August 25, 2019][31]

Lots of maintainers welcomed the experiment as a much-needed conversation starter. That’s not to say that folks were thrilled with the idea of ads in their terminal. Many supporters expressed their dislike of advertising – even advertising where the sponsors are carefully selected and the implementation does not track users or collect data.

![](/images/funding-vweevers.png)

If nothing else, it’s nice that `funding` forced open source “consumers” – folks who enjoy the benefits of open source software without ever contributing anything back – to reconsider their relationship with open source. I think we successfully pushed back against the entitlement to free labor that is pervasive in the interactions that open source consumers have with maintainers.

![](/images/funding-mixmix.png)

> I love your funding experiment [@feross][32] ❤️ don’t give up. Haters gonna hate.
>
> — Jake Verbaten (@Raynos) [August 25, 2019][33]

> [@feross][34] I'm glad you tried & ran the funding experiment, no matter what flak got thrown your way. :)
>
> — noffle 🌱 (@noffle) [August 27, 2019][35]

### The brigaders

Large numbers of the detractors seemed to come from the [r/programming][36] subreddit who are notoriously anti-JavaScript. A smaller number came from 4Chan and Hacker News. These [drive-by condemners][37] were eager to join in a [pile-on][38] in the `standard` issue tracker. But since these folks were neither users nor contributors to `standard`, I think their opinions should be discounted compared to those of actual users, fellow contributors, and fellow maintainers.

> glob bless [@feross][39] for poking the hornet’s nest tho
>
> — Forrest L Norvell (@othiym23) [August 25, 2019][40]

Folks who contribute nothing don’t get a seat at the table.

[Rich Hickey][41] said it best in [Open Source is Not About You][42]:

> The only people entitled to say how open source ‘ought’ to work are people who run projects, and the scope of their entitlement extends only to their own projects.
>
> As a user of something open source you are not …… entitled to anything at all. You are not entitled to contribute. You are not entitled to features. You are not entitled to the attention of others. You are not entitled to having value attached to your complaints. You are not entitled to this explanation.

### Ending the experiment

> A new idea is delicate. It can be killed by a sneer or a yawn; it can be stabbed to death by a quip and worried to death by a frown on the right man’s brow. – Ovid

Since it seems clear this isn’t going to be the solution that saves us all, I’m ending the experiment. (In fact, it’s already been paused since Saturday when the initial two sponsors backed out.)

> We reconsidered after reflecting on the developer community's reaction. We still passionately support open source software along with [@feross][43], but we'll be more careful about experimenting in the future while continuing to innovate. On that note:[https://t.co/WFrHBFGzul][44]
>
> — Linode (@linode) [August 26, 2019][45]

Both Linode and LogRocket are supportive of exploring new ways to support open source. It’s a bummer this didn’t work out, but I don’t hold it against either of them.

### The future

I have plenty of interest from other sponsors and could keep working on `funding` with them onboard. One sponsor is particularly eager to start running their own terminal ad ASAP.

**But I have other experiments in the works that I’m way more excited to try out.**

And anyway, terminal ads seem like they have a limited lifetime. Specifically, there is an effort underway to replace post-install scripts with a [field in `package.json`][46] for soliciting donations. This will likely lead to the silencing of non-error install script output, which is honestly not a bad idea. The days of free-form post-install solicitations seem numbered. I expect that if npm makes this change they will couple it with automatic reporting of funding calls-to-action during `npm install` so as not to remove one of the few avenues maintainers currently have to reach users.

So while terminal ads may work for a little while longer, there are clearly better paths forward. Onward!

Approximately 100% of the Fortune 500 use open source code. Maintainers are just starting to wake up to our own power. Expect to be surprised. This certainly won’t be the last open source funding experiment.

Despite all the personal attacks against me, I’m really glad I ran this experiment. I think it was worthwhile because it seems to have moved the conversation forward, at least among the more thoughtful folks in the wider community.

I really appreciate the support that folks have shown for experimentation, and all the useful discussions that have resulted! Also, a huge thank you for the words of encouragement and support in the midst of all the harassment. Thank you everyone 🥰 🥰 🥰

**Update:** If you want to read more thoughts about `funding` from someone who’s a much better writer than me, I recommend these posts from Kyle Mitchell:

- [Process of Elimination][47]
- [But You Said I Could][48]

### Thanks for reading! [![RSS Feed Icon](/images/rss.png)][49]

[Introducing \`funding\`][64] [libtorrent adds support for the WebTorrent protocol][65]

[1]: /
[2]: /funding-experiment-recap/
[3]: /about/ "Feross Aboukhadijeh"
[4]: /tag/node.js/
[5]: /tag/javascript/
[6]: /npm-install-funding/
[7]: https://gravitational.com/blog/open-core-vs-saas-intro/
[8]: https://events.linuxfoundation.org/events/open-source-summit-north-america-2019/
[9]: https://blog.licensezero.com/2018/06/14/profit-sustainability.html
[10]: https://nolanlawson.com/2017/03/05/what-it-feels-like-to-be-an-open-source-maintainer/
[11]: https://dominictarr.com/
[12]: https://gist.github.com/dominictarr/9fd9c1024c94592bc7268d36b8d83b3a
[13]: https://sindresorhus.com/
[14]: https://techcrunch.com/2013/12/17/yahoo-acquires-peercdn/
[15]: https://substack.net
[16]: /introducing-thanks/
[17]: https://www.patreon.com/feross
[18]: https://tidelift.com/subscription/pkg/npm-standard?utm_source=npm-standard&utm_medium=readme
[19]: https://github.com/sponsors/feross
[20]: https://staltz.com/software-below-the-poverty-line.html
[21]: https://reference.kemitchell.com/top-donations-developers.html
[22]: https://medium.com/@kitze/github-stars-wont-pay-your-rent-8b348e12baed
[23]: https://staltz.com/software-below-the-poverty-line.html
[24]: https://github.com/sponsors
[25]: https://github.com/zloirock/core-js/issues/548
[26]: https://t.co/2knajtL0ay
[27]: https://twitter.com/jasnell/status/1165662575352172544?ref_src=twsrc%5Etfw
[28]: https://hx.ht/
[29]: https://twitter.com/StandardJS?ref_src=twsrc%5Etfw
[30]: https://twitter.com/heapwolf/status/1166301352009633794?ref_src=twsrc%5Etfw
[31]: https://twitter.com/substack/status/1165742866796183554?ref_src=twsrc%5Etfw
[32]: https://twitter.com/feross?ref_src=twsrc%5Etfw
[33]: https://twitter.com/Raynos/status/1165630071887015937?ref_src=twsrc%5Etfw
[34]: https://twitter.com/feross?ref_src=twsrc%5Etfw
[35]: https://twitter.com/noffle/status/1166212318864166913?ref_src=twsrc%5Etfw
[36]: https://www.reddit.com/r/programming/
[37]: https://blog.licensezero.com/2019/08/26/but-you-said.html
[38]: https://github.com/standard/standard/issues/1381
[39]: https://twitter.com/feross?ref_src=twsrc%5Etfw
[40]: https://twitter.com/othiym23/status/1165709255967510528?ref_src=twsrc%5Etfw
[41]: https://clojure.org
[42]: https://gist.github.com/richhickey/1563cddea1002958f96e7ba9519972d9
[43]: https://twitter.com/feross?ref_src=twsrc%5Etfw
[44]: https://t.co/WFrHBFGzul
[45]: https://twitter.com/linode/status/1166095174516297728?ref_src=twsrc%5Etfw
[46]: https://github.com/npm/cli/pull/187
[47]: https://blog.licensezero.com/2019/08/24/Process-of-Elimination.html
[48]: https://blog.licensezero.com/2019/08/26/but-you-said.html
[49]: https://feross.org/atom.xml "Subscribe to the Feross.org Feed"
[50]: https://twitter.com/feross
[51]: /about/
[52]: https://www.npmjs.com/~feross
[53]: https://github.com/feross
[54]: /thanks/
[55]: /support/
[56]: https://webtorrent.io
[57]: https://webtorrent.io/desktop
[58]: https://standardjs.com
[59]: https://bitmidi.com "Free MIDI files"
[60]: https://play.cash
[61]: https://www.apstudynotes.org/ "AP Notes"
[62]: https://www.apstudynotes.org/essays/ "College Essays"
[63]: https://twitter.com/feross
[64]: /npm-install-funding/ "Previous Post: Introducing `funding`"
[65]: /libtorrent-webtorrent/ "Next Post: libtorrent adds support for the WebTorrent protocol"
