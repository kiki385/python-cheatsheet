# Medjuspremnici / Buffers

vim file1.txt file2.txt otvara obje datoteke u memoriju

:buffers                :ls             otvara listu međuspremnika (otvoreni fileovi i trenutne pozicije kursora)
                                        a       file je učitan i prikazan (active)
                                        h       file je učitan i nije prikazan (hidden)
                                                file nije učitan i nije prikazan (active)
                                        %       file koji se trenutno pregledava
                                        #       označava prethodno otvoreni file
                                        +       označava da je file uređen od zadnjeg spremanja

```
Nisu svi fileovi učitani u memoriju, već samo oni s oznakama h i a.
Fileovi bez oznake su "unloaded" iz memorije, a vim za njih pamti samo neke metapodatke.
```


:b 1                                            otvara međuspremnik 1
:b file1.txt                                    otvara file1.txt ako se on nalazi u međuspremniku
:bnext                  :bn                     otvara idući file
:bprevious              :bp                     otvara predhodni file
:bfirst                 :bf                     otvara prvi file
:blast                  :bl                     otvara zadnji file
Ctrl + ^                                        otvara ranije otvoreni file
:badd file3.txt         :ba file3.txt           dodaje file u međuspremnik
:bdelete [file3.txt]    :bd [file3.txt]         uklanja trenutni file/[file3.txt] iz međuspremnika

:wqall                                          :wq za sve fileove u memoriji
:qall!                                          :q! za sve fileove u memoriji

:bufdo %s/"staro"/"novo"/g | w                  izvršava naredbu za sve fileove, a zatim sprema promjene
                                                | je separator naredbi u vim-u

:E                                              *explorer* datoteka u trenutnom direktoriju
                                                za izlazak iz explorera, upisati :bd

:set hidden                                     omogućuje da se *file*-ovi ne unloadaju iz memorije
                                                na taj način nije potrebno stalno forsirati save trenutnog file-a prije prebacivanja na idući i slično
