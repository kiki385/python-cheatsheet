# Macro

*Macro*-i služe za ponavljanje kompleksnih radnji, korištenjem snimanja radni.

q<registar>               započinje i završava snimanje *macro*-a koji će se pohraniti u neki registar
qa

Nakon što je snimanje započeto, provode se radnje koje će se snimati.

Snimljeni macro se izvršava korištenjem registra.

@<registar>               izvršava radnju snimljenu u registar
@a

Registar se može jednostavno izmijeniti, tako da se *paste*-a i zatim ručno izmjeni.

"<registar>p              *paste*-a registar u tekst
"<registar>dd             briše tekst te ga pohranjuje u registar
"ap
"add

:<domet> normal @<registar>      izvršava macro na dometu
:1,6 normal @a

Domet može biti:

1,.                         od prve linije do kraja teksta
.,$                         od trenutne linije do kraja teksta
%                           kroz cijeli tekst

3@a                         izvršava *macro* tri puta

*macro*-i se mogu pohraniti u `.vimrc` konfiguracijski file.
let @a = '<macro>'

```
*literal* znakovi, npr. Esc, Enter i slično mogu se upisati:
i           uključuje insert mode
Ctrl+v      uključuje literal mode unutar insert mode-a
Esc         ubacuje literal Esc
```

Preporuke:
```
Na početku *macro*-a pomaknuti se na početak s 0 ili ^.
Na kraju *macro*-a pomaknuti se na liniju ispod s j.
```
