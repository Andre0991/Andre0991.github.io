---
layout: post
title:  "Three abstraction mistakes"
date:   2022-05-29 19:34:10 -0300
categories: posts
---

### Function overfitting
A function is said to be overfit when it is more specific than it needs to be.
The specificity might come from its arguments, its return value, or both.

{:refdef: style="text-align: center;"}
![overfitting](/assets/images/overfitting.png)
{: refdef}

Functions that are too specific are harder to grasp.

### Incidental similarity

{:refdef: style="text-align: center;"}
![maggrete-the-double-secret](/assets/images/maggrete-the-double-secret.png)
{: refdef}


### Pseudoabstraction
A pseudoabstraction is the result of declouping a part of a system in a way that understanding the split part is impossible without referring to the original system.



For example, when a function gets too big, it might be tempting to extract some portion of it to a new function.
This might result in a new function that cannot be undertood unless one knows the original one.
That function would be a pseudoabstraction.
