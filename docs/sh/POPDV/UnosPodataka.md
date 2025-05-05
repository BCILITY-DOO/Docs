# Unos podataka u POPDV obrazac

## **1. Podešavanje**

Podešavanje za unos odgovarajućih vrednosti u **POPDV obrazac** vrši se putem stranice **Mapiranja izveštaja o PDV-u u RS**, gde se otvaraju kartice za **POPDV pozicije**, svaka za jedno od mogućih polja za unos. 

Svaka pozicija se povezuje sa odgovarajućom kombinacijom **Poslovne grupe knjiženja po PDV-u** i **Grupe knjiženja proizvoda za PDV**, na osnovu kojih se unosi tačna vrednost u odgovarajuće polje samog izveštaja.

![popdv](../assets/POPDV/popdv1.png)

### **1.1 Kartica Mapiranja izveštaja o PDV-u u RS**

Na kartici, u delu **Opšte**, potrebno je uneti **kod** koji služi za prepoznavanje mapping podataka u okviru **Podešavanja knjiženja za PDV**-a, kao i **opis** podatka koji će se prikazati u obrascu.

U zavisnosti od toga da li se podatak koji se unosi u **POPDV obrazac** odnosi na **nabavku** ili **prodaju**, kartica je podeljena na sekcije **Nabavka** i **Prodaja**.

![popdv](../assets/POPDV/popdv2.png)

U polja koja se nalaze u delovima *Nabavka i Prodaja* bira se polje u kom će se podatak pojaviti u POPDV obrascu.

![popdv](../assets/POPDV/popdv3.png)

### **1.2 Nabavka**

U **Nabavka** fast tab-u unosi se podatak u koje polje za datu poziciju treba da se unese podatak o osnovici ili iznosu PDV-a u obrascu POPDV.  

![popdv](../assets/POPDV/popdv4.png)

- **Baza plaćanja nabavke** – Osnovica PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjiženog izvoda (**Osnovica PDV-a** za **Tip dokumenta: Plaćanje**).

- **Iznos plaćanja u nabavci** – Iznos PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjiženog izvoda (**Iznos PDV-a** za **Tip dokumenta: Plaćanje**).

- **Baza ulazne fakture** – Osnovica PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjižene fakture (**Osnovica PDV-a** za **Tip dokumenta: Faktura**).

- **Iznos ulazne fakture** – Iznos PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjižene fakture (**Iznos PDV-a** za **Tip dokumenta: Faktura**).

- **Baza nabavnih odobrenja** – Osnovica PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjiženog knjižnog odobrenja (**Osnovica PDV-a** za **Tip dokumenta: Knjižno odobrenje**).

- **Iznos nabavnog odobrenja** – Iznos PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjiženog knjižnog odobrenja (**Iznos PDV-a** za **Tip dokumenta: Knjižno odobrenje**).

- **Baza neodbitnog PDV-a** – Osnovica PDV-a bez prava na prethodni odbitak se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjižene fakture.

- **Iznos neodbitnog PDV-a** – Iznos PDV-a bez prava na prethodni odbitak se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjižene fakture.

- **Iznos PDV-a sa pravom na odbitak** – Iznos PDV-a sa pravom na prethodni odbitak se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjižene fakture (evidentira se **samo** kada postoji mapping za **Iznos neodbitnog PDV-a**).

### **1.3 Prodaja**

U **Prodaja** fast tab-u unosi se podatak u koje polje za datu karticu treba da se unese podatak o osnovici ili iznosu PDV-a u obrascu POPDV. 

![popdv](../assets/POPDV/popdv5.png)

- **Baza prodajnih plaćanja** – Osnovica PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjiženog izvoda (**Osnovica PDV-a** za **Tip dokumenta: Plaćanje**).

- **Iznos prodajnih plaćanja** – Iznos PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjiženog izvoda (**Iznos PDV-a** za **Tip dokumenta: Plaćanje**).

- **Baza izlazne fakture** – Osnovica PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjižene fakture (**Osnovica PDV-a** za **Tip dokumenta: Faktura**).

- **Iznos izlazne fakture** – Iznos PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjižene fakture (**Iznos PDV-a** za **Tip dokumenta: Faktura**).

- **Baza prodajnih odobrenja** – Osnovica PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjiženog knjižnog odobrenja (**Osnovica PDV-a** za **Tip dokumenta: Knjižno odobrenje**).

- **Iznos prodajnog odobrenja** – Iznos PDV-a se upisuje u POPDV obrazac u odgovarajuće polje na osnovu proknjiženog knjižnog odobrenja (**Iznos PDV-a** za **Tip dokumenta: Knjižno odobrenje**).

- **Osnovica punog PDV-a za prodaju** – Iznos osnovice za evidentiranje promene samo na konta PDV-a, na osnovu proknjiženog opšteg naloga po tipu **Faktura**.

### **1.4 Knjiga dolaznih ili odlaznih faktura**

U zavisnosti od toga da li je data mapirana šifra prepoznata na osnovu nabavke ili prodaje, iznosi zabeleženi promenom na koju se ona odnosi se beleže i u ***knjigama dolaznih ili odlaznih faktura***.

*Nabavka / Knjiga dolaznih faktura*

![popdv](../assets/POPDV/popdv6.png)

*Prodaja / Knjiga odlaznih faktura*

![popdv](../assets/POPDV/popdv7.png)

*Mapiranje knjige ulaznih i izlaznih računa* vrši se na osnovu numeracije polja na samom izveštaju.

![popdv](../assets/POPDV/popdv8.png)

![popdv](../assets/POPDV/popdv9.png)

### **1.5 Podešavanje knjiženja za PDV**

Svaka šifra koja je kreirana preko kartice mora biti dodeljena odgovarajućoj kombinaciji *Poslovne grupe knjiženja po PDV-u* i *Grupe knjiženja proizvoda za PDV*

![popdv](../assets/POPDV/popdv10.png)

### **1.6 Podešavanje PDV-a**

Na stranici Podešavanje PDV-a potrebno je uključiti funkciju *Uključi PDV bez odbitka*.

![popdv](../assets/POPDV/popdv11.png)