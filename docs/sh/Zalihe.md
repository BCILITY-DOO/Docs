# **Modul zaliha**

Iako se zalihe uglavnom pokrivaju kroz module **Nabavka** i **Prodaja**, u ovom modulu ćemo se fokusirati na:  

- **Proveru zaliha** unutar sistema  
- **Prenos zaliha** između različitih lokacija  

## **1. Provera zaliha**

Proveru zaliha u sistemu moguće je izvršiti na nekoliko načina. U ovom uputstvu pokrićemo najčešće korišćene metode.  

Jedan od načina je pregled liste artikala, gde kolona **Zalihe** prikazuje ukupnu zalihu određenog artikla u sistemu.  

![zalihe](../assets/Zalihe/Zalihe1.png)

Kolona **Zalihe** predstavlja sumu svih stavki analitike artikla. Pored ukupne zalihe, putem analitike možemo pristupiti i dodatnim podacima kao što su:  

- **Rezervisana količina**  
- **Jedinični trošak**  
- **Preostala količina**  
- **Ostali relevantni podaci**  

Jedan od najlakših načina za pregled stavki analitike dostupne količine je otvaranje stranice sa filterom **Otvoreno = DA**. Ovaj filter prikazuje sve stavke koje su trenutno dostupne, ali treba imati na umu da iste stavke mogu biti rezervisane, zbog čega je važno pratiti i kolonu **Rezervisana količina**.  

![zalihe](../assets/Zalihe/Zalihe2.png)

Ako želite saznati koliko određenog artikla imate na pojedinim dokumentima, tu informaciju možete pronaći na **kartici artikla**, u brzoj kartici **Zalihe**.  

Za svako od prikazanih polja moguće je dobiti detaljan pregled količine tako što kliknete na broj.  

Na primer, ako želite videti količinu na redovima nabavne porudžbine, klikom na broj prikazaće se dokumenti na kojima se ta zaliha nalazi.  

![zalihe](../assets/Zalihe/Zalihe3.png)

Još jedan način za pregled trenutne zalihe je korišćenjem alatne trake:  
**Artikal → Raspoloživost artikla po** (sa liste ili kartice artikla).  

Ova opcija omogućava različite prikaze zalihe, uključujući:  

- **Raspoloživost zalihe** prema događaju  
- **Pregled po periodu**  
- **Razlikovanje po varijanti artikla**  
- **Raspored zalihe po lokaciji**  
- **Pregled po nivou sastavnice**  
- **Prikaz prema jedinici mere**  

Ovi prikazi omogućavaju detaljan uvid u stanje zaliha i njihovu dostupnost u različitim kontekstima.  

![zalihe](../assets/Zalihe/Zalihe4.png)

## **2. Prebacivanje zaliha na drugu lokaciju**

**Nalog za prenos**  

Za manipulaciju artiklima u skladištu koristi se dokument **Nalog za prenos**. Ovaj dokument služi za prebacivanje jednog ili više artikala sa jedne lokacije na drugu.  

**Direktni prenos**  

Ako se polje **Direktni prenos = DA** postavi, roba se direktno prebacuje bez tranzitnog perioda. U tom slučaju sistem automatski knjiži:  

- **Otpremnicu prenosa**  
- **Priznanicu prenosa**  

Ako je deo robe već otpremljen i primljen, polje **Direktni prenos** više nije moguće menjati.  

**Prenos sa tranzitom**  

Ako se koristi tranzit, proces se odvija u dva koraka:  

1. **Knjiženje otpremnice** – roba napušta skladište.  
2. **Knjiženje prijema** – kada roba stigne na odredišnu lokaciju, korisnik evidentira njen prijem.  

**Pronalaženje naloga za prenos**  

Listu svih kreiranih naloga za prenos koji još nisu obrađeni možete pronaći unosom **"nalozi za prenos"** u pretragu. Svaki korisnik vidi samo naloge koji se odnose na magacine za koje je zadužen.  

![zalihe](../assets/Zalihe/Zalihe5.png)

### **2.1 Kreiranje naloga za prenos**

Prilikom kreiranja **Naloga za prenos**, određena polja se automatski ili ručno popunjavaju:  

- **Polje Br.** – Popunjava se automatski prelaskom na bilo koje drugo polje. Sistem dodeljuje naredni slobodan broj iz definisane brojčane serije.  
- **Šifra izvora prenosa** – Lokacija (magacin) sa koje se artikli prenose.  
- **Šifra odredišta prenosa** – Lokacija (magacin) na koju se artikli prenose.  
- **Šifra u tranzitu** – Tranzitna lokacija na kojoj se artikli nalaze od trenutka isporuke sa izvorne lokacije do prijema na odredište.  
- **Datum knjiženja** – Datum pod kojim se kreira nalog za prenos.  

![zalihe](../assets/Zalihe/Zalihe6.png)

U okviru redova **Naloga za prenos** unose se podaci o artiklima koji se prenose:  

- **Br. artikla** – Izbor artikla koji se prenosi.  
- **Količina** – Unos ukupne količine za prenos.  
- **Količina za isporuku** – Automatski se popunjava na osnovu unete količine, ali može se ručno izmeniti ako je potrebno podeliti isporuku na više delova.  

**Definisanje datuma isporuke i prijema**  

- **Datum isporuke** – Planirani datum isporuke artikala.  
- **Datum prijema** – Planirani datum prijema na odredišnu lokaciju.  

Ove datume možete uneti direktno u redovima naloga ili u okviru brzih tabova **Prenos iz** i **Prenos u**.  

### **2.2 Knjiženje isporuke i prijema**

Kada ste popunili nalog za prenos relevantnim podacima, možete izvršiti evidentiranje istog u sistemu. U okviru komandne trake izaberite akciju *Proknjiži*, a potom *Isporuči*. 

![zalihe](../assets/Zalihe/Zalihe10.png)

![zalihe](../assets/Zalihe/Zalihe7.png)

Pokretanjem ove akcije, polje **Status** će dobiti vrednost **Izdato**, nakon čega polja na nalogu za prenos više neće biti moguće menjati.  

Takođe, primetićete da su se podaci u okviru redova naloga izmenili, kao što je prikazano na slici:  

![zalihe](../assets/Zalihe/Zalihe11.png)

Možemo primetiti da je planirana količina za isporuku u potpunosti realizovana, što znači da je potrebno izvršiti prijem iste količine.  

Da biste to uradili, ponovo izaberite akciju **Proknjiži** u okviru komandne trake, a zatim kliknite na **Primi**.  

> **Napomena:** Ako pokušate da izaberete opciju **Isporuči**, sistem će vas obavestiti da nema preostale količine za isporuku.  

![zalihe](../assets/Zalihe/Zalihe8.png)

Nakon što potvrdimo ovu akciju, pojaviće se sledeće obaveštenje:

![zalihe](../assets/Zalihe/Zalihe9.png)

Nakon što je **nalog za prenos** u potpunosti realizovan, on više neće biti prisutan na listi **otvorenih** i **izdatih naloga za prenos**.  

U slučaju da ste pogrešno evidentirali prenos sa jednog magacina na drugi, potrebno je da kreirate novi nalog za prenos u suprotnom smeru, sa istom količinom artikala (u našem primeru sa magacina na magacin, količina 15).  

Kada to uradite, možete otvoriti novi nalog za prenos sa ispravnim podacima.  

