

# DExpress Setup

DExpress integracija omogućava automatizaciju slanja pošiljki preko DExpress službe direktno kroz Business Central. Ova integracija pojednostavljuje proces dostave, eliminiše potrebu za ručnim unosom podataka i smanjuje mogućnost grešaka.


### Osnovna Konfiguracija
- **Omogućen**: Prekidač za aktivaciju/deaktivaciju DExpress integracije.
- **Osnovna URL adresa**: Pristupna tačka za DExpress servise.  
- **API korisničko ime**: Jedinstveni identifikator za autentifikaciju.
- **API lozinka**: Sigurnosni kredencijal za pristup API-ju.
- **Špediter**: Određuje pružaoca kurirske usluge.  
     Postaviti vrednost na: `DEXPRESS`

### Podrazumevana Podešavanja
- **Podrazumevani tip isporuke**: Određuje način isporuke.  
- **Podrazumevano plaćanje po**: Određuje ko snosi troškove dostave.  
- **Podrazumevano otkupljivanje za**: Označava primaoca pošiljke.  
- **Podrazumevani dokument za povraćaj**: Definiše način rukovanja povratnom dokumentacijom.  
- **Podrazumevani tip plaćanja**: Određuje način plaćanja.  

### Datumi Sinhronizacije

- **Opštine sa poslednjim datumom** – Poslednji datum sinhronizacije opština.
- **Ulice poslednjeg dadtuma** – Poslednji datum sinhronizacije ulica.
- **Gradovi poslednjeg datuma** – Poslednji datum sinhronizacije gradova.
- **Radnje sa poslednjim datumima** – Poslednji datum sinhronizacije prodavnica.
- **Lokacije poslednjeg datuma** – Poslednji datum sinhronizacije lokacija.
- **Poslednji dispenseri datuma** – Poslednji datum sinhronizacije dispenzera.
- **Centri za poslednje datume** – Poslednji datum sinhronizacije centara.
- **Statusi poslednjeg datuma** – Poslednji datum sinhronizacije statusa.
  
Odlaskom na "Akcije" u zaglavlju pruža se pristup svim podacima koji se nalaze u sistemu. Ovi podaci uključuju liste dostupnih gradova, ulica, prodavnica na koje se može vršiti isporuka.
     

## Kreiranje i obrada prodajnog naloga sa DExpress dostavom

Nakon podešavanja DExpress integracije, proces slanja pošiljki funkcioniše na sledeći način:  

### 1. Kreiranje prodajnog naloga  
- Otvorite **Sales Orders** i kreirajte novi prodajni nalog.  
- Unesite podatke o kupcu, uključujući adresu dostave i kontakt informacije.  
- Dodajte artikle koji se prodaju, uz količine i cene. 
-  Idite na opciju **Assign Packages**


### 2. Izbor DExpress-a kao dostavne službe  
- U sekciji **Shipping and Billing**, pronađite polje **Agent**.  
- Iz padajuće liste izaberite **DEXPRESS** kao kurirsku službu.  

Opcija **"Dodeli pakete"** na sales order-u omogućava korisnicima da raspodele stavke porudžbine u više paketa. Kada se klikne na ovu opciju, otvara se prozor sa sledećim kolonama:

- **Broj dokumenta**: Broj dokumenta koji identifikuje porudžbinu.
- **Broj reda.**: Broj linije unutar porudžbine, koji omogućava praćenje specifične stavke.
- **Broj stavke**: Broj proizvoda koji je deo porudžbine.
- **Opis**: Opis proizvoda.
- **Količina**: Količina proizvoda koja je deo porudžbine.
- **Neto težina**: Neto težina proizvoda.
- **Ukupna težina**: Ukupna težina svih proizvoda u toj liniji.
- **Širina [mm]**: Širina proizvoda u milimetrima.
- **Dužina [mm]**: Dužina proizvoda u milimetrima.
- **Visina [mm]**: Visina proizvoda u milimetrima.
- **Broj paketa**: Broj paketa kojem je dodeljena stavka.

**„Dodeli pakete“** funkcioniše tako što korisnik može za svaku stavku dodeliti odgovarajući broj paketa. Ovo omogućava raspodelu stavki u više paketa prema potrebama porudžbine. Stavke koje imaju isti broj biće isporučene u istom paketu.
     

### 3. Knjiženje prodajnog naloga  
Kada su svi podaci uneti, proknjižite dokument.  
Nakon knjiženja, kreira se **Posted Sales Shipment**, gde se mogu videti detalji o proknjiženoj pošiljci.  
Ovaj dokument sadrži sve informacije relevantne za isporuku putem DExpress-a. 

U okviru proknjiženog prodajnog naloga (Posted Sales Shipment), postoji opcija **DExpress isporuke**, koja omogućava pregled podataka o pošiljci kreiranoj putem DExpress integracije.
Opcija View DExpress Shipment u okviru proknjiženog prodajnog naloga omogućava korisnicima da pregledaju detalje o pošiljci poslatoj putem DExpress kurirske službe. Ovaj prikaz sadrži ključne informacije, uključujući identifikacione podatke pošiljke, primaoca i pošiljaoca, kao i vrednost pošiljke, iznos otkupnine (COD Amount) i masu paketa. Takođe, korisnici mogu videti podatke o dimenzijama paketa i koristiti opciju za štampanje nalepnice za isporuku pomoću opcije **Print Shipment Label Odštampaj oznaku isporuke**.

Ukoliko na Nalogu za prodaju nije odabrana kurirska služba, ovaj korak se može uraditi naknadno u Proknjiženom nalogu za prodaju koristeći opciju **"Pošalji u DExpress"**
  
### 4. Praćenje statusa isporuke  
- Nakon knjiženja, sistem može ažurirati status isporuke na osnovu podataka dobijenih od DExpress-a.  
- *Status pošiljke se može pratiti putem DExpress API-ja ili direktno iz Business Central-a.*  
