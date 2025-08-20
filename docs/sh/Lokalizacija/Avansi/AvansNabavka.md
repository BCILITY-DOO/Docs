# Avansi u nabavci (dati avansi)

## **1. Podešavanje**

Podešavanja služe za definisanje konta na kojima će biti evidentirane avansne uplate, kao i konta za PDV koji se obračunava na osnovu tih uplata.

### **1.1 Nalozi plaćanja**

Knjiženje uplata i isplata obavlja se putem *Naloga plaćanja*, koji mora biti podešen tako da se transakcije knjiže na odgovarajući bankovni račun. Da bi promena na bankovnom računu bila ispravno evidentirana kao avansna uplata, potrebno je označiti opciju *Akontacija/avansna uplata* u *Nalozi plaćanja*.

![avans](../../assets/AvansiNabavka/avansnab1.png)

### **1.2 Grupe knjiženja dobavljača**

Podešavanjem knjižnih grupa dobavljača određuje se konto na koji će biti evidentirane sve avansne uplate namenjene tom dobavljaču, što se definiše u koloni *Poslovni kontakt akontacije/avansne uplate*. Kada se određena knjižna grupa dodeli kartici dobavljača, sve poslovne promene za tog dobavljača biće knjižene na kontima povezanim s tom grupom.

![avans](../../assets/AvansiNabavka/avansnab2.png)

### **1.3 Podešavanje knjiženja za PDV**

Na stranici VAT Posting Setup potrebno je definisati konto za evidentiranje PDV-a iz primljenih avansa u polju *Konto nabavnog PDV-a*, pri čemu njegov tip treba biti *Samo PDV*. Knjižne grupe povezane s ovim kontom moraju biti unete na karticu konta, uključujući konto za uplatu (15000) i konto za PDV (27200).

![avans](../../assets/AvansiNabavka/avansnab3.png)

![avans](../../assets/AvansiNabavka/avansnab4.png)

![avans](../../assets/AvansiNabavka/avansnab5.png)

## **2. Dokumenta**

### **2.1 Uplata avansa**

Uplata avansa dobavljaču evidentira se preko *Naloga plaćanja*, gde se bira dobavljač za kog se uplata odnosi i označava se kao avansna uplata, kako bi se evidentirala na odgovarajućem kontu.

![avans](../../assets/AvansiNabavka/avansnab1.png)

### **2.2 Avansni račun**

Nakon prijema avansnog računa, evidentiranje se vrši knjiženjem Purchase Invoice-a. Na liniji fakture unosi se broj konta 27200, na koji se evidentira PDV iz primljenih avansa. U zaglavlju računa potrebno je označiti da se radi o avansnom računu. Pri knjiženju, evidentira se isključivo iznos PDV-a iz avansne uplate.

![avans](../../assets/AvansiNabavka/avansnab51.png)

### **2.3 Avansno knjižno odobrenje**

Avansno odobrenje primljeno od dobavljača knjiži se putem dokumenta *Nabavno odobrenje*. Pri unosu je neophodno označiti da se radi o avansnom odobrenju tako što se u zaglavlju dokumenta čekira polje *Avans*.

![avans](../../assets/AvansiNabavka/avansnab6.png)

### **2.4 Konačni račun**

Nakon što primimo konačni račun, knjižimo ga po standardnoj proceduri.

### **2.5 Preknjižavanje konta**

U zavisnosti od razlike između iznosa na konačnoj fakturi i avansne uplate, potrebno je izvršiti preknjižavanje sa konta na kojem je evidentirana avansna uplata na konto dobavljača.  

Preknjižavanje se vrši putem *Naloga knjiženja*, pri čemu je važno da nalog bude pravilno popunjen kako bi ostao u ravnoteži. Strukturiranje naloga treba da odgovara pravilu knjiženja, uz tačno određena konta i iznose, kao što je prikazano na slici.

![avans](../../assets/AvansiNabavka/avansnab7.png)

## **3. Nalog knjiženja**

### **3.1 Evidencija avansne uplate**

Nalog knjiženja avansne uplate:

![avans](../../assets/AvansiNabavka/avansnab8.png)

### **3.2 Evidencija avansnog računa**

Nalog knjiženja avansnog računa:

![avans](../../assets/AvansiNabavka/avansnab9.png)

### **3.3 Avansno knjižno odobrenje**

Nalog knjiženja avansnog knjižnog odobrenja:

![avans](../../assets/AvansiNabavka/avansnab10.png)

