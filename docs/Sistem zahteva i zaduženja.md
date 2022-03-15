# Sistem zahteva i zaduženja 

Ova stranica opisuje osnovne komponenete sistema koji upravlja zahtevima i zaduženjima u okviru programa.

Veoma je bitno dobro razumeti procedure i tok kojim se treba voditi kako bi se vodila ispravna evidencija.


Dokument sadrži opise sledećih procedura:
  - [Formiranje zahteva](#formiranje-zahteva)
    - [Dodavanje zahteva](#dodavanje-zahteva)
    - [Odobravanje zahteva](#odobravanje-zahteva)
    - [Poručivanje zahteva](#poručivanje-zahteva)
    - [Storniranje zahteva](#storniranje-zahteva)
    - [Pregled zahteva](#storniranje-zahteva)
  - [Formiranje zaduženja](#formiranje-zaduženja)
    - [Kreiranje i vrste zaduženja](#kreiranje-i-vrste-zaduženja)
    - [Montaža i zaduženje](#montaža-i-zaduženje)
    - [Pregled zaduženja](#pregled-zaduženja)
  - [Formiranje povratnica](#formiranje-povratnica)
    - [Dodavanje povratnica](#dodavanje-povratnica)
    - [Rashodovanje artikala](#rashodovanje-artikala)
    - [Premeštaj artikala](#premeštaj-artikala)


## Formiranje zahteva

Zahtev predstavlja pismeno ili usmeno potraživanje nekog radnika firme za određenim artiklom. Najčešći primeri su zamena guma na mašini, uzimanje službenog vozila ili zamena akumulatora.

Dakle, zahtev se formira tako što radnik usmeno (uglavnom bolje pismeno, SMS porukom, kako bi ostali podaci i dokaz o traženom zahtevu) potražuje određeni artikal.

Na zahtev korisnik programa reaguje prateći sledeću proceduru:
  
  1. [Dodavanje zahteva](#dodavanje-zahteva)
  2. [Odobravanje zahteva](#odobravanje-zahteva)
  3. [Poručivanje zahteva](#poručivanje-zahteva)

### Dodavanje zahteva

Prvo je neophodno da se zahtev pribeleži u programu.

Procedura koja treba da se prati prilikom te operacije je sledeća:

  1. Klikom na dugme ***Dodaj zahtev*** se otvara nova forma
  2. Popuniti sva tražena polja koja su trenutno dostupna i odgovarajuća za novi zahtev
     * U slučaju da se zahtev (zajedno sa artiklima koji ce kasnije biti pridruženi njemu) odnosi na gradilište odabrati tu opciju ***Gradilište***
     * U slučaju da se zahtev odnosi na nabavku/zamenu ili neki sličan zahtev za delovima odabrati opciju ***Mašina***
     * U slučaju da je zahtev za zaduživanjem vozila odabrati opciju ***Radnik - zaduženje službenog vozila***
  3. Nakon odabira ***Na šta se zahtev odnosi*** biće omogućen i odabir odgovarajućeg gradilišta, mašine odnosno radnika ***koji će koristiti službeno vozilo***.
  4. Nastaviti proceduru klikom na dugme ***Dodaj artikle***
  
Klikom na dugme ***Dodaj artikle*** će se otvoriti nova forma za unos. Na njoj će biti prikazani neki prethodno uneti podaci kao dodatna polja Tip artikala, Pozicija, Količina.

Takođe tu se nalazi tabelarni prikaz trenutnog zahteva kako bi korisnik imao potpunu i ažurnu sliku o tome koje artikle je do sad dodao u ovaj zahtev. Procedura se nastavlja:
  
  5. Odabrati tip artikla na koji se zahtev odnosi pomoću polja ***Tip artikla***
     * U slučaju da odgovarajući artikal ne postoji klikom na dugme ***Unesi novi artikal*** se otvara tabela sa tipovima artikla koji postoje u sistemu. Veruje se korisniku da ispravno unese novi tip ne dirajući ostale. Nakon ***čuvanja*** prethodne izmene novi artikal će moći da se odabere u polju ***Tip artikla***.
  6. Polje ***Pozicija*** će biti omogućeno u slučaju da je odabrano mesto izmene ***Mašina*** i ***Tip artikla Guma*** i odnosi se na poziciju gume na odgovarajućoj mašini.
  7. Polje ***Količina*** se odnosi na broj artikala koji su u odgovarajućem zahtevu.
  8. Klikom na dugme dodaj još artikala se ponovo otvara ista forma pri čemu je sada moguće dodati drugi tip artikala. (Ovaj korak ***nije neophodan*** ukoliko postoji ***samo jedan*** tip artikla)
  9. Klikom na dugme ***Zaključi zahtev*** se zaključuje prethodni zahtev u potpunosti i zatvara se forma.


### Odobravanje zahteva

Tek nakon što je zahtev kreiran, odnosno dodat, potrebno je odobriti ga.

Odobravanje treba da bude konsultovanje sa ***nadležnim licem*** u firmi za tu operaciju, koja mora dati odobrenje za odgovarajući zahtev.
Podaci o osobi koja odobrava zahtev, kao i datumu odobrenja se unose prilikom ovog koraka.

  1. Klikom na dugme ***Odobri zahtev*** se otvara nova forma
  2. Zahtev koji će biti odobren se bira na osnovu polja ***Id zahteva*** gde je prikazano ko je podnosilac zahteva, datum zahteva i napomena ukoliko postoje.
     * Nakon odabira nekog zahteva automatski se ažurira tabela sa strane koja sadrži sve elemente odabranog zahteva i služi korisniku za bolji pregled
  3. Potrebno je odabrati odgovarajuće lice koje odobrava ovaj zahtev kroz polje ***Zahtev odobrio***
  4. Uneti datum odobravanja kroz polje ***Datum odobrenja*** (ne mora biti isto kao i datum zahteva)
  5. Klikom na dugme ***Odobri zahtev*** završiti odobravanje zahteva

### Poručivanje zahteva

Nakon što je zabeleženo da je zahtev odobren, u slučaju da je npr. zahtev za nabavkom delova, potrebno je poručiti odgovarajuće delove.

U programu se takođe beleže informacije o ovom događaju kroz sledeće korake:

  1. Klikom na dugme ***Poruči zahtev*** se otvara nova forma
  2. Zahtev koji će biti odobren se bira na osnovu polja ***Id zahteva*** gde je prikazano ko je podnosilac zahteva, datum odobrenja i napomena ukoliko postoje.
     * Nakon odabira nekog zahteva automatski se ažurira tabela sa strane koja sadrži sve elemente odabranog zahteva i služi korisniku za bolji pregled
  3. Uneti datum poručivanja kroz polje ***Datum poručivanja*** (ne mora biti isto kao i datum zahteva ili datum odobrenja)
  4. Klikom na dugme ***Poruči zahtev*** završiti poručivanje artikala sa ovog zahteva

***Važno pitanje: da li je potrebno poručiti svaki zahtev, npr. i onaj za službenim vozilom?, to baš nema smisla, kako odrediti koji se poručuju a koji ne?***

### Storniranje zahteva

U slučaju da je došlo do greške prilikom kreiranja zahteva, potrebno je stornirati ga sledećom procedurom
  
  1. Klikom na dugme ***Storniraj zahtev*** se otvara nova forma
  2. Zahtev koji će biti odobren se bira na osnovu polja ***Id zahteva*** gde je prikazano ko je podnosilac zahteva i napomena ukoliko postoje.
  3. Klikom na dugme ***Storniraj*** se odabrani zahtev stornira i izazi se iz forme.
  
  ***Biti veoma oprezan prilikom ove operacije i nekoliko puta proveriti odgovarajući ID zahteva koji će biti storniran. Greška može dovesti do bezpovratnog gubitka podataka.***


Napomena: Biti veoma pažljiv sa odabirom zahteva koji se stornira jer je ova operacija nepovratna, tj. nije moguće vratiti stornirane podatke.

### Pregled zahteva

Najvažniji deo prilikom rada sa zahtevima jeste i dobar pregled svih zahteva koji postoje u programu.
Korisnik programa ***treba često da koristi*** ovu mogućnost kako bi i on sam bio u toku sa trenutnim dešavanjima.

Detaljan pregled je omogućen sledećom procedurom:

  1. Klikom na dugme ***Pretraži zahteve*** se otvara nova forma
  2. U novootvorenoj formi se nalazi mnogštvo karakteristika zahteva i moguće je postaviti razne uslove kako bi se odredio zahtev koji je potrebno detaljnije ispitati
     * Ukoliko korisnik želi da odredi datum zahteva koji se nalazi između dva perioda (npr. za Datum zahteva želi da bude pre 1.1.2023. unosi tu vrednost u polje ***Datum zahteva do***, za pravilan rad programa ***neophodno*** je i da unese neku vrednost za ***Datum zahteva od***, npr. 1.1.2020.
     * Ukoliko korisnik želi da pregleda ***sve zahteve*** dovoljno je da ne menja vrednosti nijednog polja i samo klikne na dugme ***Pretraži***
  3. Klikom na dugme ***Pretraži*** se prikazuje tabela zahteva koji zadovoljavaju zadate kriterijume i ona sadrži dosta detaljnih informacija

Ukoliko se primete bilo kakve ***neregularnosti*** ili ***nelogičnosti*** prilikom pregleda zahteva, potrebno je reagovati na njih. Ukoliko su tehničke prirode kontaktirati ***stučna lica*** ili ukoliko je problem manje prirode (npr. greška u datumu) samostalno izmeniti podatke uz ***dosta*** opreza.


## Formiranje zaduženja

Zaduženja predstavljaju novu vrstu objekata sa kojim se korisnik može susresti u ovom programu. Naravno, svako zaduženje aritkala ne može postojati samo od sebe već je potrebno da za njega postoji određeni zahtev.

Zaduženja se ne prave ekplicitno već prilikom ***potvrđivanja*** zahteva dolazi do automatskog kreiranja zaduženja određenih artikala na određeno mesto.

Kao što možemo videti u prethodnoj rečenici za zaduženja su ključni: 
  - ***Artikal*** koji je zadužen
  - ***Mesto*** na kome je zadužen artikal (Gradilište, Mašina, Mašina sa pozicijom, Radnik - zaduživanje službenog vozila)
  - ***Montaža*** artikla na određeno mesto - ***najvažniji deo*** zaduženja (***važno***: montaža ne mora eksplicitno da znači fizičko montiranje objekta, može da bude i uručivanje ključeva radniku za službeno vozilo)

Detaljnije o ovim delovima zaduženja pogledati u sledećoj sekciji.

### Kreiranje i vrste zaduženja

Kao što je rečeno, zaduženja nije potrebno da eksplicitno pravi korisnik programa već se ona prave automatski prilikom kreiranja zahteva.

Detaljnije ćemo opistai svaki od važnih delova koji čine zaduženje:

  - ***Artikal*** je određeni artikal koji je glavni objekat jednog zaduženja
     - Prilikom kreiranja zahteva bira se ***tip artikla*** koji je zahtevan i upravo taj tip nam određuje koji artikli mogu da dođu u opticaj za kreirano zaduženje
     - Kako je u zahtevu samo specifikovan tip artikla koji je potreban, neophodno je pridružiti ***tačno određeni artikal*** zaduženju i taj korak se radi prilikom ***montaže***
  - ***Mesto*** predstavlja lokaciju na koju se zahtev odnosi. Trenutno u sistemu postoje 4 tipa mesta i to su:
     - Gradilište
     - Mašina
     - Mašina sa pozicijom (razlika u odnosu na Mašina je što je specifikovana i pozicija na koju se stavlja artikal - trenutno jedino korišćeno za praćenje pozicija guma na mašinama)
     - Radnik - zaduženje službenog vozila 
    
    Jedino je potrebno malo detaljnije objasniti stavku ***Radnik - zaduženje službenog vozila*** jer je svaka prethodna jasna.
    Naime, kada je potrebno zadužiti službeno vozilo, mesto koje je nama najznačajnije nije sama mašina već radnik jer njemu dodeljujemo službeno vozilo koje u ovom slučaju ima zapravu ***ulogu artikla*** (deluje malo nelogično ali kada se posmatra da uvek dodeljujemo artikal na određeno mesto ima smisla uvesti ovakve oznake).

Posebna sekcija je izdvojena kako bi se objasnio odnos između montaže i zaduženja

### Montaža i zaduženje

Prilikom montaže artikla i zadovoljavanja određenog zahteva potrebno je pratiti sledeću logiku:

  - ***Gde se montira/zadužuje***: Prvo je potrebno odrediti ***mesto*** na kojem je nešto potrebno da se zaduži, odnosno montira (prateći sva prethodna poglavlja do sad bi trebalo da nam bude jasno da to može biti neko Gradilište, Mašina, Mašina sa pozicijom ili Radnik (Radnik - zaduženje službenog vozila)).
  - ***Šta se montira/zadužuje***: Nakon određivanja mesta, potrebno je odretiti ***šta*** se zadužuje odnosno montira. Ovaj korak je neophodan jer je moguće da je na istom mestu aktivno nekoliko zahteva za ***različitim artiklima*** (npr. na mašini je moguće da je istovremeno potrebno zameniti akumulator i filter za ulje, što predstavlja dve stvari koje mogu da se montiraju na mašinu)
  - ***Artikl***: Nakon toga je potrebno tačno odrediti artikal koji će biti zadužen, odnosno montiran. Kako je moguće montirati samo ono što trenutno imamo u magacinu (uključujući i službena vozila) potrebno je odabrati nešto od toga. Ovde korisnik programa mora biti ***VEOMA OPREZAN*** jer u slučaju da odabere artikal koji ***nije zaista montiran***, već neki drugi, može doći do nesaglasnosti podataka u programu i stvarnom svetu. Dakle, biti veoma ***pažljiv*** prilikom odabira artikla.
  - ***Račun montaže***: Dalje je potrebno u sistem povezati račun koji se odnosi na ovu montažu. Ukoliko taj račun postoji on bi trebao već da bude unesen u program kroz dugme ***Dodaj račun***. Više o tome pogledati !!!OVDE!!!. Takođe, treba imati na umu da je moguće da ***nema računa*** samo u slučaju ukoliko su radnici u radionici ***sami monitrali*** deo.
  - ***Montirao***: Bitno je uneti i informaciju o tome ***ko je*** montirao, odnosno zadužio određeni artikal. U slučaju da je to urađeno u našoj radionici pribeležiti ***odgovornog majsotra***, a u slučaju da je to urađeno od strane nekog ***dobavljača*** odabrati njegovo ime (ako dobavljač ne postoji dodati ga na neki od prethodnih načina).

Uz prethodo opisane korake ostaje jasno kako bi trebalo popuniti formu koja se dobija na sledeći način:

  1. Klikom na dugme ***Dodaj montažu*** se otvara nova forma
  2. U novootvorenoj formi se nalaze prethodno opisana polja i neka dodatna za koje nije potrebno detaljno objašnjenje (npr. datum montaže) koja je potrebno ispravno popuniti
  3. Klikom na dugme ***Potvrdi montažu*** se zaključuje uneta montaža

### Pregled zaduženja

Najvažniji deo prilikom rada sa zaduženjima jeste i dobar pregled svih zaduženja koji postoje u programu.
Korisnik programa ***treba često da koristi*** ovu mogućnost kako bi i on sam bio u toku sa trenutnim dešavanjima.

Detaljan pregled je omogućen sledećom procedurom:

  1. Klikom na dugme ***Pretraži zaduženja*** se otvara nova forma
  2. U novootvorenoj formi se nalazi mnogštvo karakteristika zaduženja i moguće je postaviti razne uslove kako bi se odredio zahtev koji je potrebno detaljnije ispitati
     * Ukoliko korisnik želi da odredi datum zahteva koji se nalazi između dva perioda (npr. za Datum zahteva želi da bude pre 1.1.2023. unosi tu vrednost u polje ***Datum zahteva do***, za pravilan rad programa ***neophodno*** je i da unese neku vrednost za ***Datum zahteva od***, npr. 1.1.2020.
     * Ukoliko korisnik želi da pregleda ***sva zaduženja*** dovoljno je da ne menja vrednosti nijednog polja i samo klikne na dugme ***Pretraži***
  3. Klikom na dugme ***Pretraži*** se prikazuje tabela zahteva koji zadovoljavaju zadate kriterijume i ona sadrži dosta detaljnih informacija

Ukoliko se primete bilo kakve ***neregularnosti*** ili ***nelogičnosti*** prilikom pregleda zahteva, potrebno je reagovati na njih. Ukoliko su tehničke prirode kontaktirati ***stučna lica*** ili ukoliko je problem manje prirode (npr. greška u datumu) samostalno izmeniti podatke uz ***dosta*** opreza.


## Formiranje povratnica

### Dodavanje povratnica

### Rashodovanje artikala

### Premeštaj artikala



