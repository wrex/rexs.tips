---
date: 2020-03-10T21:14:10-07:00
title: "New Site!"
linkTitle: "New Site"
description: "Announcing Rex's Tips, a docsy themed site."
author: "Rex Walters"
resources:
  - src: "**new-site.jpg"
    title: "New site"
---

Time for a refresh.

{{< imgproc new-site Fill "600x400" >}}
{{< /imgproc >}}

I'm going to retire [the old site](https://lessons.doiwalters.com) and start using this site exclusively going forward. It provides better content organization and allows me to post on any topic (not just guitar). It's **way** easier to maintain versions, backups, branches, etc., and it's trivial for me to deploy new content. What's not to like?

If you're curious about the technical details, I've decided on the following:

* [Hugo](https://gohugo.io) as the static site Generator.
* [LoveIt](https://themes.gohugo.io/docsy/) as the theme for the site.
* [Hover](https://www.hover.com) for my domain registration.
* [Github](https://github.io) for version control
* [Netlify](https://www.netlify.com) for deployment and CDN

As always, this is as much about tinkering as anything.

[Docsy](https://themes.gohugo.io/docsy) helped clarify my thinking about content organization. I finally realized I have at least two types of content I want to publish:

* Time-ordered blog posts about whatever is on my mind. While I want this content tagged/categorized and searchable, it's somewhat ephemeral. The newest content of this type is most interesting. It makes sense to use publish/modify dates as the primary ordering. Navigation of this content is mostly just scrolling further back in time, with occasional searches for a tag or keyword.

* Structured content like tutorials and proficiency tests. This content comprises several pages that may be modified or re-ordered at any time. Neither publish nor modify date makes any sense to establish the order of these pages. This content is structured much more like books or documentation. That's why the [Docsy](https://themes.gohugo.io/docsy/) theme is such a good fit.

[Netlify](https://www.netlify.com) made deploying my site from my [github repository](https://github.com/wrex/rexs.tips) absolutely trivial.

It couldn't be easier for me to publish new content: I just edit a markdown file, commit the changes with git, and push the changes to [github](https://github.com/wrex/rexs.tips). Shazam! The changes are published within a minute or two on the production site, and I have fully version controlled backups both on my local machine and in the cloud (on [Github](https://github.com/wrex/rexs.tips)). Wonderful.

I could have even registered my domain with [Netlify](https://www.netlify.com), to begin with, instead of using [Hover](https://www.hover.com). [Hover](https://www.hover.com) is great, but one stop shopping would also have been nice.

Everything other than domain registration is absolutely free for the little traffic and data I have, too. Hooray!
