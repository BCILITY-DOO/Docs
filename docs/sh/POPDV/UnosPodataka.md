# Unos podataka u POPDV obrazac

## **1. Podešavanje**

Podešavanje za unos odgovarajućih vrednosti u **POPDV obrazac** vrši se putem stranice **Mapiranja izveštaja o PDV-u u RS**, gde se otvaraju kartice za **POPDV pozicije**, svaka za jedno od mogućih polja za unos. 

Svaka pozicija se povezuje sa odgovarajućom kombinacijom **VAT Business** i **VAT Product grupa**, na osnovu kojih se unosi tačna vrednost u odgovarajuće polje samog izveštaja.

![popdv](../assets/POPDV/popdv1.png)

### **1.1 Kartica Mapiranja izveštaja o PDV-u u RS**

Na kartici, u delu **General**, potrebno je uneti **kod** koji služi za prepoznavanje mapping podataka u okviru **VAT Posting Setup**-a, kao i **opis** podatka koji će se prikazati u obrascu.

U zavisnosti od toga da li se podatak koji se unosi u **POPDV obrazac** odnosi na **nabavku** ili **prodaju**, kartica je podeljena na sekcije **Purchase** i **Sales**.

![popdv](../assets/POPDV/popdv2.png)

U polja koja se nalaze u delovima *Purchase i Sales* bira se polje u kom će se podatak pojaviti u POPDV obrascu.

![popdv](../assets/POPDV/popdv3.png)

### **1.2 Purchase Fast Tab**

U **Purchase** fast tab-u unosi se podatak u koje polje za datu poziciju treba da se unese podatak o osnovici ili iznosu PDV-a u obrascu POPDV.  

![popdv](../assets/POPDV/popdv4.png)

- **Purchase Payment Base** – Osnovica PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjiženog izvoda (**VAT Entry Base** za **Doc. Type: Payment**).

- **Purchase Payment Amount** – Iznos PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjiženog izvoda (**VAT Entry Amount** za **Doc. Type: Payment**).

- **Purchase Invoice Base** – Osnovica PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjižene fakture (**VAT Entry Base** za **Doc. Type: Invoice**).

- **Purchase Invoice Amount** – Iznos PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjižene fakture (**VAT Entry Amount** za **Doc. Type: Invoice**).

- **Purchase Cr. Memo Base** – Osnovica PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjiženog knjižnog odobrenja (**VAT Entry Base** za **Doc. Type: Cr. Memo**).

- **Purchase Cr. Memo Amount** – Iznos PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjiženog knjižnog odobrenja (**VAT Entry Amount** za **Doc. Type: Cr. Memo**).

- **Non-Deductable Base** – Osnovica PDV-a bez prava na prethodni odbitak se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjižene fakture.

- **Non-Deductable Amount** – Iznos PDV-a bez prava na prethodni odbitak se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjižene fakture.

- **Deductable Amount** – Iznos PDV-a sa pravom na prethodni odbitak se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjižene fakture (evidentira se **samo** kada postoji mapping za **Non-Deductable VAT Amount**).

### **1.3 Sales Fast Tab**

U **Sales** fast tab-u unosi se podatak u koje polje za datu karticu treba da se unese podatak o osnovici ili iznosu PDV-a u obrascu POPDV. 

![popdv](../assets/POPDV/popdv5.png)

- **Sales Payment Base** – Osnovica PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjiženog izvoda (**VAT Entry Base** za **Doc. Type: Payment**).

- **Sales Payment Amount** – Iznos PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjiženog izvoda (**VAT Entry Amount** za **Doc. Type: Payment**).

- **Sales Invoice Base** – Osnovica PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjižene fakture (**VAT Entry Base** za **Doc. Type: Invoice**).

- **Sales Invoice Amount** – Iznos PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjižene fakture (**VAT Entry Amount** za **Doc. Type: Invoice**).

- **Sales Cr. Memo Base** – Osnovica PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjiženog knjižnog odobrenja (**VAT Entry Base** za **Doc. Type: Cr. Memo**).

- **Sales Cr. Memo Amount** – Iznos PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjiženog knjižnog odobrenja (**VAT Entry Amount** za **Doc. Type: Cr. Memo**).

- **VAT Base Full VAT** – Iznos osnovice za evidentiranje promene samo na konta PDV-a, na osnovu proknjiženog opšteg naloga po tipu **Invoice**.

### **1.4 Books of incoming or outgoing invoices**

U zavisnosti od toga da li je data mapirana šifra prepoznata na osnovu nabavke ili prodaje, iznosi zabeleženi promenom na koju se ona odnosi se beleže i u ***knjigama izlaznih ili ulaznih računa***.

*Purchase / Book of Incoming Invoices*

![popdv](../assets/POPDV/popdv6.png)

*Sales / Book of Outgoing Invoices*

![popdv](../assets/POPDV/popdv7.png)

*Mapiranje knjige ulaznih i izlaznih računa* vrši se na osnovu numeracije polja na samom izveštaju.

![popdv](../assets/POPDV/popdv8.png)

![popdv](../assets/POPDV/popdv9.png)