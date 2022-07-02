# Plugins

:set packpath                           direktoriji u koje se pohranjuju *plug-in*-ovi

Package je kolekcija *plug-in*-ova.

Unutar nekog *packpath* direktorija, potrebno je kreirati direktorij "pack" unutar kojeg se pohranjuju *plug-in*-ovi.
<packpath>/pack/<package-directory>

<package-directory> može biti proizvoljan!

~/.vim/pack/start/pack-dir1                                                 učitavaju se uvijek, pri startu
~/.vim/pack/opt/pack-dir2                                                   učitavajuučitavaju se po potrebi
Za pokretanje *plug-in*-a, bitno je konačno ime direktorija u koji je pohranjen!

:packadd <plugin-directory-name>    :pa <plugin-directory-name>             učitavanje *plug-in*-a iz *opt* direktorija

Package je de-facto git repozitorij koji se klonira negdje u ~/.vim/pack/ direktorije.
* ako se klonira u neki start/ direktorij, radit će odmah po startu *vim*-a
* ako se klonira u neki opt/ direktorij, pokretat će se po potrebi s naredbom :packadd <direktorij>

*Plug-in*-ovi (bilo u start/ ili opt/ direktorijima se u pravilu pokreću sa "svojim" naredbama, npr.:
:NERDTree
:Tab
...

*Plug-in*-ovi se brišu tako da se obriše njihov direktorij / git repozitorij.
