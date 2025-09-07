---
layout: post
title:  "...combinational circuits are applicative functors?"
date:   2025-09-06 17:38:36 -0700
categories: electronics clash haskell 
---

### Understanding Clash's functional description of circuits

#### Intro
Coming from a background in electronics hardware, I find myself unusually fascinated by Haskell as a programming language. My limited work with programming usually involves writing C in a strictly embedded context (ignoring my somewhat completed [Typogenetics project]), so I don't spend a lot of time working in high levels of abstraction that are provided by languages like Haskell. I am sure in the future I'll spend some time collecting my thoughts on the language and functional programming in general.

I think it's a natural first instinct to imagine functional programs as a pretty far divide from embedded work or as an applicable language for electronics, so coming across Gerg&#337; &#201;rdi's episode of the [Haskell Interlude] and hearing about [Retrocomputing with Clash], my mind was blown. 
Mathematical models or functional descriptions of circuit behavior was something I was somewhat aware of, but this book provides a strong motivation for me to research further into the subject. This book does assume an "intermediate level of skill" with Haskell, unfortunately not a category I fall under. But I'm using the fusion of my interests that this book covers as my excuse to gain a better understanding of the language.  

This post (or likely series of posts) will cover some of the more jargony sections of the book, and serve to explain just what is meant by an "applicative functor" to someone not so used to the terms in Haskell. 

#### The Clash Language
OK, we're not talking about Haskell, it's [Clash]. From the description, clash "borrows both its syntax and semantics from the functional programming language Haskell." I won't pretend to be an expert in either, and most the concepts I cover should be applicable to either language.

#### Describing circuits in Clash 






[Haskell Interlude]: https://haskell.foundation/podcast/12/
[Retrocomputing with Clash]: https://unsafeperform.io/retroclash/
[Typogenetics project]: https://github.com/finntonwentworth/typogenetics.git
[Clash]: https://clash-lang.org/