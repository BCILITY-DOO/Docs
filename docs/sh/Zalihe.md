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


