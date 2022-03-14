# Gradcoop - baza podataka
Dokumentacija za Microsoft Access bazu podataka za građevinsku kompaniju Gradcoop.

Program se sastoji od nekoliko važnih funkcionalnih komponenti pri čemu su najvažnije:
  - [Praćenje protoka goriva](#praćenje-protoka-goriva)
  - [Troškovi gradilišta i mehanizacije](#troškovi-gradilišta-i-mehanizacije)
  - [Magacin](#magacin)
  - [Sistem zahteva i zaduženja](#sistem-zahteva-i-zaduženja)


Ovde je detaljno opisan način na koji bi svaki funkcionalni sistem trebao da funkcioniše u okviru ovog programa.
Ideja je da opisom ovih procedura pomognemo svakome ko koristi program.


## Praćenje protoka goriva

Tek treba da se uradi dokumentacija za ovu sekciju.


## Troškovi gradilišta i mehanizacije

Tek treba da se uradi dokumentacija za ovu sekciju.


## Magacin

Magacin predstavlja deo programa koji se odnosi na digitalno skladište artikala koji se trenutno nalaze u okviru fizičkog magacina.

Trenutno nemamo više fizičkih magacina već samo jedan, pa je tome prilagođeno i digitalno skladištenje podataka.

Osnove tabele koje čine magacin su:
  - Tip Artikla
  - Artikal
  - Racun

Više o svakoj od njih i rukovanju njima opisano je na stranici [Magacin](./docs/Magacin.md).


## Sistem zahteva i zaduženja

Veoma nam je značajno da precizno vodimo evidenciju o zaduživanju artikala iz magacina i službenih vozila.

Osnovne tabele koje čine ovu sekciju su:
  - Zahtev
  - Zaduženje
  - Mesto
  - Montaža

Detaljnije o ovim tabelama i procesima između njih možete pročitati na stranici [Sistem zahteva i zaduženja](./docs/Sistem%20zahteva%20i%20zaduženja.md).

