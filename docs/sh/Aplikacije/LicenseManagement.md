# License Management

**License Management** je dodatak za Dynamics 365 Business Central razvijen od strane kompanije **BCILITY**, koji omogućava kompanijama da na jednostavan i centralizovan način **upravljaju dostupnim licencama** u svom Business Central okruženju.

Aplikacija je namenjena administratorima sistema i IT odeljenjima, i služi za bolju kontrolu nad aktivnim korisnicima, dodeljenim licencama i tipovima pristupa – posebno u okruženjima sa većim brojem korisnika ili u okruženjima gde se često menja korisnička struktura.

**Ključne prednosti**

- Prikaz svih korisnika sa dodeljenim licencama i njihovim statusima
- Informacije o tipu licence (Full, Team Member, Device, External Accountant itd.)
- Brza identifikacija neaktivnih ili nepotrebno dodeljenih licenci
- Praćenje iskorišćenosti licenci u realnom vremenu
- Lakša komunikacija sa Microsoft partnerima i administratorima sistema

## **1. Kako se koristi?**

### **1.1 Licence**

![LicenseManagement](../assets/Aplikacije/LicenseManagement/licenmanag1.png)

Ova stranica prikazuje podatke o svim licencama i aplikacijama koje koriste naši klijenti, uključujući i određene informacije o njihovom okruženju.

Licence su kreirane tako da se **jedna licenca odnosi na jedno okruženje**. Nije potrebno ručno unositi ove podatke – aplikacija ih automatski popunjava kada klijent pokuša da validira svoju licencu.

Polja koja se najčešće ručno menjaju su *„Datum isticanja“* i *„Aktivna“*, jer upravo ona određuju da li je licenca aktivna.

Na desnoj strani stranice nalazi se **fact box** koji prikazuje detaljnije podatke iz svih kompanija unutar povezanog okruženja.

**Akcije na vrhu stranice** vode ka stranicama: *Podešavanja aplikacija (Extension Setup)*, *Mapiranje klijenta i tenanta (Customer Tenant Mapping)* i *Podešavanje za upravljanje licencama (License Management Setup)*.

### **1.2 Podešavanja aplikacija**

![LicenseManagement](../assets/Aplikacije/LicenseManagement/licenmanag2.png)

Stranica *„Podešavanja ekstenzija“* pruža informacije o licencama za dodate ekstenzije.
Ovaj deo možemo koristiti da podesimo trajanje besplatnog probnog perioda i definišemo u kojim okruženjima se ekstenzija može koristiti besplatno.

Nije potrebno da ručno unosimo sve podatke o licenciranju pre objavljivanja aplikacije – **Licensing Management aplikacija** će automatski popuniti ove informacije kada klijent pokuša da validira svoju licencu.

Podrazumevane vrednosti za polja kao što su „Da li je sandbox besplatan“, „Dužina besplatne probe“ i „Da li je aplikacija besplatna“  mogu se kasnije menjati na stranici *Podešavanja za upravljanje licencama*.

### **1.3 Mapiranje kupca i tenanta**

![LicenseManagement](../assets/Aplikacije/LicenseManagement/licenmanag3.png)

Ova stranica sadrži neophodne podatke o tenantima naših klijenata.

Jedino što je potrebno da uradimo jeste da označimo koji klijent koristi dati tenant tako što ćemo popuniti polje *Br.*.

#### **1.3.1 Spisak tenanta**

Ova stranica prikazuje podatke o tenantima koje koriste naši klijenti.

Baš kao i na prethodne dve stranice, ako nepoznat tenant pokuša da validira svoju licencu, podaci će se automatski popuniti na ovoj stranici.

Do ove stranice možemo doći klikom na ime tenanta na stranici *Licence*.

Akcije na vrhu stranice otvaraju stranice *Povezane licence*, *Povezana okruženja* i *Povezane kompanije*.

Stranice *Povezana okruženja* i *Povezane kompanije* prikazuju detaljnije podatke o našim klijentima.

![LicenseManagement](../assets/Aplikacije/LicenseManagement/licenmanag4.png)

### **1.4 Podešavanja upravljanjem licencama**

![LicenseManagement](../assets/Aplikacije/LicenseManagement/licenmanag5.png)

Na ovoj stranici možemo konfigurisati podrazumevane vrednosti licence koje se primenjuju kada se prvi put kreira licenca za aplikaciju.

#### **1.4.1 Da li je licenca aktivna?**

Glavno polje koje određuje da li je licenca aktivna jeste polje *Licenca važi do*. Ako je datum isteka prošao, licenca se smatra neaktivnom.

Ukoliko je polje za datum isteka prazno, licenca se smatra doživotnom, i tada polje *Da li je licenca aktivna* određuje da li je licenca aktivna.

***Postoje i određeni izuzeci:***

**Istekle licence** – Ako je datum isteka licence pre današnjeg datuma, licenca se smatra neaktivnom, čak i ako je polje *Da li je licenca aktivna* podešeno na *aktivno*. Ovaj status će biti ažuriran pri sledećem pokušaju validacije licence od strane korisnika.

**Besplatne aplikacije** – Ako je aplikacija označena kao besplatna u svom *Podešavanju ekstenzija*, licenca će se smatrati aktivnom čak i ako je datum isteka prošao ili je polje *Da li je licenca aktivna* podešeno na *neaktivno*. Status će se takođe ažurirati pri sledećem pokušaju validacije licence.