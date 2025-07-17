# Mandatory Fields

**Mandatory Fields** je dodatak za Dynamics 365 Business Central razvijen od strane kompanije **BCILITY**, koji omogućava administratorima i supervizorima da definišu **obavezna polja (mandatory fields)** na ključnim stranicama sistema, u cilju osiguranja tačnog i potpunog unosa podataka.

Ova aplikacija pomaže organizacijama da standardizuju unos informacija, spreče nepotpune evidencije i minimizuju greške koje mogu uticati na dalje poslovne procese, kao što su fakturisanje, izveštavanje ili logistika.

**Ključne prednosti**

- Mogućnost označavanja **bilo kog polja kao obaveznog** na određenoj stranici
- Vizuelno označavanje obaveznih polja u korisničkom interfejsu
- Blokada zatvaranja dokumenta/zapisa dok se sva obavezna polja ne popune
- Fleksibilna konfiguracija prema tipu dokumenta, korisničkoj roli ili poslovnom procesu
- Nema potrebe za razvojem – sve se podešava direktno iz korisničkog interfejsa

## **1. Kako se koristi?**

### **1.1 Podešavanje obaveznih polja**

Pretražujemo karticu *Podešavanje obaveznih polja* na kojoj biramo opciju *Novo*. 

Na *kartici podešavanja obaveznih polja* u polje *ID stranice* unosimo broj koji predstavlja ID stranice na kojoj želimo da postavimo obavezna polja. Kada unesemo broj stranice, polje *ime stranice* biće popunjeno automatski. 

Da bismo omogućili obavezna polja, moramo da čekiramo polje *Omogućen*.

U sekciji redovi dodajemo *Br. polja* i *Ime polja* koja želimo da budu obavezna. To možemo učiniti klikom na 3 tačke (...) na praznom polju kolone *Br. polja*. Odabirom broja polja će *Ime polja* biti automatski popunjeno. 

![MandatoryFields](../assets/Aplikacije/MandatoryFields/mandfield1.png)

### **1.2 Primena (Kartica kupca)**

Na kartici kupca moćemo da primetimo da sva polja koja smo naznačili kao obavezna, a koja nisu popunjena imaju crveni okvir. Takođe, možemo da primetimo da na vrhu stranice imamo traku progresa koja pokazuje procenat koji pokazuje koji procenat obaveznih polja je popunjen, dok pored trake imamo *Tok obaveznih polja* koji pokazuje broj popunjenih obaveznih polja/broj obaveznih polja. Prelaskom miša preko ovih brojeva možemo videti i nazive obaveznih polja.

![MandatoryFields](../assets/Aplikacije/MandatoryFields/mandfield2.png)

Popunjavanjem nekog od praznih obaveznih polja menja se broj popunjenih obaveznih polja, kao i procenat na traci progresa.

![MandatoryFields](../assets/Aplikacije/MandatoryFields/mandfield3.png)