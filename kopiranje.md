# Kopiranje

y               kopiranje znaka
yy              kopiranje linije

p               paste iza kursora
P               paste prije kursora

```
Obrisano i kopirano se sprema u registre.
""          neimenovani registar za y, d i x
"0          registar za y
"1 - "9     registri za d i x
"a - "z     registri za štogod
"_          "black hole" registar
"+          sistemski clipboard (potreban je paket vim-X11 i binary vimx)
```

u           undo naredbe
ctrl+r      redo naredbe

Vrijedi:
```
<registar><broj-ponavljanja><operacija>
```

"ayy        kopiranje linije u registar a
"Ayy        kopiranje linije u registar a (append)

"h3dd       *cut*-anje tri linije u registar h
"H3dd       *cut*-anje tri linije u registar h (append)

"ap         *paste*-anje linije iz registra a
 "a3p       *paste*-anje linije iz registra a tri puta

:reg        pregled registra (registar je *system-wide*, tj. nije vezan za trenutnu datoteku)
:reg abc    pregled registara za a, b i c
