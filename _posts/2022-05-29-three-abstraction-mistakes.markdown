---
layout: post
title:  "Three abstraction mistakes"
date:   2022-05-29 19:34:10 -0300
categories: posts
---

### Function overfitting
A function is said to be *overfit* when it is more specific than it needs to be.
The specificity might come from its arguments, its return value, or both.


{:refdef: style="text-align: center;"}
![a-demora-wendell-well](/assets/images/a-demora-wendell-well.jpg)
{: refdef}

Functions that are too specific are harder to grasp.

### Incidental similarity

Some functions look similar in surface, but represent different things.
In extreme cases, they might even be *identical* (having the same code), but having different meanings, that is, semantics.

{:refdef: style="text-align: center;"}
![la-reproduction-interdite](/assets/images/la-reproduction-interdite.jpg)
{: refdef}

Merging such functions would be a mistake, because their similarity is merely *incidental*: they seem to be equal today, but they have distinct meanings and should evolve independently.

### Pseudoabstraction
A pseudoabstraction is the result of declouping a part of a system in a way that understanding the split part is impossible without referring to the original system.

{:refdef: style="text-align: center;"}
![magrete-the-double-secret](/assets/images/magrette-the-double-secret.jpg)
{: refdef}

For example, when a function gets too big, it might be tempting to extract some portion of it to a new function.
This might result in a new function that cannot be undertood unless one knows the original one.
That would be a *pseudoabstraction*.
