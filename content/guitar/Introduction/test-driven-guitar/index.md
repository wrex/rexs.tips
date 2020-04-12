---
date: 2020-04-08T16:59:35-07:00
title: "Test Driven Guitar"
linkTitle: "Test Driven Guitar"
author: "Rex Walters"
description: >
  A system for knowing what to practice.
type: "docs"
weight: 30

---

{{% pageinfo %}}
This material is purely background on my system of [proficiency tests](/guitar/tests). It explains why and how I came up with TDG, and some of my future plans.

If you just want to get started with learning the instrument, please feel free to skip this chapter.
{{% /pageinfo %}}

Every student, myself included, desires "spoon feeding." We are all fundamentally lazy. We want someone to tell us exactly what we should be working on and in what order, every step of the way.

Sadly, few of us have a nanny-tutor looking over our shoulder at every practice session. We all have to figure out how to make our practice efficient on our own.

Like most people, I'm also prone to thinking I've mastered something and am ready to move on as soon as I can perform it *once* at a slow, shaky tempo.

I thought, for example, that once I'd memorized all five shapes of the pentatonic scale I was *done*. Next!

Wrong, wrong, wrong.


## On knowing
{{% alert color="info" %}}
It took me several years to realize the *degree* to which I needed to learn things on the guitar.

Guitarists must learn fundamentals to an almost maniacal degree. They must know things as well as they know letters of the alphabet, the names and colors of fruits, or the names and faces of friends and family members.

I call this **KNOWING** something (all caps and bold). Knowing is not **KNOWING**.

Just as when you hear “green” you immediately visualize the color, hearing the note name "C&sharp;" should cause several locations on the fretboard to *light up* in your mind's eye.

**KNOWING** means you know something back-to-front as well as front-to-back.

It means: given a note name, you can instantly, *effortlessly* find that note all over the fretboard.

It means: after plunking a finger down anywhere on the fretboard, you instantly, *effortlessly* know the name of the note at that location and the name of the other notes nearby.
{{% /alert %}}

Just memorizing the five shapes barely scratched the surface. I needed to learn which note performed what function in each position. I needed to internalize each note *sounded* over different chords in a blues progression. I needed to be able to think "G Major pentatonic" with my hand at any fret on the neck and *instantly* find the closest scale shape. Without conscious thought, I needed to be able to instantly switch to the scale for the next chord in a progression *as nearby on the neck as possible*.

That takes weeks or even months of focused practice. I had just barely *begun* to learn the pentatonic scale!

Knowing these two things, I decided I needed a *system* for practicing.

Concretely, I wanted a system that answered just two questions:

1. Have I practiced this particular exercise **enough**?
2. **What** should I work on next?

## Have I practiced enough?

Most drills and exercises in books, videos, or online courses only explain how to perform a particular drill. If they mention when you can stop practicing at all, it's usually some sort of totally subjective guidance.

The problem is that they are prescriptive: "Do this, then do that." But they are *open-ended*: "Keep going until you think you've got it down."

I'm just a novice, how can I to judge whether I've mastered something sufficiently?

I wanted to create *tests* rather than completely open-ended *exercises*. I wanted *objective* pass criteria, not fuzzy, subjective self-evaluation.

I decided to borrow a technique from software developers called "test driven development" or TDD.

### Software TDD

Software developers that use the TDD system write tests *first*, and only then begin coding the actual implementation.

The TDD process follows a cycle.

1. First they write a test and just a "stub" implementation (that compiles but doesn't actually do anything).

2. **Red Light**. Initially, the tests fail (with a "red" message). They know the code doesn't work yet, so they expect the test to fail.

2. **Green Light**. The developer codes the simplest possible implementation that makes the test pass ("green" light). The code is usually pretty ugly and slow at this point.

3. **Refactor**. The developer then makes changes to the code ("refactoring") to make it more readable, maintainable, efficient, and fast. They re-run the tests as they make changes to ensure the code still works. They can be confident their changes haven't broken the code if the light remains green.

While the field of software development is obviously quite different from playing guitar, there are some ideas from TDD we can apply to practicing guitar.

The most important idea is to explicitly define what makes the light turn green **before you start practicing**. In other words, document precisely what it takes to know when you've practiced enough.

### TDG: Proficiency tests

Early in each tutorial page on this site, I refer to a *proficiency test* that let's you know when you've mastered the material.

A *proficiency test* expressly defines objective criteria for what constitutes a "green light" with a particular exercise or drill.

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

I won't pretend that every guitar exercise "green light" can be defined with a metronome setting, but it does suffice for a huge majority of exercises. Regardless, I've tried hard to define *some* sort of objective "green light" criteria for every proficiency test.

## What should I work on next?

Defining "enough" for each exercise was only half the battle, though. I still needed a way to track progress, and tell me what to work on next.

Conceptually, I wanted a list of "things to practice" that tracked my progress and prevented me from getting lost. Basically a shopping list of guitar exercises.

I definitely *didn't* want anything that dictated a rigid, linear progression through the items, one by one. Most instructional sites are written that way: complete this, then do that, and only then start this new thing. I almost invariably stray from the prescribed path eventually.

Some days I just don't feel like working on technique and would rather learn some theory. Other days I *only* wanted to focus on technique. Many days, I just wanted to practice actually making music (playing a song, switching between chords, or picking out a melody) without any repetitive technique drills or brain-busting theory.

My energy level and inclinations *change* day by day. This is *normal* (or at least so I've convinced myself).

Still, I want to know if I've been skipping technique drills or theory lessons for too long. I want to make it visible if I keep starting and never finishing items.

How to track my progress?

### The list

What if I just maintained a simple list of every proficiency test? Conceptually, I just needed a list of proficiency tests, each in one of three possible states:

* Never attempted
* In progress
* Mastered

With a little thought, I created a list like this:

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

After a bit more thought, I realized just one long list had several problems:

1. The list will quickly grow quite long. Knowing my proclivities, even the filtered list of "in progress" items will grow without bound. With umpteen dozen "in progress" exercises, will I really know what I should be working on?

2. I needed some way of creating *hierarchy* and relationships. Some practice items need several sub-items. Several drills/exercises are attempting to teach the same skill.

3. I don't intend to be the only user, so clearly I need a database of some sort to track all this stuff for each user.

4. While I eventually hope to provide automatic tracking of items for each logged in user, I needed a pencil and paper mechanism during the interim.

I learned a while ago that I start to stress whenever I'm working on more than roughly three to five things at a time.

---

Next: [Fundamentals]({{< ref "/guitar/Fundamentals" >}})
