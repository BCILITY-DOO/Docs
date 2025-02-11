# DExpress Setup

DExpress integracija omogućava automatizaciju slanja pošiljki preko DExpress službe direktno kroz Business Central. Ova integracija pojednostavljuje proces dostave, eliminiše potrebu za ručnim unosom podataka i smanjuje mogućnost grešaka.


### Osnovna Konfiguracija
- **Enabled**: Prekidač za aktivaciju/deaktivaciju DExpress integracije.
- **Base URL**: Pristupna tačka za DExpress servise.  
- **API Username**: Jedinstveni identifikator za autentifikaciju.
- **API Password**: Sigurnosni kredencijal za pristup API-ju.
- **Shipping Agent**: Određuje pružaoca kurirske usluge.  
     Postaviti vrednost na: `DEXPRESS`

### Podrazumevana Podešavanja
- **Default Shipment Type**: Određuje način isporuke.  
- **Default Payment By**: Određuje ko snosi troškove dostave.  
- **Default Buy Out For**: Označava primaoca pošiljke.  
- **Default Return Document**: Definiše način rukovanja povratnom dokumentacijom.  
- **Default Payment Type**: Određuje način plaćanja.  

### Datumi Sinhronizacije

- **Last Date Municipalities** – Poslednji datum sinhronizacije opština.
- **Last Date Streets** – Poslednji datum sinhronizacije ulica.
- **Last Date Towns** – Poslednji datum sinhronizacije gradova.
- **Last Date Shops** – Poslednji datum sinhronizacije prodavnica.
- **Last Date Locations** – Poslednji datum sinhronizacije lokacija.
- **Last Date Dispensers** – Poslednji datum sinhronizacije dispenzera.
- **Last Date Centres** – Poslednji datum sinhronizacije centara.
- **Last Date Statuses** – Poslednji datum sinhronizacije statusa.
  
Odlaskom na "Akcije" u zaglavlju pruža se pristup svim podacima koji se nalaze u sistemu. Ovi podaci uključuju liste dostupnih gradova, ulica, prodavnica na koje se može vršiti isporuka.
     

## Kreiranje i obrada prodajnog naloga sa DExpress dostavom  

Nakon podešavanja DExpress integracije, proces slanja pošiljki funkcioniše na sledeći način:  

### 1. Kreiranje prodajnog naloga  
- Otvorite **Sales Orders** i kreirajte novi prodajni nalog.  
- Unesite podatke o kupcu, uključujući adresu dostave i kontakt informacije.  
- Dodajte artikle koji se prodaju, uz količine i cene.  

### 2. Izbor DExpress-a kao dostavne službe  
- U sekciji **Shipping and Billing**, pronađite polje **Agent**.  
- Iz padajuće liste izaberite **DEXPRESS** kao kurirsku službu.  
     

### 3. Knjiženje prodajnog naloga  
- Kada su svi podaci uneti, proknjižite dokument.  
- Nakon knjiženja, kreira se **Posted Sales Shipment**, gde možete videti detalje o proknjiženoj pošiljci.  
- Ovaj dokument sadrži sve informacije relevantne za isporuku putem DExpress-a.  

### 4. Praćenje statusa isporuke  
- Nakon knjiženja, sistem može ažurirati status isporuke na osnovu podataka dobijenih od DExpress-a.  
- *Status pošiljke se može pratiti putem DExpress API-ja ili direktno iz Business Central-a.*  
