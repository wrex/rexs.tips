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

Sadly, few of us are ever likely to have a nanny-tutor with us for every practice session.

Worse, I've discovered that like most people, I'm prone to thinking I've mastered something **long** before I become truly proficient. I thought, for example, that once I could play the pentatonic scale in all five positions I was *done*. Next!

Wrong, wrong, wrong. Knowing is not [KNOWING](#). I needed to learn which note was which in each position. I needed to be able to think "G Major pentatonic" with my hand at any fret on the neck and *instantly* find the closest scale shape. I had just barely *begun* to learn the pentatonic scale.

I decided to create a *system* for practicing that instantly tells me:

1. **What** should I be working on?
2. Have I practiced this particular item **enough**?

Let's tackle those two questions in reverse order.

## Deciding "enough"

How can I know when I've practiced something sufficiently?

The problem is that most of the practice exercises and drills I've picked up from other instructors are prescriptive, but open ended. "Do this, then do that. Keep going until you think you've got it down.""

But I'm just a novice, who am I to judge whether I've mastered something sufficiently?

I decided to borrow a technique from software developers called "test driven development" or TDD.

### Test Driven Development

With TDD, you write tests *first*, and only then begin coding the actual software implementation.

With software, the process follows a cycle:

1. **Red Light**. The tests are written, but fail (with a "red" message) because the code is just a "stub" that doesn't actually do anything.

2. **Green Light**. The developer codes the simplest possible implementation that makes the test pass ("green" light). The code is usually pretty ugly and slow at this point.

3. **Refactor**. The developer then makes changes to the code ("refactoring") to make it more readable, maintainable, efficient, and fast, rerunning the test periodically to ensure the code still works. After each change is tested, the code is broken unless the light is green.

While the field of software development is obviously quite different from playing guitar, I stole ideas from TDD and applied them to learning the guitar.

I call this *test driven guitar*.

The most important idea is to **explicitly define what makes the light turn green**. In other words, document precisely what it takes to know you've practiced enough.

### Pass criteria

Most drills and exercises in books, videos, or online courses only explain how to perform the drill, with only a bit of subjective guidance (if anything) regarding when you can stop practicing.

I wanted the exercises on this site to be *tests* with objective pass criteria, so I've expressly defined what constitutes "green light" in every practice exercise ("proficiency test") on this site.

But how to make the pass criteria objective? Enter Mr. Metronome

Most people think a metronome only has two purposes:

* Provide a steady pulse during practice to improve your internal rhythm
* Let you build speed by practicing at higher and higher BPM

But a metronome also excels as an objective, and *cruel*, task master:

  "Can you complete the exercise three times in a row with half notes at 120 BPM without error".

The metronome is not just for developing your sense of time, it's also an incredibly disciplined task master.

Imagine teaching a child to recite the alphabet.

My father used to tell a great story about teasing his younger brother: "You're so dumb I bet you can't even recite the alphabet." My uncle replied, "Sure I can! ... Of course, once you get up to 'R' and all that stuff ....".

I bet my uncle could repeat the alphabet at 40 BPM quarter notes, but he'd probably have struggled at a faster tempo.

Unfortunately, the pass criteria isn't always measurable. Sometimes it's unavoidably subjective and requires self assessment: "You can play the lick/song/whatever fluently and expressively without undue stress and without losing your place."

The idea, though, is to specify the pass criteria *before* you start practicing.

Many proficiency tests will have a corresponding tutorial or other page describing the background material.

All tests will have "Green light criteria": what does it take to pass the test?

Some tests may have extra credit (effectively "refactoring suggestions") to continue your exploration even after you've mastered the item.


## Tracking "what"

In order to know what I should be working on, I obviously needed some way to track

I needed a way to keep track of what I was working on. Conceptually, I wanted a list of "things to practice" that kept track of my progress and kept me from getting lost.

I definitely *didn't* want anything that dictated a rigid, linear progression through the items, though. Most instructional sites are written that way: complete this, then do that, and only then start this new thing.

Somedays I just didn't feel like working on technique and wanted to better undertand theory. Other days I *only* wanted to focus on technique. Still other days, I just wanted to practice actually making music (playing a song, switching between chords, or picking out a melody).

My energy level and inclinations *change* day by day. This is normal (or at least so I've convinced myself).

One thing I know for sure is that learning is **not** linear!

It's completely reasonable and normal (actually unavoidable in my opinion) to branch out and explore whatever strikes your fancy on any given day.

But how can we track our progress and remain disciplined?

### Epiphany #1:  list of all items

What if I just maintained a simple list of every practice item? Conceptually, I just needed to mark each item in one of three possible states:

* Never attempted
* In progress
* Mastered

With a little more thought, I came up with a simple list like this:

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

The item number and description could even *links* to an explanation of the drill, with diagrams, videos, etc.

After a bit more thought, I realized I still had several problems:

1. The list will quickly grow quite long.

2. I needed some way of creating *hierarchy* and relationships. Some practice items need several sub-items.

3. Even if I'm the only user it seems like I need a database of some sort to track all this stuff. I know I'll have at least two users, so I need to track the mastered and last attempted columns per user.

4. Knowing my proclivities, even the list of "in progress" items will grow very long. I'll still struggle figuring out what I should be practicing today.


### Defining "mastered"


### TDG in practice

I'm calling each item in TDG a "proficiency test". Each item explicitly states what constitutes basic proficency for the item (a "green" light).



The goal is to present each user with a list of practice items sorted and filtered based on the current days interests.

Eventually, I'd like to show the progress state of each item for the logged in user, but I'll need to do some coding to make that work. For now, you'll just have to use pen and paper to track which items you're currently working on or have mastered.
