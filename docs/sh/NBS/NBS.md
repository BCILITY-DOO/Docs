# Integracija sa Narodnom Bankom Srbije

## 1. Kreiranje Kupca/Dobavljača putem PIB-a

Na kartici kupca u sekciji *Fakturisanje*, u polje **PIB** možemo uneti PIB kompanije. 

![nbs](../assets/NBS/nbs1.png)

Nakon što unesemo PIB, sistem će nas pitati da li želimo da ažuriramo podatke o kupcu, nakon potvrde prikazaće nam se svi podaci o tom kupcu čiji smo PIB uneli.

![nbs](../assets/NBS/nbs2.png)

Isti je postupak i za **Dobavljača**.

## 2. Ažuriranje kursne liste

Da bi se ažuriranje kursne liste izvršavalo automatski, podešavamo ga u *Pozadinskom izvršavanju zadataka*, što se u sistemu zove *Stavke reda čekanja za posao*.

![nbs](../assets/NBS/nbs3.png)

Kada otvorimo obeleženu karticu možemo da primetimo da se ova akcija pokreće automatski svakog dana u 8 ujutru. Takodje primećujemo da na vrhu kartice imamo akcije kojima i ručno možemo da pokrenemo ažuriranje, promenimo status ili stavimo na čekanje.

![nbs](../assets/NBS/nbs4.png)

## 3. Povlačenje kursne liste na dokumentima prilikom kreiranja INO dokumenta

Prilikom kreiranja INO dokumenta, kao što je na primer prodajna faktura za INO kupca, podrazumeva se da je valuta inostrana. 

Kada dodamo artikle koji su na prodaju, prikazana cena u lokalnoj valuti će biti po kursu tog dana.

![nbs](../assets/NBS/nbs5.png)

Međutim ukoliko promenimo **Datum knjiženja**, na datum kada je kurs bio drugačiji, automatski će se i iznos preračunati po kursu tog dana i dobićemo obaveštenje:

![nbs](../assets/NBS/nbs6.png)![nbs](../assets/NBS/nbs7.png)

Potvrdom o promeni kursa, promeniće se i iznos u lokalnoj valuti.

## 4. Kursevi valuta

Pretragom valuta otvaramo karticu *Valute*, na kojoj su prikazane sve strane valute u sistemu. 

![nbs](../assets/NBS/nbs8.png)

Klikom na kurs željene valute, otvaramo stranicu *Kursevi valuta*:

![nbs](../assets/NBS/nbs9.png)

Na stranici je prikazana kursna lista za valutu *Evro* i iznosi po datumima sve do današnjeg datuma, jer se kursna lista ažurira svakog dana po kursu *Narodne Banke Srbije*. Isti je princip za valutu *USD*.