
# WooCommerce Setup

WooCommerce Setup omogućava povezivanje Business Central ERP sistema sa WooCommerce online prodavnicom, čime se automatski sinhronizuju podaci o proizvodima, kategorijama, zalihama i narudžbinama. Cilj podešavanja je da omogući nesmetan protok podataka između ova dva sistema, smanjujući potrebu za ručnim unosom i smanjujući rizik od grešaka.

Pre nego što započnete podešavanje WooCommerce integracije, potrebno je da imate: 

- Aktivno okruženje Business Central  
- WordPress sa instaliranim WooCommerce-om  
- API ključeve generisane u WooCommerce-u  
- Administratorski pristup oba sistema

## 1. Povezivanje Business Central-a i WooCommerce-a
- Korisnik unosi API kredencijale (**Consumer Key** & **Customer Secret**) koji omogućavaju sigurnu komunikaciju između Business Central-a i WooCommerce-a.  
- **Base URL** definiše na kojoj WooCommerce prodavnici će se izvršiti sinhronizacija.  

Ova konfiguracija omogućava povezivanje dva sistema, eliminiše potrebu za ručnim unosom podataka u obe platforme i smanjuje mogućnost grešaka.  

## 2. WordPress autentifikacija
- Unesite korisničko ime i lozinku administratora WordPress-a za pristup i ažuriranje podataka u WooCommerce-u.  

Ovaj korak obezbeđuje kontrolisan pristup podacima i sinhronizaciju bez potrebe za ručnim unosom.  

## 3. Podešavanja šablona (Template Settings)
- **Default Customer & Customer Template** – Definišu se pravila dodeljivanja kupaca za nove narudžbine.  
- **Item Template** – Određuje kako će se artikli prikazivati u WooCommerce prodavnici.  
- **Manufacturer Attribute** – Postavlja atribute proizvođača kako bi se proizvodima dodale dodatne informacije.  

Ova konfiguracija obezbeđuje standardizovano kreiranje proizvoda i olakšava upravljanje kupcima i zalihama.  

## 4. Upravljanje Woo ID-em i dodatne opcije
- **Allow Update Woo ID** – Kada je omogućeno, sistem može automatski ažurirati WooCommerce ID proizvoda kako bi se sprečili konflikti u bazi podataka.  

Ova opcija osigurava dosledno mapiranje podataka između dva sistema, sprečavajući greške u sinhronizaciji.

## 5. Automatska sinhronizacija podataka
- **Auto Sync Item** – Omogućava automatsko ažuriranje proizvoda između ERP-a i WooCommerce-a.  
- **Auto Sync Item Category** – Sinhronizuje kategorije proizvoda.  
- **Auto Sync Item Attribute** – Sinhronizuje dodatne atribute proizvoda, kao što su proizvođač, boja, dimenzije. 
- **Auto Sync Item Attribute Value** -  Sinhronizuje vrednosti atributa.

Obezbeđuje da su svi podaci o proizvodima i zalihama uvek ažurirani u WooCommerce prodavnici bez potrebe za ručnim unosom.  
  

## 6. Testiranje povezivanja
- **Connection Test Success** - Označava da li je veza bila uspešna, pružajući trenutne povratne informacije o statusu integracije.
- **Last Connection Test Time** - Pokazuje kada je poslednji put uspešno testirana veza između Business Central-a i WooCommerce-a.

Omogućava korisniku da samostalno proveri da li integracija funkcioniše i da brzo identifikuje eventualne probleme.
