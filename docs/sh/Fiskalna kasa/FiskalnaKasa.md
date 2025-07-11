# Fiskalna kasa

## **1. Uputstvo za korišćenje kase**

Pretragom **POS (Kasa)** otvaramo stranicu kase. 

![pos](../assets/POS/pos8.png)

Na vrhu stranice nalaze se polja za odabir *Kase*, *Kupca* i *Prodavca*. Ova polja su automatski popunjena podrazumevanim vrednostima koje smo prethodno uneli kroz podešavanja, ali se mogu menjati u zavisnosti od potreba korisnika kase.

![pos](../assets/POS/pos9.png)

Polja *Tip kupca* i *Identifikacija kupca* se automatski popunjavaju na osnovu izabranog kupca.

![pos](../assets/POS/pos10.png)

Polja *Preostali iznos za plaćanje* i *Ukupan iznos* se automatski menjaju na osnovu dodatih proizvoda i njihovih vrednosti. 

![pos](../assets/POS/pos11.png)

### **1.1 Artikli**

U sekciji artikli možemo dodati artikle koje prodajemo, klikom na polje *Opis* otvara se padajući meni gde mozemo izabrati željeni artikal.

![pos](../assets/POS/pos12.png)

U polje *količina* upisujemo broj artikala koje prodajemo, kao i željenu *jedinicu mere*.

![pos](../assets/POS/pos13.png)

*Rabat* može biti upisan u odgovarajuće polje i odnosiće se na tu liniju artikla.

![pos](../assets/POS/pos14.png)

Ukoliko želimo da dodamo popust na ceo iznos, iznos popusta možemo u pisati u polje *% popusta* ili *Iznos popusta*. U zavisnosti koje polje popunimo, drugo polje će automatski biti popunjeno.

![pos](../assets/POS/pos15.png)

### **1.2 Linije plaćanja**

U sekciji *Linije plaćanja* imamo linije na kojima možemo da navedemo *tip plaćanja*, kao i iznos koji dodeljujemo tom tipu plaćanja. 

***- Primer:*** Ukoliko prodajemo artikal čija je vrednost 10000 dinara, na linije plaćanja kao tip dodajemo plaćanje čekom, i u polje iznos upisujemo iznos od 10000 dinara.

![pos](../assets/POS/pos16.png)

S obzirom da smo na linije plaćanja upisali ceo iznos, u delu *Preostali iznos za plaćanje* imamo nulu.

Da bismo potvrdili prodaju, na liniji akcija potvrdimo opciju *Prodaja*. ***Ova akcija se koristi samo u slučajevima kada ceo iznos imamo na linijama plaćanja.** 

![pos](../assets/POS/pos19.png)

Iznos plaćanja takođe možemo da podelimo na više tipova plaćanja, s tim što jedan tip plaćanja ne možemo koristiti više puta.

![pos](../assets/POS/pos20.png)

Ukoliko imamo situaciju da želimo da neki deo iznosa platimo jednim tipom plaćanja, a preostali iznos **kešom** ili **karticom**, na liniji akcija imamo akcije za plaćanje preostalog iznosa.

***- Primer:*** 

![pos](../assets/POS/pos17.png)

![pos](../assets/POS/pos18.png)

### **1.3 Povrat arikala**

Na linije artikala dodajemo artikal ili artikle za koje želimo da izvršimo povraćaj, a zatim izaberemo akciju *Povrat*. Takođe, možemo odabrati akciju *Povrat* iako nemamo dodat proizvod na liniju artikala, u tom slučaju će nam se otvoriti prozor sa izlistanim svim izdatim računima.

![pos](../assets/POS/pos21.png)

Odabirom akcije otvara se prozor

![pos](../assets/POS/pos22.png)

Pokretanjem akcije *Br. računa* (...), otvara se prozor gde možemo pronaći sve račune, ili sve račune na kojima se nalazi odabrani artikal.

![pos](../assets/POS/pos28.png)

Odabirom računa na kom je željeni artikal ištampaće se račun refundacije.

### **1.4 Linija akcija**

Na liniji akcija pored prodaje, plaćanja preostalog iznosa i povrata imamo opcije:

- Poništi transakciju - akcija koja briše sve linije artikala i sve linije plaćanja
- Obriši liniju - akcija koja briše selektovanu liniju artikla
- Obriši plaćanje - akcija koja briše selektovanu liniju plaćanja
  
#### **1.4.1 Promena cene**

Kada dodamo neki artikal, možemo da izvršimo promenu cene odabirom akcije *Promeni cenu*.

![pos](../assets/POS/pos23.png)

#### **1.4.2 Dnevni i periodični izveštaj**

Štampanje *Dnevnog fiskalnog izveštaja* vršimo odabirom akcije *Dnevni fiskalni izveštaj*

![pos](../assets/POS/pos24.png)

Pokretanjem ove akcije otvara se prozor gde moramo da izaberemo POS jedinicu, kao i da čekiramo da li je kraj dana. Ukoliko ovu opciju ostavimo odčekiranu, štampaće se samo presek stanja.

![pos](../assets/POS/pos25.png)

Štampanje *Periodičnog izveštaja* vršimo odabirom akcije *Periodični izveštaj*

![pos](../assets/POS/pos26.png)

Pokretanjem ove akcije otvara se prozor gde moramo da izaberemo *Datum početka*, *Datum završne obrade* kao i *POS jedinicu*.

![pos](../assets/POS/pos27.png)

Na liniji akcija -> Radnje, možemo pronaći *Istoriju računa* kao i sve *Dnevne i periodične izveštaje*.