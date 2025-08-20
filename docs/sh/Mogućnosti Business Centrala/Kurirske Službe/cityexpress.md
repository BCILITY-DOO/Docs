# City Express integracija

Ova dokumentacija opisuje proces integracije sistema sa kurirskom službom City Express u cilju automatizacije i optimizacije procesa isporuke pošiljki. Integracija omogućava korisnicima da direktno iz informacionog sistema kreiraju kurirske naloge i prate status pošiljki.

Implementacija ove integracije doprinosi uštedi vremena, smanjenju mogućnosti greške i unapređenju korisničkog iskustva kroz efikasnije upravljanje logistikom. Dokumentacija obuhvata tehničke zahteve, neophodna podešavanja, kao i primere razmene podataka između sistema i City Express platforme.

## **1. City Express podešavanja**

Na stranici podešavanja uočavamo sekciju ***Opšta***, gde se nalaze osnovna podešavanja, kao što je opcija *Uključeno*, čijim čekiranjem aktiviramo City Express integraciju. Zatim u polje *Kod agenta za isporučivanje* unosimo *CITYEXPRES*, i polje *Broj kopija liste preuzimanja* je u ovom slučaju podešen na 1, ali možemo menjati u zavisnosti od potreba.

U sekciji ***API parametri*** uočavamo 2 polja, u koja unosimo podatke koje dobijamo od City Express kurirske službe, a to su *API URL* i *API ključ*.

***Podrazumevane vrednosti isporuke*** je sekcija gde podešavamo podrazumevane vrednosti navedenih polja.

Na dnu stranice uočavamo sekciju ***Pošiljaoci*** gde u tabelu unosimo adrese lokacija sa kojih šaljemo pakete. Novu lokaciju unosimo tako što popunjavamo polja *Ime*, *Adresa*, *Poštanski kod*, *Grad*, *Broj telefona* i *E-mail(Opcionalno)*, dok se polje *City Express ID*, nakon popunjenih preostalih polja, automatski popunjava.

![img](../../assets/CityExpress/cityexpress1.png)

Na vrhu stranice se nalazi akcija *Preuzmite mapiranja poštanskih brojeva*, klikom na ovu akciju preuzimamo poštanske brojeve koji se nalaze u bazi City Express kurirske službe. Preuzete poštanske brojeve možemo pronaći pretraživanjem *Poštanski brojevi*. Ova akcija nam omogućava prikaz svih lokacija na koje ova kurirska služba vrši dostavu paketa, što umanjuje mogućnost za pravljenje grešaka.

![img](../../assets/CityExpress/cityexpress2.png)

Akcija *Radnje* -> *Načini plaćanja* nam otvara stranicu na kojoj možemo podesiti sve neophodne načine plaćanja.

![img](../../assets/CityExpress/cityexpress3.png)

Pri kreiranju *Prodajne porudžbine* kao način plaćanja možemo odabrati neki od navedenih načina plaćanja, s tim što je kolona *Plaćanje tokom isporuke* zapravo najbitnija za ovaj modul. U primeru na slici vidimo da je čekiran samo način plaćanja *POUZEĆEM*, što ukazuje na to da prilikom kreiranja prodajne porudžbine, odabirom načina plaćanja POUZEĆEM, automatski će se zahtevati otkup, dok kod ostalih načina plaćanja neće.

## **2. Kreiranje prodajne porudžbine**

Prilikom kreiranja prodajne porudžbine, neophodno je popuniti polje *Špediter*, što je u ovom slučaju *City Express*.

![img](../../assets/CityExpress/cityexpress4.png)

Takođe, neophodno je popuniti polje *Pošiljalac*, koje se odnosi na lokaciju sa koje se šalje paket. To su one lokacije koje smo dodavali u sekciji *Pošiljalac* na stranici *City Express podešavanja*.

![img](../../assets/CityExpress/cityexpress5.png)

Nakon što odaberemo lokaciju sa koje šaljemo paket, izaberemo špeditera i ostale neohodne podatke, porudžbinu možemo da proknjižimo.

## **3. City Express isporuke**

Na stranici City Express isporuke uočavamo sve porudžbine koje su povezane sa kurirskom službom City Express. Ukoliko otvorimo poslednju porudžbinu koju smo prethodno kreirali, možemo da vidimo sve podatke koje smo uneli prilikom kreiranja porudžbine, kao i podatke koji su povezani sa samim City Expressom, kao što su *Br. praćenja pošiljke* i *Status isporuke.*

![img](../../assets/CityExpress/cityexpress6.png)

Takođe, na vrhu stranice imamo nekoliko bitnih akcija. 

![img](../../assets/CityExpress/cityexpress7.png)

Akcija *Ažurirajte statuse isporuka* služi za ažuriranje statusa na samoj porudžbini, ukoliko se status u međuvremenu promenio.

Akcija *Odštampaj labele* štampa nalepnice koje se lepe na paket, sa svim informacijama o primaocu i adresi dostave, broju posiljke, itd.

![img](../../assets/CityExpress/cityexpress8.png)

Akcija *Zatraži preuzimanje* šalje zahtev za preuzimanje paketa i štampa **Listu preuzimanja**.

![img](../../assets/CityExpress/cityexpress9.png)

Klikom na akciju *Otkaži isporuku* otkazujemo isporuku.

**Na početku u podešavanjima smo podesili *Broj kopija liste preuzimanja* na 1 kopiju. To nas ograničava da akciju *Odštampaj labele*, kao i akciju *Zatraži preuzimanje* iskoristimo samo jednom. Međutim, ukoliko postoji potreba za ponovnim štampanjem labele ili liste preuzimanja, to možemo izvesti klikom na akciju *Radnje* -> *Ponovno štampanje labela* / *Ponovno štampanje liste preuzimanja*.

![img](../../assets/CityExpress/cityexpress10.png)