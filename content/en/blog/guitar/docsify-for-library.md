---
date: 2020-05-24T11:03:26-07:00
title: "Docsify your exercise library"
linkTitle: "Docsify your exercise library"
description: "How to publish your own exercise library"
toc_hide: true
author: "Rex Walters"
resources:
  - src: "**.{png,jpg}"
    title: "Image #:counter"
---

I've recently been stealing a bunch of ideas from [Josh at
FretboardAnatomy](https://fretboardanatomy.com) and others to completely revamp
my practice system.

As described in [my page on practice]({{< ref "guitar/Fundamentals/how-to-practice/rexs-system/_index.md" >}}), my
practice system comprises just two things:

1. An **exercise library** (on the computer)
2. A **handwritten note system** (on a set of index cards)

This post is about the first, my **exercise library**.

## Motivation

I strongly prefer handwritten notes while practicing, but because I steal
practice exercises from all over the place ([online
lessons](https://fretboardanatomy.com), [YouTube
videos](https://www.youtube.com/watch?v=HiUOSahhTCI),
[blogs](https://www.justinguitar.com/), _etc_.) and because I often create my
own media files (neck diagrams, notation, audio/video/image files, _etc_.) I
realized I **had** to use computer files for my exercise library.

I could have just used [Google docs](https://www.google.com/docs/about/) or the like 
for my library, but I had several concerns:

* My library would either be one enormous, monolithic document, or a pile of
  disconnected pages
* Revision control would be difficult at best
* I'd have to devise a backup strategy of some sort
* Maintaining a table-of-contents or other navigation that "maintains itself"
  would be hard or impossible
* I'd have to devise a strategy for online/offline usage and synchronization

I wanted something with the following characteristics:

* Mandatory

  * Dirt simple to create/update/delete content
  * Trivial to link/reference anything on the internet or within my own pages
  * Easy, automatic revision control (easy to revert to prior versions, see
    changes, etc.)
  * Easy, automatic backups
  * Usable even if I'm "at a cabin in the woods" with no internet connection
  * No "sole-source" dependencies (I don't want to be stranded if some SaaS
    service goes out of business or disappears for some reason)
  * Free or at least very low cost (no more than a few dollars per month)

* Desirable

  * Open source software with an active, vibrant development community
    (so it's unlikely to be orphaned)
  * As few dependencies and things to learn as possible

Everything described below meets all of these criteria.

## Markdown for content

I knew from the beginning that I wanted to use John Gruber's
[markdown](https://daringfireball.net/projects/markdown/syntax) to create my
content.

Markdown has become a defacto standard for all sorts of things: online forums,
comment systems, software documentation, _etc_.

Markdown uses "source code" for documentation that is almost as readable as the
rendered results.

Markdown turns this:

```markdown
## Markdown for content

I knew from the beginning that I wanted to use John Gruber's
[markdown](https://daringfireball.net/projects/markdown/syntax)
to create my content.

Markdown has become a defacto standard for all sorts of things:
online forums, comment systems, software documentation, _etc_.

Markdown uses "source code" for documentation that is almost as 
readable as the rendered results.
```

Into what you see above. 

> Note that the color coding in the sample markdown is from a "syntax highlighter," and is
> similar to what I see in my text editor as I compose markdown source.

## Git for revision control

Anyone who's ever used any sort of "source code control system" to write
software is probably familiar with [git](https://git-scm.com).

Writing things down helps me compose my thoughts, but like most people I
suspect, I'm absolutely incapable of getting things right on the first try. I
invariably need to revise, rewrite, and make changes throughout the process.

> Kill your darlings, kill your darlings, even when it breaks your egocentric little scribbler's heart, kill your darlings.”
>
> &mdash; Stephen King

Personally, I'd never be able to "kill kill my darlings without a way to
squirrel away copies of every single draft I ever compose.
[Git](https://git-scm.com) lets me do just that.

It's incredibly _liberating_ to easily track and save any revision you wish,
from just a few words to drastic wholesale revisions and reorganizations of an
entire site. It provides _complete confident that you can recover (or simply
review) all previous content_.

Unlike older revision control tools, [Git](https://git-scm.com) was designed for
offline and disconnected use. You can make changes _and track revisions_ to your
"source" (your exercise library) even while flying over the Pacific ocean,
disconnected from the internet.

[Git](https://git-scm.com) requires **no** connectivity to the internet. You can
use every feature of the tool while completely online. When you are next online,
however, it's trivially easy to "push" your complete set of revisions to another
machine for backup or sharing with others.

## Github for backup

[Git](https://git-scm.com) is designed for "distributed" usage: one or more
remote repositories as well as your local repository.

While it's pretty easy to set up your own server, there are quite a number of
commercial and free git hosting services on the internet. The biggest and most
popular by far is [Github](https://github.com).

[Github](https://github.com) makes it trivial to create a repository and use it
to mirror your local changes. Just type `git push` occasionally to mirror your
_entire_ local repository, and sleep well knowing that even if the hard drive in
your local computer gives up the ghost, you've got a copy of all your revision
history safely stored "in the cloud". Recovery is as simple as typing `git
clone.`

The [github free tier](https://github.com/pricing#feature-comparison) provides
more than enough features for anyone's exercise library.

## Hugo, Docsy and Github Pages for publishing

The final keys to the puzzle are [hugo](https://gohugo.io), [docsy](https://docsy.dev) and
[Github Pages](https://pages.github.com) to publish your exercise content.

[Hugo](https://gohugo.io) is a static website generator. It's what I used to
create this site. It takes a pile of markdown files and turns it into a
beautiful, navigable, website that you can view in any browser.

[Docsy](https://docsy.dev) is a [Hugo theme](https://themes.gohugo.io) expressly
for documentation oriented sites.

Once you've initialized your site, you can start a local server with the `hugo
server` command. If you then point your browser to `localhost:1313` _et voilà_ a
pretty, nicely linked collection of exercises right on your local computer (even
without a working internet connection).

If you're using [git](https://git-scm.com) and
[github](https://github.com/pricing#feature-comparison) as I've suggested, you
can then publish (for free!) your entire collection of exercises using [Github
Pages](https://pages.github.com). Simply type `git push` and anyone with the URL
can read your exercises.

You can choose whether to use the github provided URL (e.g.
`https://username.github.io/exercises/`) or, if you have your own domain, you
can name the site whatever you wish.

Hugo and docsy aren't the only way to manage markdown documentation. I briefly
considered a similar tool called [docsify](https://docsify.js.net) to maintain
my exercise library, but decided to stick with what I know.

## Detailed instructions

I'm in the process of re-organizing my own exercise library ("Rexercises") to
follow my own rapidly evolving system.

Once finished, I plan to create detailed, step-by-step instructions for anyone
to create their own exercise library.