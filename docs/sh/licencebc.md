# Dynamics 365 Business Central – Tipovi licenci

Dynamics 365 Business Central omogućava fleksibilno licenciranje u skladu sa različitim poslovnim potrebama. Pravilnim odabirom između Essentials, Premium, Device i Team Members licenci, kompanije mogu optimizovati troškove i efikasnost korišćenja sistema.

Ovaj dokument obuhvata četiri osnovna tipa licenci dostupnih u Dynamics 365 Business Central sistemu:

- Essentials
- Premium
- Device
- Team Members

---

## 1. Essentials i Premium

Dynamics 365 Business Central nudi dve glavne vrste licenci za korisnike sa punim pristupom: **Essentials** i **Premium**. Razlika između njih je u dostupnosti naprednih funkcionalnosti za proizvodnju i servis.

**Poređenje funkcionalnosti**

| Funkcionalnost                      | Essentials | Premium  |
|------------------------------------|------------|----------|
| Finansijsko upravljanje             | ✔          | ✔        |
| Upravljanje nabavkom i prodajom     | ✔          | ✔        |
| Upravljanje ljudskim resursima      | ✔          | ✔        |
| Upravljanje projektima              | ✔          | ✔        |
| Upravljanje skladištem              | ✔          | ✔        |
| Proizvodnja                         | Ograničeno | ✔        |
| Servis                              | ✘          | ✔        |

**Cene licenci (po korisniku mesečno)**

- Essentials: 70 USD
- Premium: 100 USD

> Svi korisnici sa punim pristupom u jednoj organizaciji moraju imati isti tip licence.

**Besplatan pristup za eksternog knjigovođu**

Dynamics 365 Business Central omogućava jednoj osobi u ulozi **eksternog knjigovođe** da pristupi sistemu besplatno, putem posebne licence.

**Uslovi:**

- Mora biti označen kao eksterni saradnik (External Accountant) u korisničkom profilu
- Ne sme biti zaposlen u firmi koja poseduje licencu
- Ima pun pristup sistemu, ali samo u svrhu knjigovodstva i obračuna

> Ova licenca se automatski aktivira kada je korisnik pravilno podešen kao eksterni knjigovođa i ne zahteva dodatnu kupovinu.

---

### **1.1 Essentials licenca**

Essentials licenca obuhvata sve osnovne funkcionalnosti potrebne za svakodnevno poslovanje:

- Vođenje glavne knjige
- Upravljanje klijentima i dobavljačima
- Prodaja i nabavka
- Upravljanje zalihama i skladištem
- Projekti i osnovna izveštavanja

Uključuje i osnovnu podršku za jednostavno sastavljanje proizvoda (sastavnice), pogodno za montažne procese bez kompleksnog planiranja resursa.

---

### **1.2 Premium licenca**

Premium licenca uključuje sve iz Essentials paketa, uz dodatne funkcionalnosti za:

**Proizvodnja**

- Strukture materijala sa više nivoa
- Operativne rute sa radnim i mašinskim centrima
- Detaljno planiranje kapaciteta i potreba za materijalom
- Praćenje vremena po operacijama (priprema, obrada, premestaj itd.)
- Analize i izveštaji za praćenje učinka proizvodnje

**Servis**

- Servisni nalozi i ugovori
- Upravljanje uređajima pod garancijom
- Planiranje servisera i rasporeda
- Automatsko fakturisanje servisnih aktivnosti
- Praćenje istorije servisiranja

---

### **1.3 Prelazak između licenci**

- **Sa Essentials na Premium**: jednostavno, jer se dodaju funkcije
- **Sa Premium na Essentials**: kompleksno i rizično, jer se funkcije uklanjaju

**Preporuka**

Ako firma prelazi sa Excela ili jednostavnog ERP-a, preporučuje se da se krene sa Essentials, a kasnije pređe na Premium kada se ustale osnovni procesi.

---

## **2. Licenca po uređaju (Device)**

Ova licenca omogućava više korisnika da koriste **jedan uređaj** (računar, terminal, skener itd.) bez potrebe da svaki ima svoju licencu.

**Gde se koristi**

- Maloprodajni objekti (prodajna mesta)
- Proizvodna hala (operateri mašina)
- Skladišta (prijem i otprema robe)

**Karakteristike**

- Licenca se dodeljuje uređaju, ne korisnicima
- Više korisnika koristi isti uređaj u različitim smenama
- Idealno rešenje za radna mesta gde se uređaji dele

**Dostupne funkcionalnosti**

- Kreiranje i izdavanje prodajnih dokumenata
- Ažuriranje zaliha
- Prikaz podataka o artiklima
- Zakazani zadaci preko sistema za raspoređivanje poslova

**Ograničenja**

- Korisnik sa ovom licencom ne može prvi da se prijavi u sistem
- Nema pristup celokupnoj funkcionalnosti kao korisnik sa punim pravima
- Računa se kao aktivan korisnik dok se izvršavaju njegovi zadaci

---

### **2.1 Podešavanje**

1. Administrator kreira bezbednosnu grupu u Microsoft 365 Admin centru pod nazivom:
   `Dynamics 365 Business Central Device Users`
2. Dodaju se korisnici koji koriste deljene uređaje
3. Licenca se dodeljuje po uređaju — korisnici ne moraju imati posebne licence

> Naziv grupe mora biti tačno ovako napisan, na engleskom jeziku, bez razmaka.

---

## **3. Licenca za članove tima (Team Members)**

Licenca za članove tima je predviđena za korisnike kojima je potreban **osnovni pristup** sistemu, bez mogućnosti obavljanja kompleksnih poslova.

**Idealna za korisnike koji:**

- Unose radne sate
- Ažuriraju lične podatke (HR)
- Pregledaju podatke, izveštaje i statuse
- Obavljaju pomoćne administrativne poslove

**Dostupne aplikacije**

Korisnici sa ovom licencom mogu koristiti aplikacije koje su prilagođene:

- Customer Service Team Member
- Sales Team Member
- Project Resource Hub

Ne mogu koristiti standardne aplikacije kao što su:
- Sales
- Customer Service
- Project Operations

Pokušaj pristupa takvim aplikacijama rezultira greškom o nedostatku prava pristupa.

---

**Ograničenja**

- Nema pristup prilagođenim aplikacijama
- Maksimalno 15 entiteta po aplikaciji (standardni ili prilagođeni)
- Dozvoljene su osnovne prilagodbe (terminologija, forme, prikazi)

> Sve promene i korišćenje moraju biti u skladu sa smernicama iz Microsoft licencnog vodiča.

---