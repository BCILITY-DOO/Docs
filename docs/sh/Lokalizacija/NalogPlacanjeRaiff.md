# Nalog za plaćanje Raiffeisen banka

## 1. Kreiranje naloga za plaćanje iz Business Central-a

Pretragom *Nalog plaćanja* otvaramo stranicu na kojoj unosimo podatke o uplatama.

![nalog](../assets/NalogPlacanja/nalog1.png)

Na samom vrhu stranice imamo polje *Ime grupe*, gde biramo *Grupu naloga knjiženja*:

![nalog](../assets/NalogPlacanja/nalog2.png)

Nakon odabira grupe, popunjavamo linije, gde je bitno popuniti polja: *Vrsta dokumenta*, *Vrsta konta*, *Br. konta*, *Šifra načina plaćanja i Iznos*, dok če polja *Vrsta i Broj protivkonta* biti automatski popunjena samim odabirom grupe naloga knjiženja.

Vrsta protivkonta je *Bankovni račun*, dok je broj protivkonta bankovni račun odabrane banke. U ovom slučaju je to *dinarski račun Raiffeisen banke*.

Ako prikažemo detalje ovog računa:

![nalog](../assets/NalogPlacanja/nalog5.png)

Otvara se *Kartica bankovnog računa*. U sekciji *Prenos*, imamo polje ***Format izvoza plaćanja***, gde biramo **RAIF**.

![nalog](../assets/NalogPlacanja/nalog6.png)

Nakon popunjavanja linija, na liniji akcija, u sekciji ***Banka*** imamo dve opcije:

- **Izvoz**
- **Izvezi jedan red**

Opcija **Izvoz** sve linije naloga plaćanja izvozi u XML formatu, dok opcija **Izvezi jedan red** izvozi samo selektovan red, takođe u XML formatu.

Prikaz XML fajla kada se izveze više linija:

![nalog](../assets/NalogPlacanja/nalog3.png)

Prikaz XML fajla kada se izveze jedna linija:

![nalog](../assets/NalogPlacanja/nalog4.png)


