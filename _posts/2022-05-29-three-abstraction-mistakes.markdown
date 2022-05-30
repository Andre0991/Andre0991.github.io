---
layout: post
title:  "Three abstraction mistakes"
date:   2022-05-29 19:34:10 -0300
categories: posts
---

### Incidental similarity

Sonhar é assombroso, e sempre será.
Vê-se imagens: imagens não menos perfeitas que as que são transformadas pela retina.
Sentem-se cheiros: cheiros fiéis ao não-sonho.
Ouvem-se vozes: vozes como as de quem as escuta desperto.
E, no entanto, só um louco (ou um gênio) poderia igualar o universo onírico à realidade dos acordados.

Assim opera o princípio da incidental similarity: realça a falsa igualdade do ponto de partida.

{:refdef: style="text-align: center;"}
![la-reproduction-interdite](/assets/images/la-reproduction-interdite.jpg)
{: refdef}

Some functions look similar in surface, but represent different things.
Consider two functions that have only slightly different behaviours.
Merging such functions would be a mistake, because 
You might think that joining these function would simplify the code.
But then, as time passes, it could need to support more and more behaviours.
The abstraction fails apart quickly and you realise they should have always have stayed independent.
That's because their similarity was merely *incidental*: they seem to be equal today, but they have distinct meanings and should evolve independently.

In extreme cases, functions might even look *identical* (having the same code).
But they are not.
Just like a dream.

### Function overfitting
A function is said to be *overfit* when it is more specific than it needs to be.
The specificity might come from its arguments, its return value, or both.

{:refdef: style="text-align: center;"}
![a-demora-wendell-well](/assets/images/a-demora-wendell-well.jpg)
{: refdef}

Functions that are too specific are harder to grasp.

### Pseudoabstraction

Não há abstração que resista à realidade.
A realidade é una e complexa: tudo muda tudo.
Nenhum recorte é permitido.
A borboleta que levanta voo no quintal pode desencadear um tornado.

Mesmo assim, criamos explicações que excluem a maior parte do real, pois só assim é factível compreender o mundo.

Sendo toda abstração falhas, algumas são mais falhas mais do que as outras.
A pseudoabastraction is a specific case of failure.

{:refdef: style="text-align: center;"}
![magrete-the-double-secret](/assets/images/magrette-the-double-secret.jpg)
{: refdef}

A pseudoabstraction is the result of decoupling a part of a system in a way that understanding the split part is impossible without referring to the original system.

When a function gets too big, it might be tempting to extract some portion of it to a new function.
This might result in a new function that *cannot be understood without consulting the original one*.
That would be a *pseudoabstraction*.
