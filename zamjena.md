# Zamjena

r           zamjena jednog znaka
R           zamjena dok prekida unosa

c           zamjena za korištenje uz pokret

cw          zamjena jedne riječi
c$          zamjena do kraja linije

Napomena:
```
U tekstu niže, g se smatra dijelom naredbe, odnosno g~, gU i gu su naredbe!
```

~           zamjena znaka *uppercase* <-> *lowercase*
g~w         zamjena riječi *uppercase* <-> *lowercase*
g~~         zamjena cijele linije *uppercase* <-> *lowercase*

gUw         zamjena cijele riječi u *uppercase*
gUU         zamjena cijele linije u *uppercase*

guw         zamjena cijele riječi u *lowercase*
guu         zamjena cijele linije u *lowercase*

"acw        zamjena riječi i prebacivanje obrisanog u registar

Općenito vrijedi:
```
<broj-ponavljanja><nareba><pokret>
```

2gUU        zamjena dvije linije u *uppercase*
2g~w        zamjena dvije riječi *uppercase* <-> *lowercase*

*sed-like* zamjene (za riječ "old" u "new":
: s/old/new          zamjena na trenutnoj liniji, i to za prvu instancu riječi "old" u liniji
:1,5 s/old/new/      zamjena samo za linije 1-5, i to za prvu instancu riječi "old" u liniji
:.,$ s/old/new/      zamjena od trenutne linije do zadnje linije, i to za prvu instancu riječi "old" u liniji
:% s/old/new/g       zamjena kroz cijeli tekst, u svim instancama (koristi se *global* flag "g"

Općenito vrijedi:
```
:<range> s/<pattern>/<string>/<flags>
Može se koristiti i drugi znak umjesto "/"
```
