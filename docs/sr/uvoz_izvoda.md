# Uvoz bankovnih izvoda

Kreirana dokumentacija se odnosi na unos dinarskog izvoda Halkbank banke i dinarskog i deviznog izvoda Raiffeisen banke.

## 1. **Halk banka**  

### 1.1 Kreiranje definicije za razmenu podataka

U pretrazi je potrebno pronaći **„Definicije za razmenu podataka“** i u zaglavlju izabrati **Novo**.

![novo](assets/halk/Picture2.png)

Kreiraće se dokument u kom je potrebno uneti osnovne podatke o računu:

- **Šifra**
- **Ime**
- **Vrsta datoteke** koja se uvozi
- **Vrsta računa**

Zatim popuniti sledeće podatke:

- **Codeunit za čitanje/pisanje**: `1200`
- **XML port za čitanje/pisanje**: `1220`
- **Codeunit za rukovanje eksternim podacima**: `1240`

![novo](assets/halk/Picture3.png)


### 1.2 Popunjavanje sekcija *Definicije redova* i *Definicije kolona*

Iz XML fajla koji se nalazi na dnu dokumenta potrebno je posmatrati čvorove i na osnovu njih definisati putanje i polja.

#### Definicije redova

| Polje              | Vrednost                     |
|--------------------|-----------------------------|
| **Vrsta reda**     | Detalj                       |
| **Šifra**         | HALK_LINES                   |
| **Ime**           | DEFAULT_LINES                |
| **Broj kolona**   | 3                             |
| **Oznaka reda podataka** | `/pmtnotification/trnlist/stmttrn` |

Nakon unetih podataka, sekcija **Definicije redova** treba da izgleda kao na sledećoj slici.

![def.red.](assets/halk/Picture4.png)

#### Definicije kolona

| Br. kolone | Ime            | Vrsta podataka | Opis       | Putanja |
|------------|---------------|---------------|-----------|---------|
| 1          | `/purpose`    | Tekst         | purpose   | `/pmtnotification/trnlist/stmttrn/purpose` |
| 2          | `/statusinfo/timeposted` | Datum | timeposted | `/pmtnotification/trnlist/stmttrn/statusinfo/timeposted` |
| 3          | `/trnamt`     | Decimal       | amount    | `/pmtnotification/trnlist/stmttrn/trnamt` |

Nakon unetih podataka, sekcija **Definicije kolona** treba da izgleda kao na sledećim slikama.

![def.kol.1](assets/halk/Picture5.png)

![def.kol.2](assets/halk/Picture6.png)


### 1.3 Mapiranje polja

Naredni korak je odlazak na opciju **„Mapiranje polja“**, koje se nalazi u zaglavlju sekcije *Definicije redova*.

![map.polja1](assets/halk/Picture7.png)

U otvorenom dokumentu potrebno je popuniti sledeća polja:

- **ID tabele**: `274`
- **Codeunit za mapiranje**: `1248`

![map.polja2](assets/halk/Picture8.png)

#### Definicija mapiranja

| Br. kolone | Naziv kolone | ID polja | Naziv polja         | Prioritet |
|------------|-------------|---------|--------------------|-----------|
| 1          | `/purpose`  | 6       | Opis               | 0         |
| 2          | `/statusinfo/timeposted` | 5 | Datum transakcije | 0         |
| 3          | `/trnamt`   | 7       | Iznos na izvodu    | 0         |

Nakon unetih podataka, sekcija **Mapiranje polja** treba da izgleda kao na sledećoj slici.

![map.polja3](assets/halk/Picture9.png)


### 1.4 Podešavanje bankovnog izvoza/uvoza

U pretrazi pronaći **„Podešavanje bankovnog izvoza/uvoza“** i otvoriti dati link.

U otvorenom prozoru kreirati novi zapis klikom na **Novo** i popuniti sledeće podatke:

- **Šifra**
- **Ime**
- **Pravac**
- **ID Codeunit-a za obradu** (automatski će se popuniti kolona **Ime Codeunit-a za obradu**)
- **ID XMLport-a za obradu** (automatski će se popuniti kolona **Ime XML port-a za obradu**)
- **Šifra definicije za razmenu podataka**   
  
Prikaz je na sledećoj slici:

![izvoz-uvoz](assets/halk/Picture10.png)

### 1.5 Povezivanje sa računom

U pretrazi pronaći **„Računi u banci“** i ući na račun **Halk Dinarski**.

Na kartici kreiranog računa, u delu **Prenos**, u polju **Format uvoza izvoda iz banke**, iz padajuće liste bira se: **HALK_DINARSKI**

![halk-din](assets/halk/Picture11.png)

### 1.6 Uvoz izvoda

U pretrazi pronaći **„Sravnjenje bankovnog računa“** i u sekciji **Banka** odabrati akciju **Uvoz izvoda iz banke**.

![halk-din-izvod](assets/halk/Picture12.png)

U otvoreni prozor prevući ili odabrati izvode koje treba dodati (fajl se nalazi na dnu dokumenta).

![halk-din-izvod2](assets/halk/Picture13.png)

### 1.7 Pregled transakcija

Sada su bankovni izvodi uneti, a ostvarene transakcije i njihovi detalji mogu se pregledati u sekciji **Redovi izvoda iz banke**, gde se mogu uporediti sa transakcijama knjiženim u sistemu.

![sravnjenje-bank-rac](assets/halk/Picture14.png)
---

### 1.8 XML šablon za dinarske izvode

[Otvorite XML šablon za **dinarske izvode** Halkbank banke](assets/halk/[338222@ibank][155-88160-49][22].xml)

## 2. **Raiffeisen banka**

### 2.1 Kreiranje definicije za razmenu podataka

U pretrazi je potrebno pronaći **„Definicije za razmenu podataka“** i u zaglavlju izabrati **Uvoz/Izvoz**, a potom opciju **Uvoz definicije za razmenu podataka**.

![def-razm-pod](assets/raiff/Picture15.png)

Kada se opcija odabere potrebno je izabrati fajl kojim će se kreirati šablon za uvoz podataka. Moguće je izabrati željeni fajl ili ga prevući u otvoreni prozor.

![def-razm-pod-1](assets/raiff/Picture16.png)

Kreiraće se dokument kao na sledećoj slici.

![def-razm-pod-2](assets/raiff/Picture17.png)

### 2.2 Definicije redova i kolona

U sekciji **Definicije redova** potrebno je kliknuti na red **Detalj** da bi se prikazali podaci u sekciji **Definicije kolona**.

U datoj sekciji potrebno je čekirati polje u koloni pod nazivom **„Importuj negativno“**, za red `/Stavke[@Duguje]`.

![def-red-kol](assets/raiff/Picture18.png)

---

## 2.3 Podešavanje bankovnog računa

Sledeći korak je u pretrazi pronaći **„Podešavanje bankovnog izvoza/uvoza“** i otići na dati link.

U otvorenom prozoru potrebno je kreirati novi zapis klikom na **Novo**, a potom popuniti sledeće podatke:

- **Šifra**
- **Ime**
- **Pravac**
- **ID Codeunit-a za obradu** (automatski će se popuniti kolona **Ime Codeunit-a za obradu**)
- **ID XMLport-a za obradu** (automatski će se popuniti kolona **Ime XML port-a za obradu**)
- **Šifra definicije za razmenu podataka**

![bank-racun](assets/raiff/Picture19.png)

Nakon toga je potrebno u pretrazi pronaći **„Računi u banci“** i kreirati novi račun klikom na opciju **Novo** u zaglavlju.

![podaci-racun](assets/raiff/Picture20.png)

Popuniti opšte podatke o računu.

![podaci-racun-1](assets/raiff/Picture21.png)

Na kartici računa, na delu **Prenos**, u polju **Format uvoza izvoda iz banke**, iz padajuće liste bira se kreirani šablon: **RAIF_RSD**.

![raif-rsd](assets/raiff/Picture22.png)

---

## 2.4 Uvoz izvoda

Naredni korak je pronaći **„Sravnjenje bankovnog računa“**, ući na račun **Raiffeisen Dinarski** i u sekciji **Banka** odabrati akciju **Uvoz izvoda iz banke**.

![sravnjenje-bank-rac](assets/raiff/Picture23.png)

U otvoreni prozor potrebno je prevući ili odabrati izvode koje treba dodati.

![datot-uvoz](assets/raiff/Picture24.png)

Sada su bankovni izvodi uneti, a ostvarene transakcije i njihovi detalji se mogu pregledati u sekciji **Redovi izvoda iz banke** i mogu se uporediti sa transakcijama koje su knjižene u sistemu.

![redovi-izvoda](assets/raiff/Picture25.png)
---

## 2.5 XML šabloni za dinarske i devizne izvode

- Sledeći objekat predstavlja **.xml fajl sa podacima za DEVIZNE izvode Raiffeisen Bank**, koji se ubacuje u **Definicije za razmenu podataka**.  
   
  [Otvorite XML šablon za **devizne izvode** Raiffeisen banke](assets/raiff/DEVIZNI Data Exch. Def. import template.xml)

- Sledeći objekat predstavlja **.xml fajl sa podacima za DINARSKE izvode Raiffeisen Bank**, koji se ubacuje u **Definicije za razmenu podataka**.  
  
  [Otvorite XML šablon za **dinarske izvode** Raiffeisen banke](assets/raiff/RSD Data Exch. Def. import template.xml)


