# Brisanje

x       brisanje znaka na kursoru (delete)
X       brisanje znaka ispred kursora (backspace)

d       naredba za brisanje

dd      brisanje cijele linije

Općenito vrijedi:
```
d<pokret>
<broj-ponavljanja>d<pokret>
```
... čime će se brisanje ponoviti za određeni uvijet, npr:
* d3j                   brisanje 1 trenutne + 3 linije dolje
* 3dd                   brisanje 1 trenutne + 2 linije dolje
* d3w                   brisanje 3 riječi udesno 
* d^    d0              brisanje do početka linija (prvi znak uključen)
* d$    D               brisanje do kraja linije (zadnji znak uključen)
* dgg                   brisanje do početka teksta (prvi znak uključen)
* dG                    brisanje do kraja teksta (zadnji znak uključen) 
* d3gg  d3G             brisanje do 3. linije (3. linija uključena)
