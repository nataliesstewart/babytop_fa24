# Babytop fall 2024

* [Hardlink to pdf](https://github.com/nataliesstewart/babytop_fa24/blob/main/main.pdf)

These are lecture notes for the [MIT babytop seminar](https://math.mit.edu/topology/babytop/index.html), held Fall of 2024 concerning stable equivariant homotopy theory and the Kervaire invariant one problem. Feel free to submit pull requests for contributions, from minor edits to notes for full talks--please declare that you will do so before a talk is delivered to save Natalie from livetex duties.

## Suggested workflow

The structure of data files is the following: 

```
.
|   README.md			% you are here
|   main.tex			% meta-tex for main output
|   oneref.tex			% only calls one talk tex
└───aux
|   |	environments.sty	% declares theorem-style environments
|   |   macros.sty		% semantic \def's and \newcommand's
|   |   mainmeta.sty		% single import for main.tex
|   |   references.bib		% bibtex file
|   |   style.sty		% formatting, toc, etc.
└───originals
|   └───mm_dd
|       |   foo.tex		% original tex for the talk on american mm/dd, if tex was created elsewhere
└───tex
|   |   mmdd.tex		% inputtable tex for talk on american mm/dd
``` 
If creating or editing tex for a talk on mmdd, please modify it as `./tex/mmdd.tex` following the (no) formatting on previous talks, and to compile it, edit the single content line of `oneref.tex` to read `\talk{Author: Title}{mmdd}` and compile `oneref.tex`. 
Please dump header or bibliography matters into the correct `./aux/*` files and let Natalie know of any bibliographic conflicts (such as differing keys for the same citation).

