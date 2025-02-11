# WooCommerce Integracija sa Business Central

## Uvod
Ova dokumentacija opisuje korake za integraciju WooCommerce prodavnice sa Microsoft Dynamics 365 Business Central, omogućavajući sinhronizaciju proizvoda, narudžbina i kupaca.

## Preduslovi
- **WooCommerce prodavnica** sa admin pristupom
- **Microsoft Dynamics 365 Business Central** nalog
- API ključevi za WooCommerce
- Business Central dodaci za integraciju (npr. „WooCommerce Connector“)

## 1. Kreiranje API ključeva u WooCommerce
1. Prijavite se u WordPress administraciju.
2. Idite na **WooCommerce > Settings > Advanced > REST API**.
3. Kliknite **Add Key**.
4. Unesite naziv (npr. „Business Central Sync“), odaberite korisnika i postavite **Permissions** na „Read/Write“.
5. Kliknite **Generate API Key** i sačuvajte **Consumer Key** i **Consumer Secret**.

## 2. Konfiguracija Business Central
1. Prijavite se u Business Central.
2. Idite na **Extension Management** i instalirajte „WooCommerce Connector“ ako već nije instaliran.
3. Otvorite **WooCommerce Connection Setup**.
4. Unesite sledeće podatke:
   - **Store URL**: URL vaše WooCommerce prodavnice
   - **Consumer Key**: Ključ koji ste generisali u WooCommerce
   - **Consumer Secret**: Tajni ključ generisan u WooCommerce
   - **API Version**: Preporučena verzija API-ja (npr. v3)
5. Sačuvajte i testirajte vezu.

## 3. Sinhronizacija podataka
### Sinhronizacija proizvoda
1. Idite na **WooCommerce Synchronization** u Business Central.
2. Kliknite **Sync Products**.
3. Business Central će povući sve proizvode iz WooCommerce-a i ažurirati ih.

### Sinhronizacija narudžbina
1. Idite na **WooCommerce Orders**.
2. Kliknite **Fetch Orders**.
3. Narudžbine će biti uvezene u Business Central radi obrade.

### Sinhronizacija kupaca
1. Idite na **WooCommerce Customers**.
2. Kliknite **Sync Customers**.
3. Business Central će sinhronizovati kupce iz WooCommerce baze.

## 4. Automatizacija
Možete koristiti **Job Queues** u Business Central za automatsku sinhronizaciju:
1. Idite na **Job Queue Entries**.
2. Kreirajte novi zadatak i povežite ga sa „WooCommerce Sync“.
3. Definišite interval sinhronizacije (npr. svaki sat).

## 5. Testiranje i rešavanje problema
- Proverite API dozvole ako dođe do greške pri povezivanju.
- Osigurajte da Business Central ima pristup internetu.
- Proverite logove u WooCommerce i Business Central za greške.

## Zaključak
Nakon uspešne konfiguracije, Business Central i WooCommerce će raditi zajedno na automatskoj razmeni podataka, poboljšavajući efikasnost upravljanja prodajom i zalihama.
