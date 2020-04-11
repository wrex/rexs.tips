---
date: 2020-04-08T16:59:35-07:00
title: "Test Driven Guitar"
linkTitle: "Test Driven Guitar"
author: "Rex Walters"
description: >
  Knowing what to practice is half the battle.
type: "docs"
weight: 2

---

Every student, myself included, desires "spoon feeding." We are all fundamentally lazy. We want someone to tell us exactly what we should be working on and in what order, every step of the way.

Sadly, few of us have a nanny-tutor looking over our shoulder at every practice session.

Like most people, I'm also prone to thinking I've mastered something as soon as I can make it all the way through one time. I thought, for example, that once I could play the pentatonic scale in all five positions I was *done*. Next!

Wrong, wrong, wrong.

Knowing is not [KNOWING](#). I needed to learn which note was which in each position. I needed to be able to think "G Major pentatonic" with my hand at any fret on the neck and *instantly* find the closest scale shape. That takes weeks or even months of focused practice. I had just barely *begun* to learn the pentatonic scale!

Knowing these two things, I decided I needed a *system* for practicing.

Concretely, I wanted a system that answered just two questions:

1. **What** should I be working on?
2. Have I practiced this particular item **enough**?

Tracking "what" is a fairly straightforward database problem. I'll discuss my ideas for this shortly.

First, though, let's look at the second question and discsuss what I'm calling "test driven guitar."

## Deciding "enough"

How can I know when I've practiced something sufficiently?

The problem is that most of the practice exercises and drills I've picked up from other instructors are prescriptive, but open ended. "Do this, then do that. Keep going until you think you've got it down.""

But I'm just a novice, who am I to judge whether I've mastered something sufficiently?

I decided to borrow a technique from software developers called "test driven development" or TDD.

### TDD for software

With TDD, you write tests *first*, and only then begin coding the actual software implementation.

With software, the TDD process follows a cycle:

1. **Red Light**. The tests are written, but fail (with a "red" message) because the code is just a "stub" that doesn't actually do anything.

2. **Green Light**. The developer codes the simplest possible implementation that makes the test pass ("green" light). The code is usually pretty ugly and slow at this point.

3. **Refactor**. The developer then makes changes to the code ("refactoring") to make it more readable, maintainable, efficient, and fast. They re-run the tests periodically to ensure the code still works. After each change is tested, the code is broken unless the light turns green.

While the field of software development is obviously quite different from playing guitar, there are some ideas from TDD we can apply to learning the guitar.

I call this *test driven guitar*.

The most important idea is to explicitly define what makes the light turn green **before you start practicing**. In other words, document precisely what it takes to know when you've practiced enough.

### GTD: Pass criteria

Most drills and exercises in books, videos, or online courses only explain how to perform a particular drill. If they mention when you can stop practicing at all, it's usually some sort of totally subjective guidance.

I wanted to create *tests* with *objective* pass criteria, rather than completely open-ended *exercises*.

I'm publishing a series of "proficiency tests" using TDD principles to expressly define what constitutes a "green light" for a particular test.

How to make the pass criteria objective rather than subjective? Enter **Mr. Metronome.**

Most people think a metronome only has two purposes:

* It provides a steady pulse during practice to improve your internal sense of timing.
* It lets you build speed by practicing at higher and higher BPM.

Both are true, but a metronome also excels as an objective, and *cruel*, task master.

Imagine teaching a child to recite the alphabet. At some point, the kid can probably make it all the way from A to Z successfully, but with lots of "umms" and "errs" dispersed throughout. The kid smiles in relief and thinks she's done.

With an evil grin, her teacher then say, "Congrats, Kid. You've memorized your ABCs, now comes the hard part."

Teacher then sets a metronome to, say, 80 BPM and says, "Every time this clicks I want you to say the next letter of the alphabet, but you can't miss a click!"

Suddenly reciting the alphabet got a whole lot harder.

*That* is how you use the metronome to objectively measure proficiency.

I won't pretend that every exercise "green light" can be defined with a metronome setting, but it does suffice for a huge majority of exercises. Regardless, I've tried hard to define *some* sort of objective *proficiency tests* with every exercise.

Further, wherever possible, I've tried to define both "Initial Green" and "Refactored Green." That is, when do you know the material enough to start practicing seriously, and when have you truly mastered the material? When have you "learned your ABCs" and when can you recite the alphabet *without pause*?

## Tracking "what"

Deciding "enough" was only half the battle, though. I still needed a way to keep track of what I was working on.

Conceptually, I wanted a list of "things to practice" that tracked my progress and prevented me from getting lost.

I definitely *didn't* want anything that dictated a rigid, linear progression through the items, one by one.

Most instructional sites are written that way: complete this, then do that, and only then start this new thing.

Some days I just didn't feel like working on technique and wanted to better understand theory. Other days I *only* wanted to focus on technique. Still other days, I just wanted to practice actually making music (playing a song, switching between chords, or picking out a melody).

My energy level and inclinations *change* day by day. This is *normal* (or at least so I've convinced myself).

One thing I knew for sure is that learning is **not** linear!

How to track our progress yet remain disciplined?

### The master list

What if I just maintained a simple list of every practice item? Conceptually, I just needed a list of practice items, each in one of three possible states:

* Never attempted
* In progress
* Mastered

With a little more thought, I created a list like this:

| Item     | Mastered? | Last attempted | Description
| ---      | ---       | ---            | ---
| [001](#) | Y         | 3/1/2020       | [find notes along low E](#)
| [002](#) | Y         | 3/2/2020       | [find notes along A](#)
| [003](#) | Y         | 3/3/2020       | [find notes along D](#)
| [004](#) | Y         | 3/4/2020       | [find notes along G](#)
| [005](#) | Y         | 3/5/2020       | [find notes along B](#)
| [006](#) | Y         | 3/1/2020       | [find notes along high e](#)
| [007](#) |           | 3/6/2020       | [find all notes everywhere on neck](#)
| [008](#) |           |                | [play B Maj triads on GBe and DGB](#)
| [009](#) |           |                | [find E Maj triads on GBe and DGB](#)
| &vellip; | &vellip;  | &vellip;       | &vellip;

Items without an attempt date are obviously in state: "never attempted."

Item's with an attempt date but not yet mastered are "in progress."

Items with "Y" in the mastered column I've already mastered.

The item number and description were *links* to a thorough explanation of the drill, with diagrams, videos, etc.

After a bit more thought, I realized I still had a few problems:

1. The list will quickly grow quite long. Knowing my proclivities, even the filtered list of "in progress" items will grow without bound. With umpteen dozen "in progress" exercises, will I really know what I should be working on?

2. I needed some way of creating *hierarchy* and relationships. Some practice items need several sub-items. Several drills/exercises are attempting to teach the same skill.

3. I don't intend to be the only user, so clearly I need a database of some sort to track all this stuff for each user.

I learned a while ago that I start to stress whenever I'm working on more than roughly three to five things at a time.
