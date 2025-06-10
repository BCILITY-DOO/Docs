# Uvoz bankovnih izvoda

Kreirana dokumentacija se odnosi na unos dinarskog izvoda Halkbank banke i dinarskog i deviznog izvoda Raiffeisen banke.

## **1. Kreiranje definicije za razmenu podataka**

U pretrazi je potrebno pronaći **„Definicije za razmenu podataka“** i u zaglavlju izabrati **Uvoz/Izvoz**, zatim izabrati XML fajl koji želimo da uvezemo. U sklopu jednog XML fajla imamo neophodne podatke za Halk dinarski, Reiffeisen dinarski i devizni račun. 

![def.red.](../assets/halk/uvoz-izvoda.png)

Sledeći podaci će automatski biti popunjeni:

![novo](../assets/halk/Picture3.png)

### **1.1 Sekcije *Definicije redova* i *Definicije kolona***

Samim uvozom XML dokumenta, sekcije* Definicije redova* i *Definicije kolona* biće automatski popunjene.

![def.red.](../assets/halk/uvoz-izvoda1.png)

### **1.2 Mapiranje polja**

Opciju *Mapiranje polja* možemo pronaći u sekciji *Definicije redova*, međutim uvozom izvoda i mapiranje se izvršava automatski.

![def.red.](../assets/halk/uvoz-izvoda2.png)

Sekcija **Mapiranje polja** bi trebalo da izgleda kao na sledećoj slici.

![map.polja3](../assets/halk/Picture9.png)

### **1.3 Podešavanje bankovnog izvoza/uvoza**

U pretrazi pronaći **„Podešavanje bankovnog izvoza/uvoza“** i otvoriti dati link.

U otvorenom prozoru kreirati novi zapis klikom na **Novo** i popuniti sledeće podatke:

- **Šifra**
- **Ime**
- **Pravac**
- **ID Codeunit-a za obradu** (automatski će se popuniti kolona **Ime Codeunit-a za obradu**)
- **ID XMLport-a za obradu** (automatski će se popuniti kolona **Ime XML port-a za obradu**)
- **Šifra definicije za razmenu podataka**   
  
Prikaz je na sledećoj slici:

![izvoz-uvoz](../assets/halk/Picture10.png)

### **1.4 Povezivanje sa računom**

U pretrazi pronaći **„Računi u banci“** i ući na željeni račun.

Na kartici kreiranog računa, u delu **Prenos**, u polju **Format uvoza izvoda iz banke**, iz padajuće liste bira se račun željene banke.

![halk-din](../assets/halk/uvoz-izvoda3.png)

### **1.5 Uvoz izvoda**

U pretrazi pronaći **„Sravnjenja bankovnog računa“** i na kartici željenog računa u sekciji **Banka** odabrati akciju **Uvoz izvoda iz banke**.

![halk-din-izvod](../assets/halk/Picture12.png)

U otvoreni prozor prevući ili odabrati izvode koje treba dodati.

![halk-din-izvod2](../assets/halk/Picture13.png)

### **1.6 Pregled transakcija**

Sada su bankovni izvodi uneti, a ostvarene transakcije i njihovi detalji mogu se pregledati u sekciji **Redovi izvoda iz banke**, gde se mogu uporediti sa transakcijama knjiženim u sistemu.

![sravnjenje-bank-rac](../assets/halk/Picture14.png)
---

### **1.7 XML šablon za dinarske i devizne izvode**

[Preuzmi XML fajl](../assets/halk/Imp%20_%20Exp%20Data%20Exch%20Def%20%26%20Map.xml)


