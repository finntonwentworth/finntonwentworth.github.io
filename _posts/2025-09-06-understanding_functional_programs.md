---
layout: post
title:  "...combinational circuits are applicative functors? "
date:   2025-09-06 18:00:36 -0700
tags: electronics clash haskell 
---

### Learning Functional Programming from a non CS perspective

#### Intro
Coming from a background in electronics hardware, I find myself unusually fascinated by Haskell as a programming language. My limited work with programming usually involves writing C in a strictly embedded context (ignoring my somewhat completed [Typogenetics project]), so I don't spend a lot of time working in high levels of abstraction that are provided by languages like Haskell.

I think it's a natural first instinct to imagine functional programs as a pretty far divide from embedded work or as an applicable language for electronics, so coming across Gerg&#337; &#201;rdi's episode of the [Haskell Interlude] and hearing about [Retrocomputing with Clash], my mind was blown. 

I quickly reached the end of my understanding of Haskell upon flipping to Chapter 3, "Combinational Circuits are Applicative Functors". I realized I had to sit down and really try to understand just what Haskell looks to accomplish with the introduction of these very mathematical terms into programming.  
Mathematical models or functional descriptions of circuit behavior was something I was somewhat aware of, but this book provides a strong motivation for me to research further into the subject. This book does assume an "intermediate level of skill" with Haskell, unfortunately not a category I fall under. But I'm using the fusion of my interests that this book covers as my excuse to gain a better understanding of the language.  

This post (or likely series of posts) will cover some of the more jargony concepts of the book and functional languages in general, and serve to explain to myself the depth of the Haskell and Clash Languages.
Hopefully, it can help understand why you (me) might write functional code to design circuits rather than going to straight to HDL. 

#### Understanding Functional Languages
When we write in a language in C or especially Assembly, we are giving a very explicit set of instructions to the computer in order to complete some task.


I think that this is absolutely captured when applying a function to elements of a list in the two languages: 

{% highlight c %}
for (int i = 1; i <= 10; i++) {

}

{% endhighlight %}

{% highlight haskell %}
ghci> 3 * 3 
9

ghci> map (*3) [1..10]
[3,6,9,12,15,18,21,24,27,30]
{% endhighlight %}

{% highlight haskell %}
class Functor a where 
-- Definition of Functor 
{% endhighlight %}

### References 

[Haskell Interlude]: https://haskell.foundation/podcast/12/
[Retrocomputing with Clash]: https://unsafeperform.io/retroclash/
[Typogenetics project]: https://github.com/finntonwentworth/typogenetics.git