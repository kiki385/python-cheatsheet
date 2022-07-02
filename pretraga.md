# Pretraga

## "Linijske" pretrage

Kursor se pozicionira na mjestu pretrage:
f<znak>         pretraga znaka u liniji, unaprijed
F<znak>         pretraga znaka u liniji, unazad

Kursor se pozicionira na mjestu *prije* pretrage:
t<znak>         pretraga znaka u liniji, unaprijed
T<znak>         pretraga znaka u liniji, unazad

;               ponavljanje pretrage, unaprijed
,               ponavljanje pretraga, unazad


## "Globalne" pretrage

/<znak>         pretraga znaka duž cijelog teksta (ono što se traži ostaje memorirano), unaprijed
?<znak>         pretraga znaka duž cijelog teksta (ono što se traži ostaje memorirano), unazad

n               prelazak na idući rezultat pretraga
N               prelazak na prethodni rezultat pretrage

*               pretraga riječi ispred znaka, unaprijed
#               pretraga riječi iza znaka, unazad

```
Pretraga funkcionira kao pokret, pa vrijedi:
<naredba><pokret>
```

```
Ovaj mehanizam omogućava pretragu te brisanje teksta, npr.:
/and            pretraga riječi "and"
dw              brisanje te riječi
n               odlazak na iduću instancu riječi "and"
.               ponavljanje zadnje **naredbe** (brisanje)
```

## Primjeri

dfa             brisanje svega do prvog znaka "a"
d/This          brisanje svega do prve instance riječi "This"
"ay/This        *yank*-anje svega do riječi "This" u registar a
