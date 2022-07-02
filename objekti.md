# Objekti

Vim prepoznaje pojam sljedećih objekata:

w               riječ (word)
s               rečenica (sentance)
p               paragraf
( ili )         sadržaj oblih zagrada         
[ ili ]         sadržaj uglatih zagrada
{ ili }         sadržaj vitičastih zagrada
< ili >         sadržaj izlomljenih zagrada
"               sadržaj navodnika
'               sadržaj navodnika
`               sadržaj navodnika
t               tag (prostor unutar nekog *tag*-a, npr. <primjer>prostor</primjer>

Nad tim objektima, moguće je izvoditi radne kao što su *delete*, *yank*, *change*..., a te radnje se mogu modificirati "koeficijentima":
* a             a - uključuje "separator objekta"
* i             inside - ne uključuje "separator objekta"
npr.:

daw             briše riječ i razmak                    delete a word
diw             briše riječ                             delete inside word
da(             briše sadržaj zagrada i zagrade         delete a (
di(             briše sadržaj zagrada                   delete inside (
dat             briše *tag* i njegov sadržaj            delete a tag
dit             briše sadržaj *tag*-a                   delete inside tag
