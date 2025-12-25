<h1 align=center line-height=1.6>Gralmak</h1><br><br>

<div align=center ><img src="_res/img/Gralmak_Orth-Cpt_EPKL.png" 
                        alt="The Gralmak layout (EPKL help image)"></div><br>

## The Gralmak keyboard layout
Gralmak is a Graphite-Gallium variant that keeps closer to familiar layouts without sacrificing significant quality.
<br><br>

## Work-In-Progress
- For now, there isn't much in this repo. Please consult the [Gralmak layout folder][GralEP] in my [EPKL][PKLGit] program for info.
- There are a few downloads ready in the Files folder though. More to come, fairly soon I hope.


<br><br>

![Gralmak ISO help image](_res/img/Gralmak_ISO-AWS_EPKL.png)

_Gralmak-AWS-ISO. The © key can be a Compose key, or whatever you wish._

<br><br>

## Gralmak Analysis
- Below is a comparison of the Graphite layout and the Gralmak variant, disregarding most punctuation.
- It's made by the 'cmini' analyzer at the AKL Discord, with thumb-key for common punctuation.
- As shown, the differences consist of swapping `J` and `QU`, and swapping `Z` and `Q`.
- All overall stat differences are so small that I don't think they can be considered significant.

- The J-QU swap makes 2-key rolls more outwards by 0.4%; this is okay with me.
- One-hand 3-key rolls are not significantly affected.
- The [Q-Z swap][Gal-QZ] retains a little more QWERTY/Colemak familiarity, at a very low stat cost.
- There is a small increase in alternating same-finger skipgrams, which I think is okay.
- Non-SFS alternation, accordingly, goes down by an insignificant amount (from 33.85% to 33.80%).

```
gralmak-thumb(new) - graphite-thumb(old)
  b l d w ~  ~ f o u ~
  n r t s g  y h a e i
  ~ x m c v  k p     /
               ! , . ; -

SHAI:
  Alter: -0.05%
  Rolls: -0.02%   (In/Out: -0.42% |  0.39%)
  One-h:  0.03%   (In/Out: -0.04% |  0.07%)
  Redir: -0.02%   (Bad:    -0.03%)

  SFB:    0.00%
  SFS:    0.06%   (Red/Alt: 0.01% | 0.05%)
```

<br><br>

## GralQwest Transitions
- Some [Colemak][CmkPKL] learners have used my [Tarmak][BBTtmk] transitional layouts to learn the layout in smaller steps.
- Some even said they couldn't have done it all at once. Others strongly prefer going all the way at once, cold turkey.
- Learning Gralmak from QWERTY is a longer way since Colemak(-DH) moves only 17(18) keys and Gralmak 24.
- It's still possible to construct learning loops for users who want to learn 3–6 keys at a time.

Here's a way of splitting up a QWERTY-to-Gralmak transition into five steps, roughly sorted by key frequencies:
```
Big loop of 18 keys:
    S → F → U → O → I → ; → 
    P → M → C → V → B → Q → 
    T → D → E → L → W → R

Miniloops of 3 keys:
    A → K → N
    Y → H → J

Not moved – 3 keys:
    G   Z   X
```

- It makes sense to misplace less common keys during the big loop steps: `;` in step 1, `Q` in step 2.
- The rationale for postponing the common `E` and `T` is to avoid misplacing the common `R`.
- It's up to the user whether miniloops should go before or after the big loop. The `Y` miniloop gives less benefit.
- Since the big loop steps are 6 keys each, the number of steps can be reduced by skipping the first miniloop step.
- The semicolon can be swapped with the apostrophe in the 2nd part of the big loop, when it finds its place.
<br>

- For now, I'm doing this mostly as a mental exercise. 
- If someone really wants to use such a set of transitional layouts, I could help implement them.

Thus, five "GralQwest" QWERTY-to-Gralmak transitional layouts might look as follows:
```
GralQwest 0, alias QWERTY:
q w e r t    y u i o p
a s d f g    h j k l ; '
z x c v b    n m , . /

GralQwest 1 (big loop 1/3):
q w e r t    y F O U p
a ; d S g    h j k l I '                S → F → U → O → I → (;)
z x c v b    n m

GralQwest 2 (big loop 2/3):
B w e r t    y f o u '
a q d s g    h j k l i ;                P → M → C → V → B → (Q)
z x M C V    n P

GralQwest 3 (big loop 3/3):
b L D W Q    y f o u '
a R T s g    h j k E i ;                T → D → E → L → W → R
z x m c v    n p

GralQwest 4 (A miniloop):
b l d w q    y f o u '
N r t s g    h j A e i ;                A → K → N
z x m c v    K p

GralQwest 5 (Y miniloop), alias Gralmak:
b l d w q    J f o u '
n r t s g    Y H a e i ;                Y → H → J
z x m c v    k p , . /
```

This progression prioritizes getting the big loop over with, to avoid "limbo" keys in neither-QWERTY-nor-Gralmak positions.

Alternatively, here are five "GralQwest" QWERTY-to-Gralmak transitional layouts with miniloops first:
```
GralQwest 0, alias QWERTY:
q w e r t    y u i o p
a s d f g    h j k l ;
z x c v b    n m , . /

GralQwest 1 (A miniloop):
q w e r t    y u i o p
N s d f g    h j A l ;                  A → K → N
z x c v b    K m

GralQwest 2 (Y miniloop):
q w e r t    J u i o p
n s d f g    Y H a l ;                  Y → H → J
z x c v b    k m

GralQwest 3 (big loop 1/3):
q w e r t    j F O U p
n ; d S g    y h a l I                  S → F → U → O → I → (;)
z x c v b    k m

GralQwest 4 (big loop 2/3):
B w e r t    j f o u '
n q d s g    y h a l i ;                P → M → C → V → B → (Q)
z x M C V    k P

GralQwest 5 (big loop 3/3), alias Gralmak:
b L D W Q    j f o u '
n R T s g    y h a E i ;                T → D → E → L → W → R
z x m c v    k p , . /
```

This progression might be useful if you wish to practice some smaller loops first. After step 3, you may want to jump to the finish.

<br>

<h1 align=center>⌨&nbsp;&nbsp;&nbsp;⌨&nbsp;&nbsp;&nbsp;⌨&nbsp;&nbsp;&nbsp;⌨&nbsp;&nbsp;&nbsp;⌨&nbsp;&nbsp;&nbsp;⌨&nbsp;&nbsp;&nbsp;⌨</h1>


[GraGit]: https://github.com/rdavison/graphite-layout#graphite-keyboard-layout          (The Graphite layout on GitHub)
[GalGit]: https://github.com/GalileoBlues/Gallium#gallium                               (The Gallium layout on GitHub)
[GrlGit]: https://github.com/DreymaR/Gralmak#gralmak                                    (The Gralmak layout on GitHub)
[NrpRed]: https://www.reddit.com/r/KeyboardLayouts/comments/tpwyjc/                     (The Nerps layout on Reddit)
[NrpGra]: https://www.reddit.com/r/KeyboardLayouts/comments/tpwyjc/comment/jck98z6/     (Graphite comment in the Nerps post on Reddit)
[GraSci]: https://github.com/rdavison/graphite-layout/blob/main/README.md#on-scissors   (The Graphite README on Scissors)
[PKLGit]: https://github.com/DreymaR/BigBagKbdTrixPKL/                                  (The EPKL keyboard layout program for Windows)
[CmkPKL]: https://github.com/DreymaR/BigBagKbdTrixPKL/tree/master/Layouts/Colemak/                      (The Colemak layout in EPKL)
[StrPKL]: https://github.com/DreymaR/BigBagKbdTrixPKL/tree/master/Layouts/Sturdy/                       (The Sturdy layout in EPKL)
[GalPKL]: https://github.com/DreymaR/BigBagKbdTrixPKL/tree/master/Layouts/Gallium/                      (The Gallium layout in EPKL)
[GalrEP]: https://github.com/DreymaR/BigBagKbdTrixPKL/tree/master/Layouts/Gallium/README.md#galliard    (The Galliard Gallium layout variant)
[GraPKL]: https://github.com/DreymaR/BigBagKbdTrixPKL/tree/master/Layouts/Graphite/                     (The Graphite layout in EPKL)
[GralEP]: https://github.com/DreymaR/BigBagKbdTrixPKL/tree/master/Layouts/Gralmak                       (The Gralmak layout variant in EPKL)
[Galite]: https://github.com/almk-dev/galite/                                           (The Galite variant, nearly equal to Gralmak - now removed)
[ErgAWi]: https://dreymar.colemak.org/ergo-mods.html#angle-wide                         (DreymaR's BigBag on Angle+Wide ergo mods)
[ErgCrl]: https://dreymar.colemak.org/ergo-mods.html#curl-dh                            (DreymaR's BigBag on the Curl-DH ergo mod)
[ErgSym]: https://dreymar.colemak.org/ergo-mods.html#symbols                            (DreymaR's BigBag on the Symbols ergo mod)
[BBTseq]: https://dreymar.colemak.org/layers-main.html#sequences                        (DreymaR's BigBag on sequencing)
[BBTtmk]: https://dreymar.colemak.org/tarmak-intro.html                                 (DreymaR's Big Bag on Tarmak transitions)
[CoDeKy]: https://github.com/DreymaR/BigBagKbdTrixPKL/blob/master/README.md#advanced-composecodekey (The EPKL README on the CoDeKey)
[Gal-QZ]: https://github.com/GalileoBlues/Gallium/issues/6#issuecomment-2665066910      (Discussing a Q-Z swap w/ almk on the Gallium repo)
[GraPct]: https://github.com/rdavison/graphite-layout/issues/2#issuecomment-2787752575  (Discussing Graphite punctuation and Wide mods on its repo)

[Kanata]: https://github.com/jtroo/kanata                                               (The Kanata multiplatform layout program)
