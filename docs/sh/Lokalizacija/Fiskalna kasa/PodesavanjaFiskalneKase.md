# Podešavanja fiskalne kase

## **1. Podešavanje poreske fiskalizacije u RS**

Na stranici *Podešavanje poreske fiskalizacije u RS*, u sekciji *Opšta podešavanja*, neophodno je čekirati opciju ***Omogući fiskalnu verziju RS***.

Zatim u sekciji *Podešavanje kase* moraju sva polja biti popunjena. *Podrazumevani kupac*, *Podrazumevani prodavac* kao i *Podrazumevana jedinica prodajnog mesta* moraju imati vrednosti, da ne bi došlo do greške ukoliko korisnik zaboravi da izabere željenog kupca ili jedinicu prodajnog mesta.

![pos](../assets/POS/pos1.png)

### **1.1 POS jedinica**

Na stranici *Podešavanje poreske fiskalizacije u RS*, na liniji akcija nalazi se **POS jedinica**.

![pos](../assets/POS/pos2.png)

Pokretanjem akcije *POS jedinica*, otvaramo stranicu za podešavanje POS jedinice, gde je neophodno popuniti sledeća polja.

![pos](../assets/POS/pos3.png)

Kada su polja popunjena, pokrećemo akciju **Popunite KONFIGURACIJU SUF-a**, koja automatski popunjava polja na osnovu unetih podataka, a koja su neophodna za povezivanje sa *Poreskom Upravom*.

![pos](../assets/POS/pos4.png)

Zatim, pokrećemo akciju *Ažuriranje poreskih stopa* i *Popuni podatke BE kartice*, kako bi se popunili podaci o kompaniji. 

![pos](../assets/POS/pos5.png)

### **1.2 Mapiranje PDV-a**

Mapiranju PDV-a pristupamo takođe putem stranice *Podešavanje poreske fiskalizacije u RS*, na liniji akcija biramo **Mapiranje PDV-a**. 

Odabirom akcije otvaramo stranicu **Mapiranje podešavanja knjiženja za PDV u RS**, gde vidimo prikaz *Poslovnih grupa knjiženja po PDV-u* i *Grupa knjiženja proizvoda po PDV-u*. 

Kombinacije ovih grupa knjiženja sistem povlači iz *Podešavanja knjiženja PDV*, i ukoliko dodamo neku novu kombinaciju grupa u *Podešavanje knjiženja PDV*, moramo ih povući sa te stranice odabirom akcije *Inicijalizuj linije PDV postavki*, nakon čega će se na stranicu mapiranja one dodati.

![pos](../assets/POS/pos0.png)

Za svaku kombinaciju grupa možemo odabrati kategoriju poreza kroz polje **Naziv RS kategorije poreza**, gde će se odabirom kategorije automatski popuniti i polje *Oznaka RS poreza kategorije*.

![pos](../assets/POS/pos6.png)

Odabirom polja kategorije poreza, otvara se prozor gde možemo izabrati stopu PDV-a.

![pos](../assets/POS/pos7.png)

