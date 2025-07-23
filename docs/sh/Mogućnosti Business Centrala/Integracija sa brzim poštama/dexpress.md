# DExpress Integracija

**DExpress integracija** omogućava automatizaciju slanja pošiljki preko DExpress službe direktno kroz Business Central. Ova integracija pojednostavljuje proces dostave, eliminiše potrebu za ručnim unosom podataka i smanjuje mogućnost grešaka.

**Instalacija DExpress** sadrži osnovna podešavanja integracije, uključujući pristupne podatke, podrazumevane opcije isporuke i plaćanja, kao i informacije o poslednjim datumima sinhronizacije ključnih entiteta.

![img](../assets/DExpressImage/setup.png)

Detaljan opis polja sa slike dat je u tabeli ispod:

<div align="center">

<table border="1">
  <thead>
    <tr>
      <th colspan="2" align='centre'>Instalacija DExpress</th>
    </tr>
    <tr>
      <th align='centre'>Naziv Polja</th>
      <th align='centre'>Objašnjenje</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Omogućen</strong></td>
      <td>Prekidač za aktivaciju/deaktivaciju DExpress integracije.</td>
    </tr>
    <tr>
      <td><strong>Osnovna URL adresa</strong></td>
      <td>Pristupna tačka za DExpress servise.</td>
    </tr>
    <tr>
      <td><strong>API korisničko ime</strong></td>
      <td>Identifikator za autentifikaciju API-ja.</td>
    </tr>
    <tr>
      <td><strong>API lozinka</strong></td>
      <td>Sigurnosna lozinka za pristup API-ju.</td>
    </tr>
    <tr>
      <td><strong>ID klijenta</strong></td>
      <td>Dodeljuje ID klijenta u sistemu DExpress.</td>
    </tr>
    <tr>
      <td><strong>Agent</strong></td>
      <td>Određuje pružaoca kurirske usluge. <br>Postaviti vrednost na: <code>DEXPRESS</code>.</td>
    </tr>
    <tr>
      <td><strong>Podrazumevani tip isporuke</strong></td>
      <td>Određuje način isporuke.</td>
    </tr>
    <tr>
      <td><strong>Podrazumevano plaćanje</strong></td>
      <td>Određuje ko snosi troškove isporuke pošiljke.</td>
    </tr>
    <tr>
      <td><strong>Podrazumevano otkup</strong></td>
      <td>Određuje ko snositi troškove otkupa.</td>
    </tr>
    <tr>
      <td><strong>Podrazumevana povratna dokumentacija</strong></td>
      <td>Definiše način rukovanja povratnom dokumentacijom.</td>
    </tr>
    <tr>
      <td><strong>Podrazumevani tip plaćanja</strong></td>
      <td>Određuje način plaćanja.</td>
    </tr>
    <tr>
      <td><strong>Opštine</strong></td>
      <td>Poslednji datum sinhronizacije opština.</td>
    </tr>
    <tr>
      <td><strong>Ulice</strong></td>
      <td>Poslednji datum sinhronizacije ulica.</td>
    </tr>
    <tr>
      <td><strong>Gradovi</strong></td>
      <td>Poslednji datum sinhronizacije gradova.</td>
    </tr>
    <tr>
      <td><strong>Radnje</strong></td>
      <td>Poslednji datum sinhronizacije prodavnica.</td>
    </tr>
    <tr>
      <td><strong>Lokacije</strong></td>
      <td>Poslednji datum sinhronizacije lokacija.</td>
    </tr>
    <tr>
      <td><strong>Paketomati</strong></td>
      <td>Poslednji datum sinhronizacije paketomata.</td>
    </tr>
    <tr>
      <td><strong>Centri</strong></td>
      <td>Poslednji datum sinhronizacije centara.</td>
    </tr>
    <tr>
      <td><strong>Statusi</strong></td>
      <td>Poslednji datum sinhronizacije statusa.</td>
    </tr>
  </tbody>
</table>

</div>

## Kreiranje i obrada prodajnog naloga sa DExpress dostavom

Nakon podešavanja DExpress integracije, proces slanja pošiljki funkcioniše na sledeći način:  

### 1. Kreiranje prodajnog naloga  
- Otvorite **Prodajne porudžbine** i kreirajte novi dokument.  
- Unesite podatke o kupcu, uključujući adresu dostave i kontakt informacije.  
- Dodajte artikle koji se prodaju i količinu.

![img](../assets/DExpressImage/SalesOrder.png)

### 2. Izbor DExpress-a kao dostavne službe  
- U sekciji **Isporuka i Fakturisanje**, pronađite polje **Agent**.  
- Iz padajuće liste izaberite **DEXPRESS** kao kurirsku službu.  
  
![img](../assets/DExpressImage/Agent.png)
  
- Idite na akciju **Dodeli pakete** koja se nalazi u zaglavlju sekcije Redovi.
  
![img](../assets/DExpressImage/AssignPack.png)

Akcija **Dodeli pakete** omogućava korisnicima da raspodele porudžbinu u više paketa. 

Ova akcija funkcioniše tako što korisnik može za svaku stavku dodeliti odgovarajući broj paketa. Ovo omogućava raspodelu stavki u više paketa prema potrebama porudžbine. Stavke kojima je dodeljen isti broj u koloni **Broj paketa** biće isporučene u istom paketu.

![img](../assets/DExpressImage/pack.png)

### 3. Knjiženje prodajnog naloga  
Kada su svi podaci uneti, proknjižite dokument.  
Nakon knjiženja, kreira se dokument u **Proknjižene prodajne isporuke**, gde se mogu videti detalji o proknjiženoj pošiljci.  

![img](../assets/DExpressImage/PosShip.png)

U okviru proknjižene prodajne isporuke, u zaglavlju dokumenta, odlaskom na Radnje nalazi se akcija **Prikaži DExpress isporuke**.

Akcija Prikaži DExpress isporuke u okviru proknjiženog prodajnog naloga omogućava korisnicima da pregledaju detalje o pošiljci poslatoj putem DExpress kurirske službe. Ovaj dokument sadrži ključne informacije, uključujući identifikacione podatke pošiljke, primaoca i pošiljaoca, kao i vrednost pošiljke, iznos otkupnine, dimenzije i masu paketa.

**Odštampaj oznaku isporuke**

Akcija odštampaj oznaku isporuke kreira broj labela onoliko koliko ima paketa, i pruža mogućnost štampanja istih.

![img](../assets/DExpressImage/DEisporuke.png)

Ukoliko na Nalogu za prodaju nije odabrana kurirska služba, ovaj korak se može uraditi naknadno u Proknjiženom nalogu za prodaju koristeći akciju **Ažuriraj dokument**.

![img](../assets/DExpressImage/Ažuriranje.png)

U otvorenom prozoru je potrebno dodati DExpress u polju **Agent**.

![img](../assets/DExpressImage/AžurAgent.png)

Polje Agent na dokumentu će se automatski ažurirati.

![img](../assets/DExpressImage/Agent2.png)

Potom se artikli mogu podeliti u pakete odlaskom na akciju **Dodeli pakete**.

![img](../assets/DExpressImage/DodeliPakete.png)

Porudžbina se potom šalje DExpress kurirskoj službi klikom na akciju **Pošalji u DExpress** u zaglavlju.

![img](../assets/DExpressImage/Slanje.png)

### 4. Ručna isporuka za DExpress

Odlaskom na stranicu **Ručna isporuka za DExpress** moguće je ručno upravljanje pošiljkom. 

Ovaj dokument omogućava unos informacija o pošiljci, uključujući podatke o kupcu, detalje o preuzimanju i isporuci, kao i specifikacije same pošiljke. Sistem omogućava odabir tipa isporuke, načina plaćanja i vrednosti isporuke. 

![img](../assets/DExpressImage/Manual.png)

Ovaj interfejs omogućava efikasno praćenje i organizaciju pošiljki, kao i unos podataka o paketu klikom na akciju **Dodeli pakete**.

![img](../assets/DExpressImage/DodelaPak.png)

U otvorenom prozoru dodeljuje se broj paketu i unose se podaci o težini i dimenzijama paketa.

![img](../assets/DExpressImage/ManualPack.png)

Kada su svi podaci uneti, pošiljka se šalje klikom na akciju **Zakaži isporuku**.

![img](../assets/DExpressImage/ZakažiSlanje.png)

Poslata pošijka se može videti odlaskom na stranicu **DExpress isporuke**.
