---
author: "Benjamin Prevor"
authorTwitter: "@BenjaminPrevor"
desc: "A review of Learn You a Haskell for Great Good"
image: "./images/learn_you_a_haskell.jpg"
keywords: "book review, haskell"
lang: "en"
title: "Learn You a Haskell: A Retrospective on My First Six Years of Programming"
tagline: "How purity culture may have led me to a lack of purpose"
updated: "2024-05-09T12:00:00Z"
year: "2024"
---

### "Learn You a Haskell for Great Good! A Beginner's Guide" by Miran Lipovača

<div style="text-align:center">
    <img
      alt="Learn You a Haskell for Great Good by Miran Lipovaca"
      src="./images/learn_you_a_haskell.jpg"
      height="400"
    />
</div>

When I was 14, I went to a [Long Island Linux User Group](https://lilug.org/) meeting with my father and brother. I guess I knew what Linux was, but my familiarity with programming as a practice was mostly just informed by things on Reddit and TV.

I watched my brother give a lightning talk on the [Lemote YeeLong](https://www.linux-netbook.com/lemote-yeeloong-8089/), the first laptop that, from the BIOS to the hardware drivers, contained solely [free as in freedom software](https://www.gnu.org/philosophy/free-sw.en.html). My brother's unconventional choices, like opting for the [NoPhone](https://thenophone.com/) instead of a cell phone, reinforced the notion of "purity" in computing and abstraction from practicalities. I listened to many other talks that day, and by the end of the user group meeting, I got my first sense of why my brother felt so much joy from his deviation from normal consumer choices. There are respects in which Linux provides greater utility than alternative options, but this enhanced utility was not why these people were gathered; they were gathered because they felt that the way they computed was more ethical, more pure, more how God intended.

Inspired by this experience, in the summer of 2017, before I would enter my first [quarter](<https://en.wikipedia.org/wiki/Academic_quarter_(year_division)>) of studies at UChicago, I decided I would finally learn a little programming to better connect with my brother, who was at the time studying computer science as well. The introductory course [CS161: Introduction to Programming I](http://cmsc-16100.cs.uchicago.edu/2021-autumn/), taught by [Ravi Chugh](https://people.cs.uchicago.edu/~rchugh/), had a unique philosophy on how one should be introduced to higher-level study in computer science.

> This is an introductory honors course in computer science, not just computer programming. We will learn through the vehicle of a specific programming language—Haskell—a pure, lazy, functional programming language. This quarter has a distinct "high-brow" feel to it, because Haskell obtains power through generality, and generality through abstraction.

I knew that compared to the average UChicagoan in this class, I would have significantly less experience with programming. So I looked at the recommended texts and saw: <h1>Learn You a Haskell for Great Good by Miran Lipovaca</h1>

I found the book mildly charming. Miran has a fun writing style; his musings and funny [interludes](https://haskell.foundation/podcast/) kept the book readable, and thus I learned the basics of Haskell.

I didn't know this at the time, but what in hindsight makes LYaHfGG! such a remarkable book, is two main factors:

> 1. The book is written for beginners with no experience in programming at all.
> 2. The book is focused on topics you need to know to enter the "Haskell Community," not necessarily the topics you'd need to know to program useful things.

As an aside, years later while working as a full-time Haskell developer at [BlockApps](https://blockapps.net/), I would encounter a funny anecdote written by a former coworker about LYaHfGG!. He wrote, "Unless you wish to unlearn the previous way you did things, I do not recommend learning via the great good."

When I got to school in the upcoming fall, I felt like I had a comparative advantage in the class. To my fellow classmates, learning Haskell was an affectation, like entering a different dimension of programming which they had previously learned, but to me, it was just learning what was in the book and on the slides.

I was quite insecure and struggling with [imposter syndrome](https://en.wikipedia.org/wiki/Impostor_syndrome) in my first year at UChicago. Many of my classmates were simply far more knowledgeable than me in many of the domains that I was particularly interested in and at the time I didn't understand that I just needed to change my study habits. I struggled mightily in many classes during my first year, which made my relative advantage in what was supposed to be one of the hardest first-year classes at UChicago stand out even more. I interpreted this as an indication that functional programming was an area where I had a particular talent.

I think this early success heavily hindered my ability to learn and adapt in future classes. It felt as if I was striving for an ideal that was, in itself, an end. I was not just learning to code; I was aligning myself with a philosophy that simply did not have the relevance to the real world that so many students already knew.

When we learned the basic structure of Haskell, which involved learning the building blocks of Haskell (Functors, Applicatives, and Monads), I felt a sense of achievement:

```haskell
class Functor f where
    fmap :: (a -> b) -> f a -> f b
class (Functor f) => Applicative f where
    pure  :: a -> f a
    (<*>) :: f (a -> b) -> f a -> f b
class Monad m where
  (>>=)  :: m a -> (  a -> m b) -> m b
  (>>)   :: m a ->  m b         -> m b
  return ::   a                 -> m a
```

However, this sense of mastery was challenged when I took a course on web development. As I struggled to apply my Haskell knowledge to the practical tasks of building web applications, I began to realize that my early specialization in Haskell's abstract concepts might have constrained my growth as a programmer.

Looking back, I see how in later classes and projects, I sometimes tried to shoehorn obtuse ways to accomplish tasks. I would abandon practical considerations and refuse to learn methods that didn't pass the purity test. In my graduate studies, I would suffer through trying to get Python exercises to work on my NixOS system running an AMD GPU, even when the whole class had no trouble setting up their environments on a Mac or Ubuntu machine.

I had internalized that programming languages are tools, and different ones suit different purposes, but I wanted to shoehorn my existing knowledge into every domain. While principles like functional purity have their place, pragmatism and flexibility are essential.

I'm grateful for the strong foundation and lasting interest in the field of computer science that "Learn You a Haskell" gave me, but I've also accepted that it limited my horizons. The key for the future is to keep learning, try to keep an open mind, and strive for that elusive balance between learning that makes me comfortable and learning that makes me uncomfortable. That, perhaps, is the true path to "great good" in this field.

This is a work in progress
