# Prozori

:split [file]       :sp [file]      Ctrl+w s        otvara datoteku u još jednom prozoru (horizontalno)
:vsplit [file]      :vs [file]      Ctrl+w v        otvara datoteku u još jednom prozoru (vertikalno)
:ball               :ba                             otvara sve datoteke iz međuspremnika u svoje prozore
                                    Ctrl+w q        zatvara trenutni prozor
:only               :on             Ctrl+w o        zatvara sve prozore osim trenutnog

:windo %s/"staro"/"novo"/g                          izvršava naredbu na svim prozorima
                                                    slično kao i :bufdo, ali samo na prozorima

Ctrl+w w                                            prebacuje se u drugi prozor
Ctrl+w h                                            prebacuje se u prozor lijevo
Ctrl+w l                                            prebacuje se u prozor desno
Ctrl+w j                                            prebacuje se u prozor dolje
Ctrl+w k                                            prebacuje se u prozor gore

Ctrl+w +                                            povećava prozor (vertikalno)
Ctrl+w -                                            smanjuje prozor (vertikalno)
Ctrl+w >                                            povećava prozor (horizontalno)
Ctrl+w <                                            smanjuje prozor (horizontalno)
Ctrl+w _                                            maksimizira prozor po horizontali
Ctrl+w |                                            maksimizira prozor po vertikali
Ctrl+w =                                            svi prozoru postaju jednake veličine

Ctrl+w r                                            rotira sadržaj prozora (2 <- 1, 3 <- 2, 1 <- 3)
Ctrl+w R                                            rotira sadržaj prozora (obrnuti smjer od gornjeg)
Ctrl+w H                                            pozicionira aktivni prozor lijevo
Ctrl+w L                                            pozicionira aktivni prozor desno
Ctrl+w J                                            pozicionira aktivni prozor dolje
Ctrl+w K                                            pozicionira aktivni prozor gore
