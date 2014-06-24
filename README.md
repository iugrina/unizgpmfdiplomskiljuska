LaTeX ljuske za izradu diplomskog rada pri Prirodoslovno-matematičkom fakultetu
(Matematičkom odsjeku) Sveučilišta u Zagrebu.

Primjerke ljuski možete naći u "doc" direktoriju.

**Napomena**: Budući da se pravila često mijenjaju moguće je da ove ljuske neće u
potpunosti odgovarati zahtjevima odsjeka.


## Ljuska A

* datoteka bibliografija/diplomski_bibliografija.bib sluzi za unos bibliografije po BibTeX standardu. 
* datoteka diplomski_ljuska.tex je centralna datoteka rada. naslove poglavlja mijenjate u ovoj datoteci.
* dateteke include/diplomski_bibliografija.tex, include/diplomski_naslovnica.tex i include/diplomski_povjerenstvo.tex su standardnog oblika za nas fakultet i vecina vas ne bi trebala to mijenjati (nap. mjenjajte samo ako znate sto radite)
* u datoteke include/diplomski_uvod.tex i include/diplomski_zakljucak.tex napisete Uvod i Zakljucak
* u folder slike/ spremite slike koje ste napravili
* slika slike/slika_3-1.eps sluzi kao primjer i koristena je da bi se napravili
* vecinu pisanja potrebno je napraviti u zasebnim datotekama u folderu input/ koje ce predstavljati section-e vaseg diplomskog rada. kao primjer dao sam tri datoteke. Pazite da zaglavlja iz primjera koristite i kod vas uz promjene naslova i label-a

**Kompajliranje**:

a) ako ste odkomentirali liniju
```
%\includeonly{}
```
i u naredbi niste naveli ```include/diplomski_bibliografija```
onda kompajlirate sa:
```
$ latex diplomski_ljuska.tex
```

b) inace je potrebno pokrenuti i bibtex
```
$ latex diplomski_ljuska.tex
$ bibtex diplmoski_ljuska
$ latex diplomski_ljuska.tex
$ latex diplomski_ljuska.tex 
```

c) ili koristiti
[Latexmk](http://users.phys.psu.edu/~collins/software/latexmk-jcc/)

## Ljuska B

Za ljusku B vrijede slični komentari kao i za ljusku A. Pametni ste, vjerujem da
ćete se snaći ;)
