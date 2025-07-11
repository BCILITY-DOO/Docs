# Avansi u prodaji (primljeni avansi)

## **1. Podešavanje**

Podešavanja važe za određivanje konta na kojima će biti evidentirane avansne uplate i PDV, koji se obračunava na osnovu datih avansnih uplata.

### **1.1 Grupe knjiženja kupaca**

Podešavanjem knjižnih grupa kupaca određuje se konto na koji će biti evidentirane sve avansne uplate primljene od kupca, što se definiše u koloni *Poslovni kontakt akontacije/avansne uplate*. Kada se određena knjižna grupa dodeli kartici kupca, sve poslovne promene tog kupca biće knjižene na kontima povezanim s tom grupom.

![avans](../../assets/AvansiProdaja/Avans1.png)

### **1.2 Opšte podešavanje knjiženja**

Da bi iznos na avansnom računu prikazivao samo PDV sadržan u avansnoj uplati prilikom knjiženja, potrebno je evidentirati konto za knjiženje PDV-a iz avansnog računa u polju *Konto akontacija/avansnih uplata u prodaji*. Ovaj konto će biti prikazan i na samom avansnom računu u sistemu.

![avans](../../assets/AvansiProdaja/Avans2.png)

## **2. Dokumenta**

### **2.1 Izvod**

#### **2.1.1 Promet uplata**

Pretragom *Nalozi plaćanja* pristupa se stranici na kojoj se evidentiraju izvodi. Ukoliko postoji više bankovnih računa, moguće je odvojiti grupe za knjiženje izvoda. Kada se knjiženje odnosi na bankovni račun, potrebno je promeniti tip balansiranja (Vrsta protivkonta) na *Bankovni račun* i odabrati odgovarajući bankovni račun na osnovu prethodno definisanih podešavanja.

![avans](../../assets/AvansiProdaja/Avans3.png)

Kako bi se uplata smatrala avansnom, prilikom knjiženja te uplate kroz dnevnik, neophodno je čekirati *Akontacija/avansna uplata* na liniji knjiženja.

![avans](../../assets/AvansiProdaja/Avans4.png)

Zatim upisati i iznos *(Iznos)* i to u negativnom obliku.

![avans](../../assets/AvansiProdaja/Avans5.png)

#### **2.1.2 Promet refundacija**

Dokument refundacije se automatski kreira u trenutku izdavanja konačnog računa za artikle iz porudžbine. Tom prilikom, sve avansne uplate se storniraju i prenose sa konta 4300 na konto kupaca.

### **2.2 Porudžbenica**

Dodeljivanje avansne uplate poručenim artiklima vrši se putem porudžbenice, što omogućava parcijalno isporučivanje i knjiženje prodaje na osnovu avansne uplate. Iznos avansa unosi se u polje *Akontacija/avansna uplata* na porudžbenici, na osnovu čega se može izdati avansni račun. Polje *Stavka aplikacije za zatvaranje u bankama* koristi se za unos iznosa sa izvoda koji je označen kao avansna uplata.

![avans](../../assets/AvansiProdaja/Avans6.png)

Nakon odabira uplate na koju se odnosi porudžbina, na osnovu celokupnog iznosa porudžbine, automatski se obračunava procenat koji pokazuje koji deo porudžbine je isplaćen datom avansnom uplatom.

![avans](../../assets/AvansiProdaja/Avans7.png)

Takođe, umesto fiksnog iznosa, može se uneti procenat avansne uplate, pri čemu će sistem automatski izračunati iznos na osnovu vrednosti artikala na koje se procenat primenjuje. Nakon unosa procenta, pojavljuje se dijalog sa upitom o ažuriranju vrednosti u kolonama za avans na porudžbenici, nakon čega se izračunava konačan iznos avansne uplate.

![avans](../../assets/AvansiProdaja/Avans8.png)

** **Ne može biti primenjen viši iznos avansne uplate od vrednosti konačne fakture – procenat avansne uplate ne može biti veći od 100%.**

### **2.3 Avansni račun**

#### **2.3.1 Avansna faktura**

Avansni račun se može kreirati i proknjižiti putem akcije *Knjiženje*. Iznos na avansnom računu odgovara PDV-u iz avansnih uplata koje su prethodno obrađene kroz polje *Akontacija/avansna uplata*, odnosno uplatu na koju se avansni račun odnosi.

![avans](../../assets/AvansiProdaja/Avans9.png)

#### **2.3.2 Avansno knjižno odobrenje**

Avansno knjižno odobrenje se automatski kreira prilikom izdavanja konačnog računa za artikle iz porudžbine i obuhvata sve prethodno izdate avansne račune. Iznos knjižnog odobrenja određuje se na osnovu PDV-a prikazanog na konačnom računu. Nakon knjiženja, iznos sa konta 4730 prenosi se na konto PDV-a.

![avans](../../assets/AvansiProdaja/Avans10.png)

Avansni račun je kreiran za uplatu od 20.000,00 dinara, pri čemu je iznos PDV-a na avansnom računu 3.333,33 dinara. Nakon izdavanja konačnog računa od 42.000,00 dinara sa PDV-om od 7.000,00 dinara, kreirano je knjižno odobrenje u istom iznosu. U ovom slučaju nemamo preostali iznos, odnosno iznos pretplate. U slučaju da je na kontu PDV-a ostalo npr. 750,00 dinara pretplate, pri sledećem fakturisanju, sistem bi automatski kreirao knjižno odobrenje na preostali iznos PDV-a iz avansne uplate.

#### **2.3.3 Konačni prodajni račun**

Konačni prodajni račun izdaje se za artikle koji se fakturišu kupcu za kupljenu robu. Na osnovu ovog računa automatski se kreira knjižno odobrenje i evidentira promet refundacije za postojeću avansnu uplatu.

![avans](../../assets/AvansiProdaja/Avans11.png)

## **3. Nalog knjiženja**

### **3.1 Izvod - knjiženje uplate**

![avans](../../assets/AvansiProdaja/Avans12.png)

### **3.2 Knjiženje avansne fakture**

![avans](../../assets/AvansiProdaja/Avans13.png)

### **3.3 Knjiženje konačne fakture**

![avans](../../assets/AvansiProdaja/Avans14.png)