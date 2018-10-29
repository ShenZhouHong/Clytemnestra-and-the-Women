# Clytemnestra and the Women
[**St. John's College**](https://sjc.edu/)
2018 Freshmen Seminar Paper on *Agamemnon*, by Aeschylus.
Written by Shen Zhou Hong [`<shong@sjc.edu>`](mailto:shong@sjc.edu)

## Summary
The Aeschylus's Homeric play *Agamemnon* is set in a world where the status of
women is consistently placed beneath that of men. Despite this, the character of
Clytemnestra consistently confronts, and challenges the inequitable gender-norms
set forth in Agamemnon. Her *"man-like"* behavior is noted by the townsmen of
Argos, and eventually culminates to a high point, in her slaying of her husband
Agamemnon. The killing of Agamemnon becomes the definite moment where
Clytemnestra ceases to conform within the norms of womanhood, and acts in the
stead of a male hero, seeking justice through revenge.

## Parts of the thesis
### What are the gender norms for women in Aeschylus's *Agamemnon*?
Begin by examining the gender norms set forth in *Agamemnon*, especially the
norms of women in contrast to men:

- Start with an enumeration of every instance where the norms of womanhood are
  displayed or enforced:
  - **Line # `258`:** The Herald which greets Clytemnestra subtly hints at the
    secondary status of a woman to a man's.
  - **Line # `275`:** The Argive townsmen persistently doubt Clytemnestra's
    news about the sacking of Troy.
  - **Line # `480`:** Argive townsmen discuss amongst themselves the news of
    Troy's sacking, and many are dismissive of Clytemnestra, solely over the
    fact that she is a woman.
  - **Line # `810`:** *"... and in a woman's cause it hath been laid low"* ---
    Agamemnon compares the sacking of Troy to the rape of a woman.
- *Possible additions:* Briefly look at the role of women in other Homeric
  stories like the Iliad and the Odyssey.
- Briefly enumerate the norms of manhood which are displayed or enforced:
  - **Line # `355`:** When Clytemnestra eloquently explains her system of
    messengers and fire beacons, the Herald compares her speech to that of an
    *"prudent man"*.

### How does Clytemnestra challenge and surpass these gender norms?
Through textual evidence, show how Clytemnestra challenges the norms set forth
in *Agamemnon*

- **Line # `275`:** In response to the doubts of the Argive townsmen, rather
  than yielding assent, Clytemnestra vocally refutes their misgivings.
- **Line # `350`:** The Argive townsmen comments on her speech about her signal
  beacons, saying that she has "spoke like a man".
- **Line # `600`:** After the arrival of the Herald, the Argive townsmen sends
  the Herald to relate the news of the sacking of Troy. Clytemnestra refuses to
  let him repeat it, and chides the Argive townsmen for not believing her.
  - In response to this reproach, the Herald says that the speech is
    `un-wifelike` (**Line # `613`**).
- **Line # `941`:** In Clytemnestra's scene where she urges Agamemnon to step on
  the tapestries, her forceful persuasion causes Agamemnon to comment "Surely
  tis' not a woman's part to be fond of contest".

### How does Clytemnestra's killing of Agamemnon relate to the role of her gender?

- First, note how within Homeric literature, the pursuit of justice through the
  mete of blood (i.e. seeking justice by the sword) is a task that is relegated
  almost entirely to men:
  - **Textual evidence #1:** It is the men who seek Helen, in Homer's Iliad.
  - **Textual evidence #2:** Likewise, it is Odysseus and Telemachus who avenge
    Penelope of her suitors.
  - **Textual evidence #3:** The only counterexample that we can perceive is
    that of Antigone, but even in her case her seeking of justice is a passive
    one, rather than active.
- Secondly, note how the idea of a woman slaying a man is completely
  unimaginable to the Argive townsmen, even when Cassandra tells them of the
  slaying in advance. Specifically, quote the exchange at **Line # `1250`**,
  where the Argive townsmen assume it is a man.
- Compare and contrast the meek and 'woman-like' deliberations of the Argive
  townsmen after hearing the cries of their king, with Clytemnestra's bold
  speech. She also says that they think of her as a witless woman, but she is
  not.

## Some notes on Clytemnestra's speech

- Note how Clytemnestra displays her husband to the Argive townsmen, and very
  purposely say that it is her intent and forthright will to kill her husband
  -- but immediately, the townsmen dismiss her speech by asking if she is mad.
- Next, Clytemnestra speaks about how she killed Agamemnon to avenge the death
  of Iphigenia. Her argument is very passionate, for she acknowledges the sheer
  inequity of roles they play -- how Agamemnon is praised, but she the murderer.
- Additionally note how the reply of the Chorus is deeply laments. It is clear
  that one of the reasons they are so shocked by his murder, is that it has
  been committed at the hands of a woman.
- Pay particular attention to the speech by Clytemnestra at **Line # `1530`**,
  where she literally takes on the role of Thyestes, the guest of Atreus who
  was wronged evilly.

## Quickstart
In order to customize this LaTeX template file to your project, simply rename
the `essay-name.tex` file, and than edit the the included makefile to point at
the right file again:

### makefile
```
# Makefile for latexmk
source_name = essay-name
```
### Compiling document
In order to compile latex source files, run `make` in the terminal:
```
cd latex
make
make clean
```

Note: for any partial compiles where compilation fails at a certain point, you
should run `make clean` followed by make again. Trying to run make after a
failed compile would result in additional errors.

### Dependencies
This template uses a makefile to compile the latex source files. The makefile
uses `latexmk`, which runs latex the correct number of times. This is because
due to the presense of figures, tables, and biblatex databases, latex needs to
be called multiple times in some cases. Latexmk should be included in your
latex installation, but if it is now, you may download it here:

* http://personal.psu.edu/jcc8//software/latexmk-jcc/

Additionally, this template uses XeLaTeX by default, as it allows the inclusion
of unicode characters in the latex source files. If XeLaTeX is not installed, or
plain LaTeX is required, simply alter the `makefile` at the appropriate call:

```
# MAIN LATEXMK RULE
$(source_name).pdf: $(source_name).tex
  ...
	latexmk -pdf -xelatex -use-make $<
```

XeLaTeX allows one to use foreign characters like ü or æ natively in the latex
source files, though. So it's probably a good idea to install XeLaTeX:

* http://xetex.sourceforge.net/

### Related documentation
For an overview of how to populate biblatex `citations.bib` files, visit the
biblatex-mla manual at CTAN.

* https://www.ctan.org/pkg/biblatex-mla

### GPLv3 License
The raw template itself is licensed under the terms of the GPL (version 3). A
full copy of the license is attached in `LICENSE.md`. Naturally, any works
that you create using this template (i.e. any actual essays you write using
it) will be your own intellectual property. The GPLv3 license only applies to
any derivative templates.
