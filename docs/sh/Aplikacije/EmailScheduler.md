# Email Scheduler

**Email Scheduler** je dodatak za Dynamics 365 Business Central razvijen od strane kompanije **BCILITY**, koji omogućava automatsko slanje dokumenata putem e-pošte u unapred definisanim vremenskim intervalima. Umesto ručnog slanja faktura, otpremnica, ponuda ili drugih izveštaja, korisnici mogu podesiti raspored po kom će se dokumenti **automatski generisati i slati** direktno iz sistema.

Ovaj dodatak značajno unapređuje efikasnost komunikacije sa klijentima i partnerima, smanjuje potrebu za ručnim radom i obezbeđuje pravovremeno dostavljanje važnih poslovnih dokumenata. Idealno je rešenje za kompanije koje žele da automatizuju slanje faktura, podsetnika ili potvrda u skladu sa sopstvenim poslovnim pravilima.

---

## **1. Podešavanje planera e-pošte**

### **1.1 Aktivacija**

Neophodno je otvoriti stranicu **Podešavanje planera e-pošte**, na kojoj se klikom na opciju *Novo* kreira novi planer. Otvoriće se nova kartica planera e-pošte, gde je u sekciji **Opšte** obavezno uneti kod planera, dok je unos opisa opcioni.

U sekciji **Podešavanja e-pošte** definiše se predmet poruke i sadržaj koji se unosi u polje *Pregled HTML tela*. Nakon toga, određuju se **primaoci elektronske pošte**, pri čemu je potrebno izabrati tip primaoca (To, CC ili BCC), uneti e-mail adresu i, po potrebi, prikazano ime koje će biti prikazano u zaglavlju poruke.

Sekcija **Izveštaji** omogućava izbor jednog ili više izveštaja iz Business Centrala koji će biti priloženi uz e-poruku. Prilikom odabira *ID-a izveštaja*, automatski se popunjava naziv izveštaja. Zatim se definiše format izlaznog dokumenta – PDF, Word ili Excel, a po želji se može uneti i naziv fajla koji će biti prikazan u prilogu. Pored toga, dostupno je i polje za unos opisa primenjenih filtera.

![EmailScheduler](../assets/Aplikacije/EmailScheduler/schedule1.png)

Sledeća je sekcija **Podešavanje rasporeda**, u kojoj se određuje da li će se slanje e-pošte izvršiti jednokratno ili periodično. Ukoliko je potrebno da se e-poruka šalje više puta, aktivira se opcija *Ponavljajuće*, dok se za jednokratno slanje ova opcija isključuje. Kod jednokratnog slanja definišu se samo datum i vreme. Kada je slanje ponavljajuće, moguće je birati između dnevnog, nedeljnog ili mesečnog ritma, uz definisanje početnog i krajnjeg datuma, kao i tačnog vremena u toku dana. U slučaju nedeljnog rasporeda moguće je dodatno precizirati kojim danima u nedelji će slanje biti aktivno.

![EmailScheduler](../assets/Aplikacije/EmailScheduler/schedule2.png)

---

![EmailScheduler](../assets/Aplikacije/EmailScheduler/schedule3.png)

Na kraju se nalazi sekcija **Informacije o statusu**, u kojoj su prikazani datum i vreme narednog zakazanog slanja, podaci o poslednjem izvršenju, njegov status i eventualna poruka o grešci ukoliko do nje dođe tokom procesa.

![EmailScheduler](../assets/Aplikacije/EmailScheduler/schedule4.png)

Kada su sva neophodna polja podešena, e-pošta se aktivira označavanjem polja **Aktivno** u sekciji Opšte. Time se omogućava da definisani planer započne sa automatskim slanjem u skladu sa unetim rasporedom i parametrima.

---

### **1.2 Traka sa alatima**

Na kartici planera e-pošte na samom vrhu nalaze se akcije čije su funkcije objašnjene u nastavku.

![EmailScheduler](../assets/Aplikacije/EmailScheduler/schedule5.png)

---

**1. Pokreni odmah**

Ova opcija omogućava ručno pokretanje planirane e-pošte, bez obzira na podešeni raspored. Koristi se kada želite odmah da testirate ili pošaljete e-poštu definisanu u okviru planera, bez čekanja automatskog izvršenja.

**2. Prikaži dnevnik**

Otvara stranicu sa dnevnikom izvršavanja planera, gde možete pregledati sve prethodne pokušaje slanja e-pošte. Ova funkcija je korisna za praćenje uspešnih i neuspešnih izvršenja, kao i za analizu potencijalnih grešaka.

![EmailScheduler](../assets/Aplikacije/EmailScheduler/schedule6.png)

**3. Stavka redosleda poslova**

Ova akcija prikazuje povezanu stavku u redu poslova (Job Queue Entry) koja je zadužena za automatsko izvršavanje planera. Odatle je moguće dodatno pratiti ili menjati tehničke detalje vezane za raspored pokretanja.

![EmailScheduler](../assets/Aplikacije/EmailScheduler/schedule7.png)

**4. Proveri/kreiraj stavku redosleda poslova**

Omogućava automatsku proveru da li postoji validna stavka u redu poslova za ovaj planer e-pošte. Ukoliko nije pronađena, sistem će automatski kreirati novu stavku, čime se obezbeđuje da se e-pošta šalje prema definisanom rasporedu.

---

### **1.3 Primljena e-pošta**

Primer automatski poslate e-pošte:

![EmailScheduler](../assets/Aplikacije/EmailScheduler/schedule8.png)