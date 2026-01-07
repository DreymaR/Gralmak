<h1 align=center line-height=1.6>Gralmak</h1><br><br>

<div align=center ><img src="_res/img/Gralmak_Orth-Cpt_EPKL.png" 
                        alt="The Gralmak layout (EPKL help image)"></div><br>

## Gralmak Appendix
This page is for stuff that I consider too chonky for the main layout page.
<br><br>

## Meet The Family
- "Grallium" is a fun name for the [Gallium][GalGit]-[Graphite][GraGit]-Gralmak-++ layout family.
- A more serious one is "NRTS HAEI".
<br>

- The [Sturdy][StrPKL] layout came about as a result of the [Oxeylyzer][AnaHom] which includes some metrics that its predecessors didn't.
- Sturdy looks different from the family at first, especially with its different home position ...
- ... but it does have at least `LR MT SV` and `FH OA UE` columns in common with most of the others.
```
Sturdy (Oxey, 2022-07)
  v m l c p  x f o u j  
  s t r d y  . n a e i -
  z k q g w  b h ' ; ,  
```
<br>

- Several other layouts like [Nerps][NrpRed]/Nerts/Nerbs and Maya are clearly family members.
- These mostly have the `NRTS HAEI` home position and the column similarities listed above, but differ in minor aspects.
```
Nerps (Smudge, 2022-03)
  x l d p g  z k o u ;              (Nerts (Smudge, 2022-03) is another variant)
  n r t s w  y h e i a              (`x p g v` -> `p g v x` from Nerps – swap `xvgp`)
  q j m c v  b f ' , .  

Nerbs (Smudge)
  b l d v j  z f o u ;  
  n r t s g  y h a e i ,
  q x m c w  k p ' / .  

Maya (adi.lela)
  b l d g q  j f o u ,              (Designed with an Angle mod not shown here, for row-stag)
  n r t s v  k h a e i  
  z x m c w  p y ' / .  
```
<br>

- When it comes to Gralmak and its parents [Graphite][GraPKL] and [Gallium][GalPKL], they are practically the same layout.
- The [cmini][Acmini] analyzer doesn't care about upper vs lower row, so it ignores the differences in `wz cv` positions.
- The main differences are in punctuation placements. I consider that mostly a separate issue here.
```
Gallium (GalileoBlues)
  b l d c v  j f o u ,              (This is the v2/row-stag version)
  n r t s g  y h a e i              (`y p f` and `x q` positions are swapped in v1)
  q x m w z  k p ' ; .  

Graphite (StronglyTyped)
  b l d w z  ' f o u j ;            (Only the unshifted layer is shown here)
  n r t s g  y h a e i ,            (`' , - /` have nonstandard shift mappings)
  q x m c v  k p . - /  

Gralmak (DreymaR)
  b l d w q  j f o u '  
  n r t s g  y h a e i ;            (Add AngleWideSym mods as desired)
  z x m c v  k p , . /  
```
<br><br>

## Gralmak Analysis
- Below is a comparison of the Graphite layout and the Gralmak variant, disregarding most punctuation.
- It's made by the [cmini][Acmini] analyzer at the AKL Discord, with thumb-key for common punctuation.
- As shown, the differences consist of swapping `J` and `QU`, and swapping `Z` and `Q`.
- All overall stat differences are so small that I don't think they can be considered significant.

- The J-QU swap makes 2-key rolls more outwards by 0.4%; this is okay with me.
- One-hand 3-key rolls are not significantly affected.
- The [Q-Z swap][Gal-QZ] retains a little more QWERTY/Colemak familiarity, at a very low stat cost.
- There seems to be a small increase in alternating same-finger skipgrams, which I think is okay.
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
- I have devised but not implemented such loops, mostly as a mental exercise.
- If someone really wants a set of transitional layouts from QWERTY to Gralmak, I could help with implementation.

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

<h1 align=center>⌨&nbsp;&nbsp;&nbsp;⌨&nbsp;&nbsp;&nbsp;⌨&nbsp;&nbsp;&nbsp;⌨&nbsp;&nbsp;&nbsp;⌨</h1>

<br><br>

## TODO/WIP
- Tough choice: Should plain Gralmak _not_ use the SC-QU swap?!? For max compatibility with QWERTY/Colemak.
	- In this case, GralmakS with its Sym mod will be preferable for non-Wide applications.
	- I think not. For one, QU is inside the letter block in Graphite. And I like that position a lot.
	- Make it clear, then, that the SC-QU swap is a possibility for users who don't prefer this way.
- Add Gralmak to MonkeyType and Keybr?
- Introduce both Gralmaks and Sym. Explain how they work together
	- There's only one Gralmaks, incorporating Sym. Otherwise, madness.
- Discuss in-/outrolls vs alternation etc.
	https://www.reddit.com/r/KeyboardLayouts/comments/1pzhwhh/comment/nwrnp3k/
- Make a forum for discussing the Grallium layout family, in lieu of a Discord server? On GitHub?
	- Alt-fingering of SC SW GS   PH HY KY ...
	- Troublesome bi-/skipgrams: DM/MD, LR/RL ('world', 'clearly')
	- Troublesome LSBs: NG
	- Fun bigrams over rows: LS LT DS OH AU UH. Involve mostly the middle fingers.
	- 

<br>

<h1 align=center>⌨&nbsp;&nbsp;&nbsp;⌨&nbsp;&nbsp;&nbsp;⌨&nbsp;&nbsp;&nbsp;⌨&nbsp;&nbsp;&nbsp;⌨</h1>

[Acmini]: https://github.com/Apsu/cmini                                                 (Apsu's cmini layout analyzer)
[AnaHom]: https://github.com/O-X-E-Y/oxeylyzer                                          (The Oxeylyzer layout analyzer home page)
[Kanata]: https://github.com/jtroo/kanata                                               (The Kanata multiplatform layout program)
[PKLGit]: https://github.com/DreymaR/BigBagKbdTrixPKL/                                  (The EPKL keyboard layout program for Windows)
[Galite]: https://github.com/almk-dev/galite/                                           (The Galite variant, nearly equal to Gralmak - now removed)
[NrpGra]: https://www.reddit.com/r/KeyboardLayouts/comments/tpwyjc/comment/jck98z6/     (Graphite comment in the Nerps post on Reddit)
[GraSci]: https://github.com/rdavison/graphite-layout/blob/main/README.md#on-scissors   (The Graphite README on Scissors)
[Gal-QZ]: https://github.com/GalileoBlues/Gallium/issues/6#issuecomment-2665066910      (Discussing a Q-Z swap w/ almk on the Gallium repo)
[GraPct]: https://github.com/rdavison/graphite-layout/issues/2#issuecomment-2787752575  (Discussing Graphite punctuation and Wide mods on its repo)

[GraGit]: https://github.com/rdavison/graphite-layout#graphite-keyboard-layout          (The Graphite layout on GitHub)
[GalGit]: https://github.com/GalileoBlues/Gallium#gallium                               (The Gallium layout on GitHub)
[GrlGit]: https://github.com/DreymaR/Gralmak#gralmak                                    (The Gralmak layout on GitHub)
[NrpRed]: https://www.reddit.com/r/KeyboardLayouts/comments/tpwyjc/                     (The Nerps layout on Reddit)
[CmkPKL]: https://github.com/DreymaR/BigBagKbdTrixPKL/tree/master/Layouts/Colemak#colemak               (The Colemak layout in EPKL)
[StrPKL]: https://github.com/DreymaR/BigBagKbdTrixPKL/tree/master/Layouts/Sturdy#sturdy                 (The Sturdy layout in EPKL)
[GalPKL]: https://github.com/DreymaR/BigBagKbdTrixPKL/tree/master/Layouts/Gallium#gallium               (The Gallium layout in EPKL)
[GalrEP]: https://github.com/DreymaR/BigBagKbdTrixPKL/tree/master/Layouts/Gallium#galliard              (The Galliard Gallium layout variant)
[GraPKL]: https://github.com/DreymaR/BigBagKbdTrixPKL/tree/master/Layouts/Graphite#graphite             (The Graphite layout in EPKL)
[GralEP]: https://github.com/DreymaR/BigBagKbdTrixPKL/tree/master/Layouts/Gralmak#gralmak               (The Gralmak layout variant in EPKL)
[ErgAWi]: https://dreymar.colemak.org/ergo-mods.html#angle-wide                         (DreymaR's BigBag on Angle+Wide ergo mods)
[ErgCrl]: https://dreymar.colemak.org/ergo-mods.html#curl-dh                            (DreymaR's BigBag on the Curl-DH ergo mod)
[ErgSym]: https://dreymar.colemak.org/ergo-mods.html#symbols                            (DreymaR's BigBag on the Symbols ergo mod)
[BBTseq]: https://dreymar.colemak.org/layers-main.html#sequences                        (DreymaR's BigBag on sequencing)
[BBTtmk]: https://dreymar.colemak.org/tarmak-intro.html                                 (DreymaR's Big Bag on Tarmak transitions)
[CoDeKy]: https://github.com/DreymaR/BigBagKbdTrixPKL/blob/master/README.md#advanced-composecodekey (The EPKL README on the CoDeKey)
