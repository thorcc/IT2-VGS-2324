# Oppgaver - Databehandling og algoritmer

- [1 - 12: Algoritmer, pseudokode og flytdiagram](#algoritmer-pseudokode-og-flytdiagram)
- [13 - 14: Databehandling](#databehandling)

## Algoritmer, pseudokode og flytdiagram

> Oppgavene skal besvares i en fil med navn `oppgaver-doa.md`

### Oppgave 1: V23-1


Hva er en while-løkke i programmering? (ett riktig svar)

- [ ] en løkke som kjører et bestemt antall ganger
- [ ] en løkke som kjører til en bestemt hendelse intreffer
- [ ] en løkke som kjører så lenge en bestemt betingelse er sann
- [ ] en løkke som kjører så lenge en tilfeldig betingelse er sann

### Oppgave 2: H23-2

Hvilken av de følgende påstandene er riktig om for- og while-løkker innen programmering? Velg riktig alternativ.

- [ ] en for-løkke kan bare brukes med tallsekvenser
- [ ] en while-løkke kjører alltid et bestemt antall ganger
- [ ] en for-løkke er best egnet når du vet hvor mange ganger du vil at løkken skal kjøre
- [ ] en while-løkke kan ikke bruke en teller for å holde rede på hvor mange ganger den har kjørt

### Oppgave 3: H23-3


Hva er hovedprinsippet bak objektorientert programmering (OOP)? Velg riktig alternativ.

- [ ] å lage lineære og sekvensielle programkoder
- [ ] å bryte ned et problem i et sett med funksjoner
- [ ] å representere data og funksjoner som objekter
- [ ] å minimere bruken av variabler



### Oppgave 4: H23-1

Hvilket av følgende er ikke et typisk kjennetegn på pseudokode? Velg riktig alternativ.

- [ ] den har uformell syntaks.
- [ ] den ligner på vanlig menneskespråk.
- [ ] den kan kjøres direkte på en datamaskin.
- [ ] den brukes ofte i planleggingsfasen av programmering.

### Oppgave 5: V23-2

Ta utgangspunkt i den følgende pseudokoden:

```
SET m TO 3
SET i TO 1
WHILE i GREATER THAN m
  DISPLAY "Lykkelig dag!"
  INCREMENT i
ENDWHILE
```
Hvor mange ganger blir teksten "Lykkelig dag!" skrevet ut?

- [ ] tre ganger
- [ ] to ganger
- [ ] én gang
- [ ] ingen ganger

### Oppgave 6: H23-4

Hvilke av de følgende sekvensene med pseudokode skriver ut tallene fra og med 1 til og med 5? Flere alternativer kan være riktige. Velg riktige svar.

```
1.
SET i TO 1
FOR hver i LESSER OR EQUAL 5
  PRINT i
ENDFOR

2.
SET i TO 1
WHILE i < 5
  PRINT i
  INCREMENT i 
ENDWHILE

3.
SET i TO 0
FOR hver i LESSER OR EQUAL 4
  PRINT i+1
ENDFOR

4.
SET i TO 1
WHILE i <= 5
  PRINT i
  INCREMENT i BY 2
ENDWHILE
```

- [ ] 1
- [ ] 2
- [ ] 3
- [ ] 4

### Oppgave 7: H23-5

Et system som beregner billettprisen avhengig av kjøperens alder, bruker følgende regler for billettkategorier:

- Hvis brukeren er 15 år gammel eller yngre, skal brukeren få barnebillett til 30 kroner.

- Hvis brukeren er 16 år gammel eller eldre, skal brukeren få voksenbillett til 50 kroner.

- Hvis brukeren er 67 år gammel eller eldre, skal brukeren få pensjonistbillett til 35 kroner.

Lag et flytdiagram for et program der brukeren skriver inn alderen på kjøperen og programmet regner ut og skriver ut riktig billettpris.

Lag flytdiagrammet i et egnet program, og lagre det i et allment lesbart format (f.eks. pdf eller png) og legg det ved i samme mappe som filen `oppgaver-doa.md`.

### Oppgave 8: V23-3

Tallene 1, 3, 6, 10, 15, 21 og så videre kalles for trekanttall. De tilsvarer antallet prikker som vil vises i en likesidet trekant når man bruker et grunnleggende trekantmønster for å bygge trekanten. Se illustrasjonen nedenfor: 

![](./bilder/v23-3.png)

Den følgende pseudokoden beskriver en funksjon som regner ut og returner trekanttallet nummer n:

```
FUNCTION trekanttall (n)
  SET tn TO n * (n+1)/2
  RETURN tn
ENDFUNCTION
```

Bruk funksjonen som er beskrevet ovenfor, og skriv pseudokoden til et program som regner sammen og skriver ut totalsummen av de ti første trekanttallene. Bruk dobbelt mellomrom for innrykk i koden der det er aktuelt. Skriv svaret ditt nedenfor.

> OBS: Du kan bruke din egen standard for pseudokode, bare den er hensiktsmessig.


### Oppgave 9: V23-4

I figuren nedenfor finner du en illustrasjon som viser et flytskjema for en algoritme, og i *kodeboksen* under figuren finner du fire sekvenser med pseudokode.

![](./bilder/v23-4.png)

```
1:
SET n TO 1
WHILE n LESSER THAN OR EQUAL TO 10
  INCREMENT n
  DISPLAY n
ENDWHILE

2:
SET n TO 0
FOR hver n LESSER THAN OR EQUAL TO 10
  DISPLAY n
ENDFOR

3:
SET n TO 1
WHILE n LESSER THAN 10
  DISPLAY n
  INCREMENT n
ENDWHILE

4:
SET n TO 1
FOR hver n LESSER THAN OR EQUAL TO 10
  DISPLAY n
ENDFOR
```

Hvilken sekvens med pseudokode gir lik visning av output som algoritmen beskrevet av flytskjemaet? Velg riktig svar:

- [ ] 1
- [ ] 2
- [ ] 3
- [ ] 4


### Oppgave 10: V23-5

Nedenfor finner du flere linjer med pseudokode. Sorter linjene i riktig rekkefølge, slik at det blir pseudokoden til et program som skal finne det største tallet av tre tall. Tips: Linjene med pseudokode har ikke innrykk/indentering.

![](./bilder/v23-5.png)

Eksempel på svar:
```
G-1
A-2
D-3
...
```

### Oppgave 11: H23-6

a) Du får i oppgave å finne det nest største tallet i en liste (array) med tall. Dersom det finnes flere like tall som er størst, skal ingen av disse regnes som nest størst. Under finner du fire alternative løsninger for denne oppgaven skrevet i pseudokode. Hvilke to løsninger er riktige?

```
1 	
SET størst TO negativt uendelig tall
FOR hvert tall i listen
  IF tall GREATER THAN størst
    SET størst TO tall
  ENDIF
ENDFOR
Fjern størst fra listen
SET nestStørst TO negativt uendelig tall
FOR hvert tall i listen
  IF tall GREATER THAN nestStørst 
    SET nestStørst TO tall
  ENDIF
ENDFOR
DISPLAY nestStørst

2 	
SET størst TO første tall i listen
SET nestStørst TO andre tall i listen
IF nestStørst GREATER THAN størst
  Bytt størst og nestStørst
ENDIF
FOR hvert tall i listen med start fra tredje tall
  IF tall GREATER THAN størst
    SET nestStørst TO størst
    SET størst TO tall
  ELSEIF tall GREATER THAN nestStørst AND tall NOT EQUAL TO størst
  SET nestStørst TO tall
  ENDIF
ENDFOR
DISPLAY nestStørst

3 	
SET størst TO negativt uendelig tall
SET nestStørst TO negativt uendelig tall
FOR hvert tall i listen
  IF tall GREATER THAN størst
    SET nestStørst TO størst
    SET størst TO tall
  ELSEIF tall GREATER THAN nestStørst
    SET nestStørst TO tall
  ENDIF
ENDFOR
DISPLAY nestStørst

4 	
Sorter listen i synkende rekkefølge
FOR hvert tall i listen
    IF tall NOT EQUAL TO neste tall i listen
        DISPLAY neste tall i listen
        avbryt for-løkken
    ENDIF
ENDFOR
```

Velg de to riktige løsningene.

- [ ] 1
- [ ] 2
- [ ] 3
- [ ] 4

b) Skriv en kort tekst der du vurderer og sammenligner de to løsningene du valgte i punkt a.

### Oppgave 12: H23-7

Elementene i en indeksert variabel (liste/array) skal sorteres i stigende rekkefølge etter følgende algoritme: Man sammenligner hvert element fra venstre til høyre i listen med neste element, og hvis elementet er større enn neste element, bytter de plass. Deretter går man videre til neste element og sammenligner på nytt frem til hele listen er gjennomgått. Dette gjentas til hele listen gjennomgås uten at det forekommer noen ombyttinger.

Under finner du deler av pseudokoden for denne algoritmen. Her er a en liste med n elementer, og a[ i ] er elementet på plass i i listen.

```
SET i TO 0
FOR hver i LESSER THAN n - 1
  IF a[i] GREATER THAN a[i+1]    
    CALL byttPlass()
  ENDIF
ENDFOR
```

> Presisering: byttPlass() er en funksjon som bytter plass på to naboelementer i listen.

a) Hva blir innholdet i listen etter at vi har kjørt programmet representert ved pseudokoden over for listen a = [8, 5, 2, 6, 12], som har n = 5 elementer?
Velg riktig svar.

- [ ] `[ 5, 8, 2, 6, 12 ]`
- [ ] `[ 5, 2, 8, 6, 12 ]`
- [ ] `[ 5, 2, 6, 8, 12 ]`
- [ ] `[ 2, 5, 6, 8, 12 ]`

b) Utvid pseudokoden slik at programmet den representerer, sorterer ferdig listen a i stigende rekkefølge etter altgoritmen som er vist øverst. Forklar endringene du gjør. Obs! Du må også lage pseudokode for funksjonen byttPlass(). 

c) Implementer pseudokoden fra punkt b i ditt programmeringsspråk. Listen skal leses inn automatisk, og den ferdig sorterte listen skal skrives til konsollet eller vises i programmet.

## Databehandling

> Oppgavene besvares i egne filer, én fil per oppgave.

### Oppgave 13: H23-11

#### YouTube-statistikk

Du skal lage et program som leser inn informasjon fra et datasett og presenterer den. Last ned datasettet her:

- [CSV/JSON](https://sokeresultat.udir.no/eksamenprovemateriell.html?kategori=rea3049&aar=2023-19&spraak=bokm%C3%A5l&trinn=annet&ferdighet=annet)

Tips: Du står fritt til å velge hvordan programmet skal presentere informasjonen, så lenge presentasjonen er godt egnet til å vise det oppgaven spør etter. Du kan også velge om du besvarer a og b i en samlet oversikt eller lager en oversikt for hvert oppgavepunkt.

Programmet du lager i denne oppgaven, skal inneholde en flerlinjet kommentar øverst som beskriver de vurderingene og valgene du har gjort for å vaske og forberede datasettet til bruk med programmet ditt.

a) Lag et program som finner og presenterer de ti landene i datasettet som har flest YouTube-kanaler.

b) Utvid programmet til å regne ut og presentere gjennomsnittlig antall abonnenter og videovisninger per kanal for hvert av disse landene.

### Oppgave 14: V23-9

#### Oversikt over apper i Google Play Store

Du skal lage et program som leser inn informasjon fra datasettet og presenterer dette i to oversikter.
Last ned datasettet her:

- [CSV](https://sokeresultat.udir.no/eksamenprovemateriell.html?kategori=rea3053&aar=2023-6&spraak=bokm%C3%A5l&trinn=annet&ferdighet=annet)
- [JSON](https://sokeresultat.udir.no/eksamenprovemateriell.html?kategori=rea3053&aar=2023-7&spraak=bokm%C3%A5l&trinn=annet&ferdighet=annet)

Tips: Du står fritt til å velge hvordan programmet skal presentere informasjon, så lenge presentasjonen er godt egnet til å vise det oppgaven spør etter.

a) Lag et program som presenterer en oversikt over de tre største kategoriene målt i antall apper. Oversikten skal vise antallet apper, gjennomsnittsratingen og det gjennomsnittlige antallet installasjoner for hver av disse tre kategoriene.
Tips: For å kunne beregne gjennomsnittet av antallet installasjoner må du tilpasse innholdet i det aktuelle datafeltet. Du vil få noe uttelling om du bare viser antallet apper og gjennomsnittsratingen.

b) Utvid programmet slik at det også presenterer de tre mest populære appene, målt i antall installasjoner, i hver av disse tre kategoriene.
