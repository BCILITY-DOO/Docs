# **Dokumenta i nalog knjiženja**

## **1. Dokumenta**
Pretragom stranice *RS POPDV zapisi*, otvara se dijalog koji zahteva unos datuma od kog do kog sistem treba da generiše podatke koji su evidentirani u POPDV obrascu i knjigama ulaznih i izlaznih faktura.

![popdv](../assets/POPDV/popdv27.png)

Unosom početnog i završnog datuma, generisaće se samo promene koje su evidentirane u tom periodu, dok će, ukoliko se ne unese datum ni početka ni završetka, sistem generisati sve promene koje su evidentirane do datog trenutka.

### **1.1 POPDV obrazac**

Na osnovu ranije urađenog mapiranja, svi potrebni iznosi (PDV-a i osnovice) biće evidentirani na stranici.

![popdv](../assets/POPDV/popdv28.png)

Klikom na *Prikaži (...)* moguće je videti na osnovu kojih promena je dati iznos evidentiran, a polje *Pronadji stavke* otvara mogućnost utvrđivanja na koja konta je data promena evidentirana, kao i pregled drugih stavki.

![popdv](../assets/POPDV/popdv29.png)![popdv](../assets/POPDV/popdv30.png)

### **1.2 Knjige dolaznih i odlaznih faktura**

Kroz polje *Izveštaj* na stranici, otvara se mogućnost odabira pregleda knjig ulaznih i izlaznih računa, kao i štampanom dokumentu POPDV obrasca.

![popdv](../assets/POPDV/popdv31.png)

### **1.3 XML izveštaj**

XML izveštaj se eksportuje, pri čemu se kroz dijalog koji se javlja prilikom eksportovanja potvrđuje da li lice zahteva povrat prethodnog PDV-a, kao i informacije o podnosiocu PPPDV prijave. 

![popdv](../assets/POPDV/popdv32.png)![popdv](../assets/POPDV/popdv33.png)

Klikom na izabranu opciju, XML fajl se preuzima i moguće ga je uvesti na lokaciju *Poreske Uprave*.

![popdv](../assets/POPDV/popdv34.png)

## **2. Nalog knjiženja**

### **2.1 Evidencija nabavke**

Knjiženjem nabavne fakture, potrebni iznosi će biti automatski evidentirani u polja, u zavisnosti od toga kojoj poslovnoj knjižnoj grupi pripada dobavljač i kojoj knjižnoj grupi proizvoda pripada predmet fakturisanja.

![popdv](../assets/POPDV/popdv35.png)

![popdv](../assets/POPDV/popdv36.png)

Prikazane su knjižne grupe za datu porudžbinu, kao i podešavanje za knjiženje PDV-a.

Na osnovu datih podešavanja, uneti su iznosi u POPDV obrazac.

![popdv](../assets/POPDV/popdv37.png)

Polja suma se automatski popunjavaju.

### **2.2 Evidencija prodaje**

Knjiženjem prodajne fakture, potrebni iznosi će biti automatski evidentirani u polja, u zavisnosti od toga kojoj poslovnoj knjižnoj grupi pripada kupac i knjižnoj grupi proizvoda pripada predmet fakturisanja.

![popdv](../assets/POPDV/popdv38.png)

![popdv](../assets/POPDV/popdv39.png)

Prikazane su knjižne grupe za datu porudžbinu, kao i podešavanje za knjiženje PDV-a.

Na osnovu datih podešavanja, uneti su iznosi u POPDV obrazac.

![popdv](../assets/POPDV/popdv40.png)

### **2.3 Evidencija kroz opšti nalog**

Evidencija kroz opšti nalog moguća je kada jedan od konta koja se koriste za evidenciju imaju obeležene poslovne knjižne grupe za PDV kao i knjižne grupe proizvoda. Ovakva evidencija vrši se najčešće pri obračunu manjka, kada se evidentira samo trošak PDV-a koji je izazvan datim manjkom. 

Konto za evidentiranje PDV-a sadrži neophodne poslovne, kao i knjižne grupe proizvoda za PDV.

![popdv](../assets/POPDV/popdv41.png)

![popdv](../assets/POPDV/popdv42.png)

U ovom slučaju, knjiži se iznos PDV pri čemu će osnovicu sistem sam izračunati i evidentirati u neophodno polje.

![popdv](../assets/POPDV/popdv43.png)

### **2.4 Specifični slučajevi evidencije**

#### **2.4.1 Evidencija nabavke kada poreski obveznik – primalac dobara i usluga nema pravo na odbitak prethodnog poreza**

U slučaju kada primalac dobara ili usluga nema pravo na odbitak prethodnog PDV-a, knjiženje mora biti izvršeno na osnovu definisanih knjižnih grupa za dati slučaj – knjižne grupe proizvoda sa sufiksom ND.

![popdv](../assets/POPDV/popdv44.png)

![popdv](../assets/POPDV/popdv45.png)

#### **2.4.2 Evidencija u polja 3a POPDV obrasca**

Evidencija u polja 3a – promet drugog lica, iziskuje evidentiranje PDV-a i u ulaznim i u izlaznim računima, pa se kniženje vrši na sledeći način:
- Iznos osnovice po fakturi za ovu vrstu prometa potrebno je evidentirati u sekciji 8b (nabavka od domaćeg dobavljača) ili sekciji 8g (nabavka od inostranog dobavljača). PDV po ulaznim fakturama se evidentira u polju 8e.2., a PDV po izlaznim fakturama u sekciji 3a.
- Najpre će po računu biti evidentiran iznos osnovice u sekciji 8b (8g), a knjiženje PDV se obavlja kroz opšti nalog.

![popdv](../assets/POPDV/popdv46.png)

![popdv](../assets/POPDV/popdv47.png)

![popdv](../assets/POPDV/popdv48.png)

![popdv](../assets/POPDV/popdv49.png)

![popdv](../assets/POPDV/popdv50.png)

## **3. Štampa dokumenata**

### **3.1 POPDV obrazac**

Primer POPDV dokumenta za štampanje:

![popdv](../assets/POPDV/popdv51.png)

![popdv](../assets/POPDV/popdv52.png)

![popdv](../assets/POPDV/popdv53.png)

![popdv](../assets/POPDV/popdv54.png)

![popdv](../assets/POPDV/popdv55.png)

### **3.2 Knjiga ulaznih faktura**

![popdv](../assets/POPDV/popdv56.png)

### **3.3 Knjiga izlaznih faktura**

![popdv](../assets/POPDV/popdv57.png)

![popdv](../assets/POPDV/popdv58.png)
