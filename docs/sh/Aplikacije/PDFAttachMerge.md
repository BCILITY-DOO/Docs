# PDF Attachment Merge

**PDF Attachment Merge** je dodatak za Dynamics 365 Business Central razvijen od strane kompanije **BCILITY**, koji omogućava korisnicima da **kombinuju više PDF dokumenata u jedan** i automatski ih prikače kao jedinstveni prilog uz zapis u sistemu.

Ova funkcionalnost je idealna za situacije kada se uz jedan nalog ili račun prilaže više dokumenata — na primer, faktura, otpremnica i sertifikat o kvalitetu — i kada je potrebno objediniti ih u jednu celinu radi lakšeg arhiviranja, deljenja ili štampanja.

**Ključne prednosti**

- **Spajanje više PDF fajlova u jedan dokument** direktno iz Business Central-a
- Automatsko kreiranje objedinjene datoteke kao **priloga** (Attachment)
- Podrška za dokumente koji su već priloženi uz zapis ili učitani iz lokalnog sistema
- Poboljšana preglednost i efikasnije upravljanje dokumentacijom
- Jednostavan interfejs, bez potrebe za dodatnim softverom

## **1. Kako se koristi?**

### **1.1 Instalacija objedinjavanja PDF priloga**

Pretragom *Instalacija objedinjavanja PDF priloga* otvaramo karticu na kojoj možemo podesiti funkcije i podrazumevane vrednosti. Postoje dve funkcije, to su *Izbriši datoteke posle objedinjavanja* i *Izbriši datoteke posle preuzimanja*, dok kod podrazumevanih vrednosti možemo da podesimo *Podrazumevano objedinjeno ime priloga* i *Podrazumevani naziv priloga dole*.

![PDFAttMerge](../assets/Aplikacije/PDFAttMerge/pdfatt1.png)

### **1.2 Objedini PDF i priloži**

Otvorićemo karticu *Kupci* i na desnoj strani otvorićemo deo gde se nalaze *Prilozi*. U samom odeljku *Prilozi* imamo sekciju *Dokumenti*, na koju kada kliknemo pojavi se padajući meni sa opcijom *Prikaži detalje*. Odabirom te opcije, otvoriće se prozor *Prikaćeni dokumenti*. Selektovaćemo dva PDF dokumenta po želji, i nakon selektovanja odabraćemo opciju **Objedini PDF i priloži**. Nakon toga će se otvoriti prozor gde bi trebalo da upišemo naziv novog dokumenta, međutim, u prvom koraku smo imali sekciju *podrazumevane vrednosti* gde smo podesili *podrazumevano ime priloga*, tako da ukoliko ne upišemo ime uzeće podrazumevanu vrednost.

![PDFAttMerge](../assets/Aplikacije/PDFAttMerge/pdfatt2.png)

![PDFAttMerge](../assets/Aplikacije/PDFAttMerge/pdfatt3.png)

### **1.3 Objedini PDF i preuzmi**

Sada ćemo na istoj kartici, za ista 2 selektovana dokumenta da pokrenemo akciju **Objedini PDF i preuzmi**. Pojaviće nam se prozor za unos imena datoteke, i kao u prethodnom primeru, ukoliko ne upišemo naziv, biće dodeljena podrazumevana vrednost.

![PDFAttMerge](../assets/Aplikacije/PDFAttMerge/pdfatt4.png)

### **1.4 Brisanje datoteka nakon objedinjavanja/preuzimanja**

Vratićemo se na karticu *Instalacija objedinjavanja PDF priloga*, gde ćemo aktivirati opciju **Izbriši datoteke posle objedinjavanja**.

![PDFAttMerge](../assets/Aplikacije/PDFAttMerge/pdfatt5.png)

Zatim otvaramo opet karticu *Kupci*, sekciju *Prilozi* i otvaramo listu priloga. Ponavljamo postupak selektovanja 2 PDF priloga i biramo opciju *Objedini PDF i priloži*. 

![PDFAttMerge](../assets/Aplikacije/PDFAttMerge/pdfatt6.png)

Možemo da primetimo da je kreiran novi prilog sa nazivom *Brisanje priloga*, dok su 2 PDF korišćena za objedinjavanje **obrisana**.

> Isti je postupak i za akciju **Objedini PDV i preuzmi**. Nakon preuzimanja, datoteke korišćene za objedinjavanje biće obrisane ukoliko je u podešavanjima aktivirana opcija **Izbriši datoteke posle preuzimanja**
