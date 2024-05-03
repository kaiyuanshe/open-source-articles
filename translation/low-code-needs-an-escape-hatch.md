---
title: Your Low Code Solution Needs an Escape Hatch
authorURL: ""
originalURL: https://deno.com/blog/low-code-needs-an-escape-hatch
translator: ""
reviewer: ""
---

# Your Low Code Solution Needs an Escape Hatch

<!-- more -->

May 3, 2024[][1]

-   [![](https://github.com/lambtron.png)Andy Jiang][2]

-   [Subhosting][3]

Low-code solutions — visual workflow builders — can offer your users value by significantly reducing development effort and complexity. However, as your platforms’ capabilities grow with more integrations and functionalities, your users will inevitably require more customization to meet their needs. Instead of trying to anticipate and build for every use case, innovative platforms will simply offer an “escape hatch”, letting users write, host, and run custom code specifically designed to solve their problems.

Figuring out where and when to add a customizable code block to your low-code solution is an important product decision, which can require meaningful engineering effort. In this post, we’ll cover three common ways to add a code-level customization escape hatch to your low-code platform:

-   [Internal custom block for data transformation][4]
-   [Custom external HTTP connectors][5]
-   [Custom dashboard and website components][6]

Let’s get started.

## [][7]Internal custom block for data transformation

Most low-code platforms enable workflow automation via a visual drag-and-drop interface. The connectors are generally cloud integrations, and the “blocks” either transform data payloads or trigger events. Common examples include cloud connector workflow builders like Zapier and IFTTT, but this also includes platforms like Descope, a drag and drop user authentication and management tool.

![This low-code example allows you to build a lead scoring system through a drag and drop interface.](/blog/low-code-needs-an-escape-hatch/custom-internal-block-1.png)

This low-code example allows you to build a lead scoring system through a drag and drop interface.

Users may want more flexibility on how they transform or use the data payload during the workflow. For instance, if the workflow is meant to calculate a lead score based on behavior, what if the user wants to pull in data from an external API and use their own algorithm? Or if the workflow is to assess purchase risk and the user has their own method for calculating that? Offering a “block” where the user can write code to have full control over the data is hugely valuable.

![Adding a custom code block in between connectors in a low code workflow builder.](/blog/low-code-needs-an-escape-hatch/custom-internal-block-2.png)

With a custom code block, users can pull necessary data and use their own algorithms tailored to their business to calculate a lead score.

Building this “block” that can take custom code and run it can be tricky, as there are two major considerations: security and performance.

Security means that anyone’s custom code cannot access another users’ environment, any shared global objects, or even your underlying infrastructure. Doing so could result in not only leaking personal data, but also loss of user confidence and trust in your product. When designing your custom code escape hatch, it’s imperative that there are multiple layers of defense in between deployments to maximize security.

Performance is also hugely important. When your user’s custom code block is initiated, there should be minimal cold starts to ensure that the entire workflow happens immediately. For low-code platforms assessing chargeback risk or user authentication, for example, their API responses may initiate business-critical downstream workflows, where every millisecond matters. When evaluating potential technology solutions, determining which has the least cold start time will keep your users happy.

> Run untrusted JavaScript from multiple customers in a secure, hosted sandbox with Deno Subhosting. [Get started for free today][8].

## [][9]Custom external HTTP connectors

Most workflow automation builders offer external HTTP connectors, which allow users to either initiate a workflow via receiving an incoming webhook or to send an HTTP request as part of a workflow. While offering webhooks gives developers a way to integrate third party external services to your platform, [it’s not the best developer experience][10]. The onus is on the developer to standup and maintain a server (or queues) to ensure webhooks are received and processed properly.

![A low-code workflow using an external HTTP webhook connector.](/blog/low-code-needs-an-escape-hatch/custom-external-http-connector-1.png)

What if your user wants to transform the data before routing it to a third party API? Perhaps that use case is small enough that setting up and maintaining a highly available server is overkill. This user just wants to be able to write a tiny bit of serverless code that runs immediately when called.

In the above scenario, webhooks is just the start of the solution. Savvy platforms go beyond a webhook and offer their users a custom code block that takes the webhook payload and allows code to custom manipulate it with actions like sending another HTTP request to another web service. These little web-based text editors can come loaded with access to specific npm modules so that users can be productive immediately.

![Adding a custom HTTP handler as a block in a low-code workflow builder.](/blog/low-code-needs-an-escape-hatch/custom-external-http-connector-2.png)

For this use case, performance and security again are top concerns. This code needs to be executed immediately, and not have access to any other users’ code blocks, or your underlying infrastructure.

## [][11]Custom dashboard and website components

For low-code dashboard, reporting, and even site-building solutions, oftentimes there are pre-made charts, graphs, or UI components that can ingest and visualize data. Though it’s possible to build every possible chart and component type, it’s hard to predict exactly what your end users need for their use case.

![Typical workflow for using a pre-made chart component in a low-code environment.](/blog/low-code-needs-an-escape-hatch/custom-ui-component-1.png)

One approach is to offer a custom code component where users can build their own chart, graph, or UI widget. This code can either manipulate the data directly and output it in a way that can be parsed by a chart or graph, or it can even give the user control over how to render a chart or graph.

![Adding a custom code block that allows users to build their own UI components.](/blog/low-code-needs-an-escape-hatch/custom-ui-component-2.png)

By allowing your users to create custom UI components with code, it saves engineering resources from having to anticipate and build for a wide range of potential use cases. For instance, [Brazil’s top e-commerce platform][12] offers both a low-code wysiwyg site editor _and_ the ability to edit raw code to create re-usable, composable widgets for store fronts. This escape hatch provides their users the most control and flexibility when it comes to building customized solutions to fit their needs.

## [][13]Deno Subhosting: securely run untrusted JavaScript with minimal cold starts

While you can build your own infrastructure to run untrusted code, there is a significant design complexity when it comes to maximizing security and minimizing cold starts. [Deno Subhosting][14] was [designed from the ground up with security in mind][15], is [more performant than using AWS Lambda][16], and is battle tested as it supports enterprise use cases such as [Netlify that process over 255m requests per day][17].

If you’re interested in launching custom code widgets in your low-code platform in weeks and not months, [check out Deno Subhosting for free today][18].

[1]: /feed "Atom Feed"
[2]: https://github.com/lambtron
[3]: /blog?tag=subhosting
[4]: #internal-custom-block-for-data-transformation
[5]: #custom-external-http-connectors
[6]: #custom-dashboard-and-website-components
[7]: #internal-custom-block-for-data-transformation
[8]: /subhosting
[9]: #custom-external-http-connectors
[10]: /blog/webhooks-suck
[11]: #custom-dashboard-and-website-components
[12]: /blog/deco-cx-subhosting-serve-their-clients-storefronts-fast
[13]: #deno-subhosting-securely-run-untrusted-javascript-with-minimal-cold-starts
[14]: /subhosting
[15]: /blog/subhosting-security-run-untrusted-code
[16]: /blog/subhosting-vs-lambda
[17]: /blog/netlify-subhosting
[18]: /subhosting