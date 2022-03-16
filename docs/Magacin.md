# Magacin

Ova stranica opisuje osnovne komponenete magacina i načine za dodavaje novih artikala i računa, storniranje netačnih i pregled unetih računa.

Dokument sadrži opise sledećih procedura:
  - [Formiranje računa](#formiranje-računa)
     - [Dodavanje artikala bez računa](#dodavanje-artikala-bez-računa) (Napomena: raditi samo u posebnim situacijama)
     - [Dodavanje računa](#dodavanje-računa)
     - [Storniranje računa](#storniranje-računa)
     - [Prikaz artikala sa računa](#prikaz-artikala-sa-računa)
  - [Slobodna vozila](#slobodna-vozila)
  - [Stanje magacina](#stanje-magacina)

## Formiranje računa

Ova sekcija je neophodna za razumevanje svih koraka koji se tiču kreiranja artikala u programu, dodavanja računa i prikazivanja računa i artikala koji već postoje.

Sekcija je podeljena u sledeće delove:
  1. [Dodavanje artikala bez računa](#dodavanje-artikala-bez-računa) (Napomena: raditi samo u posebnim situacijama)
  2. [Dodavanje računa](#dodavanje-računa)
  3. [Storniranje računa](#storniranje-računa)
  4. [Prikaz artikala sa računa](#prikaz-artikala-sa-računa)

### Dodavanje artikala bez računa

Nekada je potrebno da se artikli dodaju u magacin bez računa i ovaj način ***ne bi trebalo generalno koristiti*** jer svaki artikal treba da ima svoje poreklo. Misli se na to da se dodaju bez računa, odnosno da se naprave artikli a da za njihovo postojanje ne postoji račun koji to opravdava.

Prethodno je neophodno uraditi samo u ***posebnim situacijama***, npr. kada je potrebno napraviti početno stanje magacina. (jer ne znamo koji su računi bili za te artikle u prošlosti).

Način na koji se to radi opisuje sledeća procedura:

  1. Klikom na dugme ***Dodaj artikl u magacin*** se otvara nova forma
  2. Potrebno je odabrati ***tip artikla***, ***oznaku*** i opcionu dodati serijski broj mada imati na umu da on ***nije obavezan***.
  3. U slučaju da je potrebno dodati tip artikla koji ne postoji trenutno u programu, on se može dodati klikom na dugme ***Unesi novi tip artikla***
   * Potrebno je u redu koji počinje sa ***(New)*** dodati red sa odgovarajućim nazivom za novi tip artikla i sačuvati tabelu prečicom ***Ctrl + S*** ili desnim klikom na tab i klikom na dugme ***Save***.
  4. Ukoliko je potrebno dodati više artikala ići na dugme ***Dodaj još artikala*** koje će ponovo otvoriti istu formu. U slučaju da se unosi poslednji artikal on se unosi klikom na dugme ***Zaključi unos*** i zatvara se forma.

***Napomena: biti veoma obazriv prilikom dodavanja novih aritkala. Naime, ukoliko postoji artikal Guma, nije potrebno praviti novi artikal Guma Michelin, već iskoristiti postojeći Guma, a detalje artikla navesti u polju oznaka.***

### Dodavanje računa

Prilikom svakog pristizanja novog računa koji se odnosi na artikle koji se skladište u okviru magacina ili se neposredno odnose na magacin, potrebno je zabeležiti informacije o tom računu.

  1. Klikom na dugme ***Dodaj račun*** se otvara nova forma
  2. Potrebno je ispravno popuniti polja
     * Za polje ***Broj računa*** je poželjno iskorititi broj računa koji se nalazi na samom fizičkom papiru. Postoji mogućnost da istovremeno budu dva računa sa istim brojem tako da je potrebno ***biti pažljiv***.
     * U polju ***Dobavljač*** odabrati odgovarajućeg dobavljača, a u slučaju da on ne postoji dodati ga klikom na dugme ***Unesi novog dobavljača***. Nakon unošenja podataka o novom dobavljaču potrebno je sačuvati tabelu sa dobavljačima da bi se on mogao odabrati.
     * Uneti vrednost računa bez PDV-a u polje ***Ukupna cena bez PDV*** i unošenjem procenta PDV se ***automatski izračunava*** vrednost polja ***Ukupna cena sa PDV***.
  3. Nakon završenog unošenja podataka nastaviti dalje klikom na dugme ***Dodaj artikle***

Ovim postupkom je završeno unošenje osnovnih informacija o računu. Potrebno je uneti podatke za artikle koji se nalaze na njemu i to prateći sledeću proceduru:

  1. U novootvorenoj formi je potrebno uneti vrednosti sledećih polja:
     * ***Tip artikla***: određuje koja vrsta artikla se unosi (U slučaju da tip artikla ne postoji u programu potrebno ga je dodati klikom na dugme ***Unesi novi tip artikla***. Nakon unošenja podataka o novom tipu artikla potrebno je sačuvati tabelu sa tipovima artikala da bi se on mogao odabrati).
     * ***Oznaka artikla***: ova oznaka treba ***što detaljnije*** da opisuje tip artikla na koji se odnosi (npr. neka je tip artikla Guma, onda bi ispravna oznaka bila zimska Michelin 255/55/17).
     * ***Količina***: Ukoliko se na računu nalazi više artikala istog tipa i oznake, moguće je istovremeno uneti sve odjednom pomoću vrednosti polja ***Količina***. Dakle, ukoliko se unosi jedan artikal, potrebno je da količiina bude 1, a ukoliko se na računu nalaze četiri ***ista*** artikla, potrebno je staviti količinu na 4.
  2. Ukoliko je potrebno dodati još artikala to je moguće uraditi klikom na dugme ***Dodaj još artikala***.
     * Svi do sada dodati artikli će se prikazivati u tabeli koja se nalazi na formi. To omogućuje bolju preglednost korisniku programa i smanjuje mogućnost za grešku.
  3. Ukoliko nije potrebno dodati više artikala ili se dodaje poslednji artikal u nizu, klikom na dugme ***Zaključi račun*** se zatvara forma


Imati u vidu da se dodavenjem računa artikli sa njega automatski smeštaju u virtuelni magacin, pa može doći do neslaganja stvarne situacije u magacinu i stanja u programu.

### Storniranje računa

U slučaju da je došlo do greške prilikom unosa određenog računa potrebno je stornirati račun.

1. Klikom na dugme ***Storniraj račun*** se otvara nova forma
2. Potrebno je odabrati broj računa koji će se stornirati. Pored broja računa se nalazi i odgovarajući ***ID*** računa u programu kako bi korisniku bilo lakše da tačnije utvrdi koji račun želi da stornira (npr. u slučaju da imaju dva sa istim brojem).
3. Klikom na dugme ***Storniraj*** se stornira odabrati račun i zatvara se forma

***Napomena: Biti veoma pažljiv sa odabirom računa koji se stornira jer je ova operacija nepovratna, tj. nije moguće vratiti stornirane podatke.***

### Prikaz artikala sa računa

Jako je bitno imati dobar pregled svih artikala sa jednog računa. Na primer, potrebno je iskontrolisati da li je broj unetih artikala u programu isti kao i na računu, da li su svi artikli sa računa uneti u program i slično. Ta opcija je omogućena u okviru programa na sledeći način:


  1. Klikom na dugme ***Pretraži račune*** se otvara nova forma
  2. U novootvorenoj formi se nalazi mnogštvo karakteristika računa i moguće je postaviti razne uslove kako bi se odredio račun koji je potrebno detaljnije ispitati
     * Ukoliko korisnik želi da odredi datum računa koji se nalazi između dva perioda (npr. za Datum računa želi da bude pre 1.1.2023. unosi tu vrednost u polje ***Datum računa do***, za pravilan rad programa ***neophodno*** je i da unese neku vrednost za ***Datum računa od***, npr. 1.1.2020.
     * Ukoliko korisnik želi da pregleda ***sve račune*** dovoljno je da ne menja vrednosti nijednog polja i samo klikne na dugme ***Pretraži***
  3. Klikom na dugme ***Pretraži*** se prikazuje tabela artikala računa koji zadovoljavaju zadate kriterijume.

Ukoliko se primete bilo kakve ***neregularnosti*** ili ***nelogičnosti*** prilikom pregleda računa, potrebno je reagovati na njih. Ukoliko je problem manje prirode (npr. greška u datumu) samostalno izmeniti podatke uz ***dosta*** opreza.


[Nazad na vrh](#magacin)


## Slobodna vozila

Klikom na dugme ***Slobodna vozila*** moguće je pogledati sva trenutno slobodna vozila.

## Stanje magacina

Klikom na dugme ***Stanje magacina*** moguće je pogledati sve artikle koji se trenutno nalaze u magacinu. Ovo može biti veoma veliki rezultat u slučaju da magacin naraste tako da se moli korisnik programa da konstruktivnim ***savetima*** kontaktira podršku kako bi se razvile dodatne mogućnosti i opcije ovog dela programa.

[Nazad na vrh](#magacin)
