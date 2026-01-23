<h1 align=center line-height=1.6>Gralmak</h1><br><br>

<div align=center ><img src="_res/img/Gralmak_Orth-Cpt_EPKL.png" 
                        alt="The Gralmak layout (EPKL help image)"></div><br>

## The Gralmak keyboard layout
Gralmak is a Graphite-Gallium variant that keeps closer to familiar layouts without sacrificing significant quality.
<br><br>

## About Gralmak
- This layout was made by DreymaR (that's me!), 2024-11.
- It is a variant of [Graphite][GraGit] by StronglyTyped and [Gallium][GalGit] by GalileoBlues. These layouts are very similar.
- Gallium/Graphite are in turn related to other recent layouts, like [Sturdy][Sturdy] by Oxey and [Nerps][NrpRed] by Smudge.
<br>

![Gralmak Angle-ANSI help image](_res/img/Gralmak_ANS-A_EPKL.png)

_The Gralmak layout (using the Angle mod for XMCVZ) on an ANSI keyboard_

<br>

- I wanted to make a Graphite-Gallium variant with traditional symbol/punctuation placements.
- Thus came about the Gralmak variant that's easily ergo modified like, e.g., Colemak-CAWS.
- Like most other layouts, I didn't want to change the Shift states of keys.
- Like the [Gallium][GalPKL] and [Colemak(-Sym)][CmkPKL] layouts, I want J in the middle and a symbol on pinky.
- I decided to have the apostrophe/quote in the letter block by default, as I like that a lot.
- I also brought Z back to its familiar spot where QWERTY and Colemak has it.
<br>

- It's easier to learn for someone coming from QWERTY, Colemak, and other layouts that leave the symbol keys unchanged.
- In this capacity, it can also be a stepping-stone to full Graphite or Gallium! Learn Gralmak first, then decide whether to proceed.
- This incurs some worse punctuation bigrams. Since I use my thumb [CoDeKey][CoDeKy] for most punctuation, I don't care.
- If you don't use punctuation solutions, you may instead use a symbol mod of your choice; see below.
<br>

The name is a play on Graphite-Gallium-Colemak, and our quest for the mythical "Holy Grail" of layouts.
<br><br>

<div align=center ><img src="_res/img/Grail-Chalice.png" style="width:30%;height:auto"></div><br>

- Gralmak manages to satisfy newer analyzers and still keep some similarity to well-known layouts like Colemak.
- For instance, only `L N M` and `F A E` swap hands from QWERTY; `L N M` and `F A P` from Colemak.
- The familiar `QW RT ZX CV` bigrams are (semi-)preserved, aiding learning and recognition.
<br>

```
+----------------------------+
| 1 2 3 4 5   6 7 8 9 0  - = |
| b l d w q   j f o u '  [ ] |    Gralmak
| n r t s g   y h a e i  ; \ |    on an ortho keyboard
| z x m c v   k p , . /      |
+----------------------------+
```
<br>

Some more info plus an implementation for my [EPKL][PKLGit] program may be found in its [Gralmak layout folder][GmkPKL].
<br><br>

## Meet The Family
"Grallium" is a fun name for the Gallium-Graphite-Gralmak-++ layout family. A more serious one is "NRTS HAEI". 
These layouts have a lot in common.

In the [Appendix](./README_APP.md#meet-the-family) you may read a little more about the different family members.
<br><br>

|  Gallium-v1  |  Graphite  |
|:------------:|:----------:|
|  ![](_res/img/Gallium-v1_Orth-Cpt_EPKL.png)  |  ![](_res/img/Graphite_Orth-Cpt_EPKL.png)  |

<br><br>

## Ergo Mods
- An [**Angle**][ErgAWi] ergo mod is recommended for this layout on row-staggered boards.
- Gralmak may be said to use the [**Curl**][ErgCrl] principle, by reducing lateral stretches to the middle home row positions.
- By default, the only symbol keys it affects are quote (QU) and semicolon (SC).
- Not moving the symbol keys makes it easier to learn and transition to, and adds flexibility.
- Depending on your use case you may want to apply further Sym and/or Wide ergo mods to Gralmak.
<br>

### GralmakS
GralmakS is a [Symbol mod][ErgSym] for Gralmak. 
In my implementations, it's really a bundle of GralmakS itself which addresses the `.` `/` `,` keys only, 
and a non-Wide Sym mod (for WideSym Gralmak, see [below](#gralmak-widesym)) that addresses the hyphen-minus key. 
<br><br>

![GralmakS help image](_res/img/Gralmak_Orth-Cpt-S_EPKL.png)

_GralmakS on an Ortho keyboard. Note its `.` `/` `,` key positions._

<br>

- The apostrophe-quote key is already moved in standard Gralmak: Like Graphite, I kept it in the letter block.
    - Since the semicolon key is already displaced from QWERTY, this arrangement seems natural to me.
    - As mentioned, you may reverse this `QU-SC` swap if you wish.
- Standard Gralmak keeps most punctuation unmoved from QWERTY, like Colemak and some other layouts do.
    - This makes Gralmak easier to learn and transition to. You can always address symbol keys later.
    - Another reason is that I can use a special thumb [CoDeKey][CoDeKy] for most punctuation.
- However, using Gralmak without a punctuation solution isn't quite ideal for text typing.
- The main issues according to Cyanophage's analyzer are the `E.` SFB (0.14%) and the `O,` SFB+skipgram (0.09%).
<br>

- GralmakS, at heart, is a mod variant that swaps `,` `/` `.` while keeping other punctuation unchanged.
- It has Graphite's period on the OA column. Both Gallium and Graphite place comma with I on the pinky.
- You'll have to decide whether that's useful for you.

```
+----------------------------+
| 1 2 3 4 5   6 7 8 9 0  - = |
| b l d w q   j f o u '  [ ] |    Gralmak
| n r t s g   y h a e i  ; \ |    (unmodified)
| z x m c v   k p , . /      |
+----------------------------+

+----------------------------+
| 1 2 3 4 5   6 7 8 9 0  [ ] |
| b l d w q   j f o u '  - = |    GralmakS 
| n r t s g   y h a e i  ; \ |    (non-Wide Sym mod)
| z x m c v   k p . / ,      |
+----------------------------+
```
<br>

- You could instead use Gallium or Graphite punctuation, if you prefer.
- Gallium punctuation has somewhat lower SFB% according to [cmini][Acmini] analysis. Its period placement is most of the reason.
- However, Gallium achieves this by placing both comma and period on off-home-row pinky keys which increases pinky usage.

```
+----------------------------+
|                        [ ] |
|             '   o u    ; = |    Graphite
|               h a e i  , \ |    symbols
|                 . - /      |
+----------------------------+

+----------------------------+
|                        - = |
|                 o u ,  [ ] |    Gallium
|               h a e i  /   |    symbols
|                 ' ; .      |
+----------------------------+
```
<br>

- My [**S**ym(bol)][ErgSym] ergo mods move the hyphen to a better position. GralmakS deserves that.
- The brackets go up to the number row (`[ ]` / `- =`), as on Graphite. 
	- Another option would be `= [` / `- ]`.
- Unfortunately, Gralmaks doesn't play well with a Wide ergo mod since it displaces the comma.
<br>

### Gralmak-WideSym
- [**W**ide][ErgAWi] ergo mods (moving right-hand keys one position to the right) usually place the two bracket keys in the middle.
- Wide/Sym modded Gralmak variants are fairly straightforward from base Gralmak, as it doesn't change any tricky symbol keys.
- I couldn't fit the [GralmakS](#gralmaks) mod that addresses the `,` `.` keys in with a Wide mod though.
<br>

- [**S**ym(bol)][ErgSym] mods usually prioritize the common <kbd>'"</kbd> (Apostrophe/Quote) and <kbd>-_</kbd> (Hyphen/Underscore) keys.
- For Wide variants, a Sym mod is beneficial. I've implemented Gralmak WideSym variants.
- The quote-semicolon (QU-SC) swap is already a part of standard Gralmak. Feel free to reverse it if you wish, though.
- I prefer the hyphen (MN) next to QU on the upper row. Seems this is a matter of individual preference.
<br>

![Gralmak-WS help image](_res/img/Gralmak_Orth-WS_EPKL.png)

_Gralmak-WideSym on an Ortho keyboard_

<br>

#### Gralmak AWS
```
+----------------------------+
| 1 2 3 4 5 6 \ 7 8 9 0 =    |
|  b l d w q [ j f o u ' - ; |    ANSI
|  n r t s g ] y h a e i     |    keyboard
|   x m c v z / k p , .      |
+----------------------------+

+----------------------------+
| 1 2 3 4 5 6 \ 7 8 9 0 =    |
|  b l d w q [ j f o u ' -   |    ISO
|  n r t s g ] y h a e i ;   |    keyboard
| z x m c v   / k p , .      |
+----------------------------+
```

<br><br>

## Experiences
After 18+ years of using Colemak plus some ergo mods, I devised Gralmak and reached a decent (at least 80-ish WPM) speed on it. 
I've told about some experiences with that on my BigBag <a href="https://dreymar.colemak.org/layers-base#delving-too-greedily"><b>Base Layout</b></a> page (open the "Still, what about ..." spoiler box).

The short version of it is: Gralmak feels good! But then, so does Colemak. 
The quality difference isn't at all as huge as some make it out to be. 
And some of it may be mostly up to preferences and experience.

Some Grallium (Gralmak/Graphite/Gallium/++) related points distilled from the BigBag layout page:
> - Grallium have several delightful n-grams.
> - More than on Colemak, all three rows are in use without much scissoring.
> - The bottom row of Gralmak goes `ZXMCV`. 
>   - Keeping `ZXCV` close to their familiar places is an asset to some.
<br>

> - As a physicist, I notice that `PHY` is worse on Gralmak.
> - Another bad one is `RL/LR` in words like 'world'; it's rare but on a ring finger.
> - `UE/EU`, correspondingly, is a bad SFB pair on both layouts. 
>   - It's in fact a little worse on Grallium as it uses the ring finger.
> - Lateral stretches for `YOU` and `NG/GN` feel less than ideal but it's no biggie. 
>   - Overall though, Grallium layouts have less LSBs than Colemak.
<br>

One distinguishing feature of Grallium is a higher alternation (switching hands) compared to Colemak. 
Most typists feel that a good inward roll beats alternation, but bad same-hand trigrams (redirects/"pinballs") are a lot worse. 
So while Colemak has some good rolls going for it, Grallium layouts avoid some of its sticky patterns with higher alternation. 

When typing, I tend not to notice alternations – while good same-hand patterns feel great and problematic ones feel bad.

My overall impression of typing with Grallium is very positive. 
I've heard that the ideal must be to type a bi- or trigram before alternating: 
It does feel like these layouts hit a good balance on that account. 
Especially since most of those one-hand n-grams have a nice flow to them. 

Compared to Colemak, I feel that Grallium layouts use the upper row more actively. 
There are some nice bigrams that either fall on the upper row or half-scissor between upper and home row in a pleasant way. 

The pinky and ring fingers are also used more to some extent, which may be a point to watch out for! 
Some users have untrained or anatomically challenged pinkies and/or ring fingers: 
For these I'd recommend learning Colemak(-DH) instead of a Grallium layout.

For more observations and thoughts, see the [Appendix](./README_APP.md#experiences).
<br><br>

## Gralmak Analysis
I've done some simple layout analysis using the [cmini][Acmini] analyzer to confirm that apart from punctuation 
(which I consider a separate matter) the Gralmak layout performs about as well as Gallium and Graphite. 
There are minute differences, but they may well be within the uncertainty of analysis and are minor anyway.

Keep in mind though, that analysis is far from everything!

In [an interesting Reddit comment](https://www.reddit.com/r/KeyboardLayouts/comments/1pzhwhh/comment/nwrnp3k/), these words of wisdom caught my attention:
> ... don't blindly trust the stats. Columns are more important, and often choosing worse columns gives you better stats ...

For details on the analysis, see the [Appendix](./README_APP.md#gralmak-analysis).
<br><br>

## GralQwest Transitions
- Some [Colemak][CmkPKL] learners have used my [Tarmak][BBTtmk] transitional layouts to learn the layout in smaller steps.
- Learning Gralmak from QWERTY is a longer way since Colemak(-DH) moves only 17(18) keys and Gralmak 24.
- It's still possible to construct learning loops for users who want to learn 3–6 keys at a time.
- For details on the proposed GralQwest transitional layouts, see the [Appendix](./README_APP.md#gralqwest-transitions).

<br>

<h1 align=center>⌨&nbsp;&nbsp;&nbsp;⌨&nbsp;&nbsp;&nbsp;⌨&nbsp;&nbsp;&nbsp;⌨&nbsp;&nbsp;&nbsp;⌨</h1>

<br><br>

![Gralmak ISO help image](_res/img/Gralmak_ISO-AWS_EPKL.png)

_Gralmak-AWS-ISO. The © key can be a Compose key, or whatever you wish._


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
[Sturdy]: https://oxey.dev/sturdy/                                                      (The Sturdy layout's home page)
[NrpRed]: https://www.reddit.com/r/KeyboardLayouts/comments/tpwyjc/                     (The Nerps layout on Reddit)
[CmkPKL]: https://github.com/DreymaR/BigBagKbdTrixPKL/tree/master/Layouts/Colemak#colemak               (The Colemak layout in EPKL)
[StrPKL]: https://github.com/DreymaR/BigBagKbdTrixPKL/tree/master/Layouts/Sturdy#sturdy                 (The Sturdy layout in EPKL)
[GalPKL]: https://github.com/DreymaR/BigBagKbdTrixPKL/tree/master/Layouts/Gallium#gallium               (The Gallium layout in EPKL)
[Gallrd]: https://github.com/DreymaR/BigBagKbdTrixPKL/tree/master/Layouts/Gallium#galliard              (The Galliard Gallium layout variant)
[GraPKL]: https://github.com/DreymaR/BigBagKbdTrixPKL/tree/master/Layouts/Graphite#graphite             (The Graphite layout in EPKL)
[GmkPKL]: https://github.com/DreymaR/BigBagKbdTrixPKL/tree/master/Layouts/Gralmak#gralmak               (The Gralmak layout variant in EPKL)
[ErgAWi]: https://dreymar.colemak.org/ergo-mods.html#angle-wide                         (DreymaR's BigBag on Angle+Wide ergo mods)
[ErgCrl]: https://dreymar.colemak.org/ergo-mods.html#curl-dh                            (DreymaR's BigBag on the Curl-DH ergo mod)
[ErgSym]: https://dreymar.colemak.org/ergo-mods.html#symbols                            (DreymaR's BigBag on the Symbols ergo mod)
[BBTseq]: https://dreymar.colemak.org/layers-main.html#sequencing                       (DreymaR's BigBag on sequencing)
[BBTtmk]: https://dreymar.colemak.org/tarmak-intro.html                                 (DreymaR's Big Bag on Tarmak transitions)
[CoDeKy]: https://github.com/DreymaR/BigBagKbdTrixPKL/blob/master/README.md#advanced-composecodekey (The EPKL README on the CoDeKey)
