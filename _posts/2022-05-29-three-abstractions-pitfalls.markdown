---
layout: post
title:  "Three abstraction's pitfalls"
date:   2022-05-29 19:34:10 -0300
categories: posts
---

### Incidental similarity

<!-- Sonhar é assombroso, e sempre será. -->
<!-- Vê-se imagens: imagens não menos perfeitas que as que são transformadas pela retina. -->
<!-- Sentem-se cheiros: cheiros fiéis ao não-sonho. -->
<!-- Ouvem-se vozes: vozes como as de quem as escuta desperto. -->
<!-- E, no entanto, só um louco (ou um gênio) poderia igualar o universo onírico à realidade dos acordados. -->

<!-- Assim opera o princípio da incidental similarity: realça a falsa igualdade do ponto de partida. -->

Dreaming is astonishing, and always will be.
One sees images: images no less perfect than those transformed by the retina.
Smells are smelled: smells faithful to the non-dream.
Voices are heard: voices like those of someone who is awake.
And yet, only a madman (or a genius) could equate the dreamlike universe with the waking reality.

This is how the principle of incidental similarity works: it highlights the false equality of the starting point.

{:refdef: style="text-align: center;"}
![la-reproduction-interdite](/assets/images/la-reproduction-interdite.jpg)
{: refdef}

Some functions look similar in surface, but represent different things.
Consider two functions that have only slightly different behaviors.
You might think that joining these function would simplify the code.
But then, as time passes, it would need to support more and more behaviors.
The abstraction fails apart quickly, and you realize they should always have stayed independent.
That's because their similarity was merely *incidental*: they seem to be equal today, but they have distinct meanings and should evolve independently.

In extreme cases, functions might even look *identical* (having the same code).
But they are not.
Just like dreams.

### Function overfitting

There's something uncanny about hyperrealism.
The intensity of the details.
Their extreme precision.
The lack of gaps.

Such are overfit functions: victims of its own perfection.

{:refdef: style="text-align: center;"}
![a-demora-wendell-well](/assets/images/a-demora-wendell-well.jpg)
{: refdef}

A function is said to be *overfit* when it is more specific than it needs to be.
The specificity might come from its arguments, its return value, or both.

Creating an over-specific function is easy: write code that returns exactly the data you need.
It will work.
But it might be difficult to grasp.
Get a step back.
Instead, write a function that performs a slightly more general operation.
Then, use its return value for extracting the specifics.

General is simple.
Specific is complex.

### Pseudoabstraction

<!-- Não há abstração que resista à realidade. -->
<!-- A realidade é una e complexa: tudo muda tudo. -->
<!-- Nenhum recorte é permitido. -->
<!-- A borboleta que levanta voo no quintal pode desencadear um tornado. -->

<!-- Mesmo assim, criamos explicações que excluem a maior parte do real, pois só assim é factível compreender o mundo. -->

<!-- Sendo toda abstração falha, algumas são mais falhas mais do que as outras. -->
<!-- A pseudoabastraction is a specific case of failure. -->

There is no abstraction that resists reality.
Reality is one and complex: everything changes everything.
No clipping is allowed.
The butterfly that takes flight in the backyard can trigger a tornado.

Even so, we create explanations that exclude most of the real, because only then is it possible to understand the world.

Although every abstraction is flawed, some are more flawed than others.
A pseudoabstraction is a specific case of failure.

{:refdef: style="text-align: center;"}
![magrete-the-double-secret](/assets/images/magrette-the-double-secret.jpg)
{: refdef}

A pseudoabstraction is the result of decoupling a part of a system in a way that understanding the split part is impossible without referring to the original system.

When a function gets too big, it might be tempting to extract some portion of it to a new function.
This might result in a new function that *cannot be understood without consulting the original one*.
That would be a *pseudoabstraction*.

Do not try too hard to abstract things.
Reality always imposes itself.
