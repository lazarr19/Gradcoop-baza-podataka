# Gradcoop - baza podataka
Microsoft Access baza podataka za građevinsku kompaniju Gradcoop

Program se sastoji od nekoliko važnih komponenti prčemu su najvažnije:
  - Praćenje protoka goriva
  - Troškovi gradilišta i mehanizacije
  - Magacin
  - Sistem zahteva i zaduženja
  

## Magacin

Magacin predstavlja deo programa koji se odnosi na digitalno skladište artikala koji se trenutno zaista nalaze u okviru magacina.

Trenutno nemamo više fizičkih magacina već samo jedan, pa je tome prilagođen i digitalno skladištenje podataka.

Osnove tabele koje čine magacin su:
  - Tip Artikla
  - Artikal
  - Racun

Više o svakoj od njih i rukovanju njima je opisano na stranici [Magacin](docs/Magacin.md).


## Sistem zahteva i zaduženja

Veoma nam je značajno da precizno vodimo evidenciju o zaduživanju artikala iz magacina i službenih vozila.

Ovde je detaljno opisan način na koji bi sistem zahteva trebao da funkcioniše u okviru ovog programa.
Ideja je da opisom ovih procedura pomognemo svakome ko koristi program za praćenje zahteva.

Osnovne tabele koje čine ovu sekciju su:
  - Zahtev
  - Zaduženje
  - Mesto
  - Montaža

Detaljnije o ovim tabelama i procesima između njih možete pročitati na stranici [Sistem zahteva i zaduženja](docs/Sistem zahteva i zaduženja).

