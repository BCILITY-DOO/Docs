# Fakturisanje pretplata u Business Central-u

**Microsoft Subscription Billing** je funkcionalnost u okviru sistema Dynamics 365 Business Central koja omogućava efikasno upravljanje uslugama i proizvodima koji se naplaćuju periodično — na mesečnom, kvartalnom ili godišnjem nivou.

Ova funkcionalnost je idealna za kompanije koje posluju po pretplatnom modelu, jer pruža:

- automatsko kreiranje rasporeda fakturisanja,

- ponavljajuće fakture (bez potrebe da se svaki mesec unosi novi dokument),

- fleksibilne početke i završetke ugovora,

- napredno upravljanje cenama, popustima i uslovima plaćanja.

---

## **1. Pretplatni artikli**

Da bi se artikal definisao kao pretplatni, potrebno je izvršiti sledeća podešavanja na kartici artikla:

- U sekciji *Artikal*, u polju *Vrsta*, izabrati opciju **Bez zaliha**.

- U sekciji *Cene i prodaja*, obavezno popuniti polje **Jedinična cena**.

- U istom odeljku, u polju *Subscription Option*, izabrati opciju **Subscription Item**, čime se artikal označava kao predmet pretplatnog modela naplate.

![subs](../../assets/SubscriptionBilling/subscription1.png)

---

## 2. **Paket pretplate (Subscription Package)**

Nakon što popunimo sva neophodna polja na kartici artikla, u zaglavlju na traci akcija, u delu *Artikal*, možemo pronaći **Subscription package**.

![subs](../../assets/SubscriptionBilling/subscription2.png)

Na linijama *Item Subscription package-a* unosimo već postojeći paket, ili kreiramo novi. Ukoliko kreiramo novi paket neophodno je popuniti polje *Code*, dok je ključna stvar u linijama paketa.

Na linijama paketa unosimo podatke koji su neophodni da bi se znalo da li se radi o:

- *Kupcu* ili *Dobavljaču* (Partner), 
- način na koji se fakturiše pretplata (Invoicing via), da li preko *Prodajne/Nabavne porudžbine* ili preko **Pretplatnog ugovora**, 
- način računanja cene (Calculation Base Type), da li se računa na osnovu cene artikla ili celog dokumenta, 
- i najbitniji deo je period pretplate () i na koji period će se vršiti naplata (Billing Base Period, Billing Rhythm), kao i period trajanja pretplate (Initial term),
- imamo i opciona polja *Subsequent term* - na koliko će se pretplata automatski produžiti, kao i *Notice period* - označava koji period pre isteka ugovora će stići obaveštenje o isteku.

![subs](../../assets/SubscriptionBilling/subscription3.png)

---

## **3. Pretplate (Subscriptions)**

Kada otvorimo stranicu *Subscriptions*, odabirom opcije *Novo* započinjemo kreiranje nove pretplate. Na *kartici Subscription* potrebno je uneti vrednost u polje **Source No.**, gde se bira artikal kojem je prethodno dodeljen *Subscription package*. Nakon izbora artikla, sistem automatski popunjava linije pretplate parametrima koji su unapred definisani u okviru izabranog paketa.

Zatim je neophodno uneti podatke o krajnjem korisniku u sekciji *End User*. Dovoljno je uneti naziv kupca u polje **Customer Name** ili ga odabrati sa liste dostupnih klijenata.

![subs](../../assets/SubscriptionBilling/subscription4.png)

---

## **4. Ugovori o pretplati sa kupcima (Customer Subscription Contracts)**

U ovom koraku kreiramo ugovor sa kupcem na stranici *Customer Subscription Contracts*, odabirom opcije *Novo*.

Potrebno je uneti podatke u polje **Customer Name**, a zatim odabrati akciju **Get Subscription Lines** u vrhu stranice. Budući da smo prethodno u okviru *Subscriptions* već uneli krajnjeg korisnika, ovom akcijom se otvara kartica na kojoj će se, u linijama, prikazati prethodno kreirana pretplata. Nakon što odaberemo odgovarajuću pretplatu, pokrećemo akciju **Assign Selected Subscription Lines**, kojom se izabrana linija pretplate dodaje na linije ugovora.

![subs](../../assets/SubscriptionBilling/subscription5.png)

Nakon toga, kreiramo fakturu odabirom opcije **Create Contract Invoice**.

![subs](../../assets/SubscriptionBilling/subscription6.png)

Otvara nam se prozor gde možemo da odaberemo datum naplate, automatski je postavljen današnji datum. Pošto smo odredili da se pretplata naplaćuje na mesečnom nivou, na linijama će biti prikazani datum početka i kraja jednomesečne rate pretplate. Nakon toga možemo da proknjižimo ovu fakturu.

![subs](../../assets/SubscriptionBilling/subscription7.png)

---

## **5. Odlaganje prihoda (Customer Subscription Contract Deferrals)**

U Subscription Billing-u, *Deferrals* omogućavaju raspodelu unapred fakturisanog prihoda na više obračunskih perioda, u skladu sa trajanjem pretplate. Umesto da se ceo iznos prihoda prizna odmah, koristi se **Deferral Code** kojim se prihod knjiži postepeno – mesečno, kvartalno ili po drugom pravilu.

U **Subscription package** na linijama imamo jedno polje gde moćemo da naglasimo da li želimo odlaganje prihoda ili ne, i treća opcija je da odlaganje bude zavisno od ugovora.

![subs](../../assets/SubscriptionBilling/subscription8.png)

Kada odaberemo da bude zavisno od ugovora, na stanici **Customer Subscription Contract** imamo opciju da li želimo da aktiviramo odlaganje ili ne, odnosno da li želimo da iznos bude podeljen na period trajanja ugovora.

![subs](../../assets/SubscriptionBilling/subscription9.png)

Ukoliko aktiviramo ovu opciju, nakon što proknjižimo pretplatu, možemo da otvorimo stranicu **Customer Subscription Contract Deferrals** gde imamo pregled svih pretplata podeljenih na mesečne naknade, kao i to da li su realizovane ili ne.

![subs](../../assets/SubscriptionBilling/subscription10.png)

---

## **6. Proširenje ugovora (Extend Subscription Contract)**

Postojeći ugovor može biti proširen dodavanjem novih artikla, i to isključivo onih koji imaju *Subscription Package*. To je moguće uraditi korišćenjem opcije ***Extend Contract*** koja se nalazi na vrhu stranice ugovora. Otvoriće se prozor na kom ćemo u sekciji *Item* dodati artikal i količinu. 

![subs](../../assets/SubscriptionBilling/subscription11.png)

Potvrdom ove akcije, na linijama ugovora biće dodat novi pretplatni artikal.

![subs](../../assets/SubscriptionBilling/subscription12.png)