# Predikaatarvutus

## Sissejuhatus predikaatarvutusse

Predikaatarvutus on matemaatilise loogika haru, mis laiendab lausearvutust, võimaldades analüüsida lausete sisemist struktuuri ja kvantoritega väljendatud üldistusi. Kui lausearvutus käsitleb ainult terviklikke väiteid ja nendevahelisi loogilisi seoseid, siis predikaatarvutus võimaldab vaadelda ka objektide omadusi, objektidevahelisi seoseid ning üldistusi kõigi või mõnede objektide kohta.

Predikaatarvutust nimetatakse ka esimest järku predikaatloogikaks ning see on võimsam vahend matemaatiliste väidete formaliseerimiseks kui lausearvutus. Predikaatarvutus võimaldab formuleerida ja tõestada palju keerulisemaid väiteid, mis tavapärases matemaatikas on olulised.

## Predikaatarvutuse tähtsus

Predikaatarvutusel on oluline roll mitmes valdkonnas:

1. **Matemaatikas**: Predikaatarvutus võimaldab formaliseerida matemaatilisi teoreeme ja tõestusi täpsemalt kui lausearvutus. See on oluline matemaatika alustes, eriti hulgateooria ja aritmeetika formaliseerimisel.

2. **Arvutiteaduses**: Predikaatarvutus on aluseks mitmele programmeerimisparadigmale, eriti loogilisele programmeerimisele (nt Prolog). Samuti kasutatakse seda andmebaaside päringute formaliseerimisel ja tehisintellekti täpsema arutluse võimaldamisel.

3. **Filosoofias**: Predikaatarvutus võimaldab analüüsida filosoofilisi argumente ja arutlusi täpsemalt, eriti epistemoloogias ja metafüüsikas.

## Predikaatarvutuse seos lausearvutusega

Predikaatarvutus laiendab lausearvutust, lisades selle võimalustele juurde:

1. **Objektide käsitlemise** – arvestatakse maailma objektidega (indiviididega), mille hulga tähistame tavaliselt tähega D (domeeni või diskursuse universum).

2. **Predikaatide kasutamise** – predikaadid väljendavad objektide omadusi või seoseid objektide vahel.

3. **Kvantorite kasutamise** – kvantorid võimaldavad teha üldistusi "kõigi objektide" või "mõnede objektide" kohta.

Lausearvutust võib vaadelda kui predikaatarvutuse erijuhtu, kus ei kasutata predikaate ega kvantoreid.

## Selle sektsiooni alamteemad

Predikaatarvutuse sektsioon koosneb järgmistest alamteemadest:

1. **[Predikaadid ja muutujad](./2-1-predikaadid.md)** - predikaatide ja muutujate tähendus, termi mõiste, vabad ja seotud muutujad

2. **[Kvantorid](./2-2-kvantorid.md)** - üldisuskvantor (∀) ja olemasolu kvantor (∃), nende tähendus ja kasutamine, kvantorite järjekord

3. **[Predikaatvalemite eitamine](./2-3-eitamine.md)** - kvantoriga valemite eitamine, De Morgani seadused kvantoritele, mitmekordne eitamine

## Miks on predikaatarvutus oluline matemaatilises maailmapildis?

Predikaatarvutus on matemaatilise maailmapildi jaoks oluline mitmel põhjusel:

1. **Võimaldab täpset väljendust** - predikaatarvutus pakub formaalset keelt, milles saab täpselt väljendada keerulisi matemaatilisi ideid ja väiteid, vältides tavakeele mitmetähenduslikkust.

2. **Struktureerib loogilist mõtlemist** - predikaatarvutuse õppimine arendab võimet mõelda täpselt ja loogiliselt, mis on oluline oskus kõigis matemaatika ja informaatika valdkondades.

3. **Võimaldab täpsemat analüüsi** - predikaatarvutus võimaldab analüüsida väidete tõesust erinevate domeenide korral ja mõista paremini matemaatiliste struktuuride olemust.

4. **Ühendab erinevaid matemaatika valdkondi** - predikaatarvutus pakub ühtse keele, mille abil saab väljendada kõikide matemaatika harude põhimõtteid ja teoreeme.

## Predikaatarvutuse praktilised näited

Predikaatarvutus võimaldab formaliseerida mitmesuguseid igapäevaelulisi ja matemaatilisi väiteid. Vaatame mõningaid näiteid.

### Näide 1: Igapäevased väited

Tavakeelne väide: "Kõik õpilased õpivad vähemalt ühte õppeainet."

Predikaatarvutuse valem: ∀x(Õpilane(x) → ∃y(Õppeaine(y) ∧ Õpib(x,y)))

Kus:
- Õpilane(x) - predikaati, mis on tõene, kui x on õpilane
- Õppeaine(y) - predikaati, mis on tõene, kui y on õppeaine
- Õpib(x,y) - predikaati, mis on tõene, kui x õpib õppeainet y

### Näide 2: Matemaatilised väited

Tavakeelne väide: "Iga naturaalarvu korral leidub temast suurem naturaalarv."

Predikaatarvutuse valem: ∀x(Naturaalarv(x) → ∃y(Naturaalarv(y) ∧ y > x))

Või kui diskursuse universumiks on naturaalarvud, siis lihtsalt: ∀x ∃y (y > x)

### Näide 3: Matemaatilised definitsioonid

Algarvu definitsioon: "Naturaalarv p > 1 on algarv, kui tema ainsad naturaalarvulised jagajad on 1 ja p ise."

Predikaatarvutuse valem: Algarv(p) ⟺ (p > 1 ∧ ∀d(Naturaalarv(d) ∧ d|p → (d = 1 ∨ d = p)))

Kus d|p tähendab, et d jagab p-d.

## Predikaatarvutuse omandamise olulisus

Predikaatarvutuse mõistmine on oluline, sest see:

1. **Arendab abstraktset mõtlemist** - predikaatarvutus nõuab võimet käsitleda abstraktseid mõisteid ja seoseid, mis on oluline oskus kõrgema matemaatika jaoks.

2. **Parandab tõestamisoskusi** - predikaatarvutus pakub täpsed vahendid matemaatiliste väidete tõestamiseks ja ümberlükkamiseks.

3. **Valmistab ette edasisteks õpinguteks** - predikaatarvutus on aluseks paljudele keerukamatele matemaatika ja informaatika kontseptsioonidele.

4. **On oluline informaatikas** - predikaatarvutus on aluseks mitmesugustele arvutiteaduse valdkondadele, sealhulgas loogilisele programmeerimisele, tehisintellektile ja andmebaaside teooriale.

Järgmistes alamteemades käsitleme põhjalikumalt predikaatarvutuse erinevaid aspekte, alustades predikaatide ja muutujate mõistest ning liikudes edasi kvantorite ja eitamise juurde.