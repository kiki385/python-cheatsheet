# .vimrc

:set                popis uključenih ne-*defaultnih* opcija
:set [no]<opcija>   [isključuje]/uključuje opciju
:set <opcija>?      provjera uklučenosti opcije
:set <opcija>!      prekidač za uključivanje/isključivanje opcije
:set <opcija>?      postavlja opciju na defaultne postavke

:e <putanja>        otvara/kreira datoteku za uređivanje

:h option-list      lista opcija   
:options            lista opcija
:color <shema>      postavljanje sheme boja     
:source <datoteka>  *source*-a datoteku, tj. izvršava sve naredbe u njoj

```
U .vimrc datoteci sve se opcije postavljaju bez dvotočke :
```

""                                  komentiranje linije
set history=1000                    postavljanje veličine *history*-ja na 1000
set ruler                           pokazuje poziciju/koordinate kursora (u donjem desnom kutu)
set showcmd                         pokazuje nedovršene naredbe (u donjem desnom kutu)
set wildmenu                        uključuje *menu*/*tab*-opcije za završavanje naredbi
set scrolloff=5                     postavlja broj linija koja će se vidjeti iznad kursora
set hlsearch                        uključuje *highlighting* kod traženja
set incsearch                       uključuje inkrementalno pretraživanje
set ignorecase                      ignorira veliko/malo slovo kod pretraživanja
set smartcase                       *override* ignorecase ako pretraga uključuje velika slova
set number                          uključuje numeraciju linija
set backup                          uključuje stvaranje *back-up*-a datoteka prije njihovog *save*-anja
set bex=SOMETHING                   postavlja ekstenziju imena *back-up* datoteka
set lbr                             uključuje line-wrapping bez prelamanja slova
set ai                              uključuje *auto-indentation* (novi red ima istu indentaciju kao trenutni)
set si                              uključuje *smart-indentation* (uključuje indentaciju za neke programske jezike) (koristiti s prethodnom opcijom)
set bg=light                        uključuje *syntax-highlighting* koji vizualno paše na svijetle pozadine
set bg=dark                         uključuje *syntax-highlighting* koji vizualno paše na tamne pozadine
color slate                         postaljanje sheme boja "slate"
map <F2> iKristijan<CR>Mrkalj<CR><ESC>  mapira naredbu za tipku F2, slično kao macro
let mapleader=","                   postavljaju drugi leader key (umjesto \)
map <leader>w :w!<CR>               zamjenjuje \w (ili ,w ako je postavljeno kao gore) da radi isto što i :w!
