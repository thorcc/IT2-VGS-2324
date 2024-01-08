# Algoritmer og pseudokode

## Algoritmer

- Hvis du gir en *presis* beskrivelse for hvordan man skal løse et *problem*, så har du
beskrevet det vi kaller en algoritme 
- En algoritme består av en serie med små og entydige steg
- En algoritme må
  - stoppe etter et endelig antall steg
  - ta null eller flere input
  - produsere et output som står i forhold til input
  - være helt presist definert for hvert enkelt steg
- En algoritme *bør* være effektiv

## Eksempel: En algoritme som finner høyeste tallet i en liste

```python
def høyeste(liste):
    høyest = liste[0]
    for tall in liste:
        if tall > høyest:
            høyest = tall
    return høyest

print(høyeste([2, -4, 5, 1])) # -> 5
```

## Pseudokode

- en måte å beskrive en algoritme på ved hjelp av naturlig språk
- brukes ofte som et verktøy for å planlegge og designe algoritmer før de faktisk blir kodet i et bestemt programmeringsspråk
- gjør det lettere å kommunisere og samarbeide med andre programmerere, samt å teste og feilsøke algoritmer før de blir kodet.
- en god måte å lære grunnleggende programmeringskonsepter på, da det kan hjelpe deg med å forstå hvordan ulike instruksjoner og logiske uttrykk fungerer sammen for å løse et bestemt problem.

### Standard for pseudokode på eksamen i Informasjonsteknologi 2

På eksamen forventes det at kandidaten behersker å lese pseudokode skrevet etter denne standarden. Alle nøkkelord skrives med store bokstaver og på engelsk, mens pseudokoden ellers skrives på norsk i oppgavene. Kandidatene har metodefrihet i sitt valg av standard for pseudokode, men det forventes konsekvens. Det forventes også at pseudokode kandidatene leverer oppfyller formålet med pseudokode, bruker naturlig språk og ikke ligger tett opptil syntaks for programkode, men likevel er presis nok til å komplett beskrive logikken i programmet. Alle strukturblokker skal være indentert i pseudokode.

Kandidatene står også fritt til å bruke norsk eller engelsk i sin kode, men det forventes konsekvens.

### Udirs ordliste

Følgende nøkkelord benyttes for å representere struktur (flytkontroll) i pseudokode på eksamen

| nøkkelord                   | beskrivelse                                                                                         |
| --------------------------- | --------------------------------------------------------------------------------------------------- |
| SEQUENCE                    | representerer lineære operasjoner som utføres sekvensielt etter hverandre.                          |
| FUNCTION-RETURN-ENDFUNCTION | representerer en kallbar subrutine med eller uten returverdi.                                       |
| WHILE                       | er en løkke med en betingelse for å kjøres i begynnelsen av løkken.                                 |
| REPEAT-UNTIL                | er en løkke som kjøres minst en gang, med en betingelse for gjentakelse til slutt.                  |
| FOR                         | er en løkke som kjøres et visst antall ganger eller over elementer i en variabel eller tilsvarende. |
| IF-THEN-ELSE                | er en valgsetning som endrer flyten i algoritmen.                                                   |
| CASE-OF-OTHERS-ENDCASE      | er en flerveis forgrening av flyten basert på verdien av et uttrykk.                                |
| BEGIN-EXCEPTION-WHEN-END    | er håndtering av unntak i kjøretid.                                                                 |

 
Følgende nøkkelord benyttes for å representere operasjoner i pseudokode på eksamen

| nøkkelord      | beskrivelse                                                                                                                   |
| -------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| SET TO         | er deklarering eller initialisering av en variabel.                                                                           |
| CALL-RETURNING | er kall til en rutine, funksjon eller metode hvor RETURNING er returverdi dersom rutinen, funksjonen eller metoden gir dette. |
| READ           | er lesing eller mottak av input.                                                                                              |
| DISPLAY        | er visning av output til bruker.                                                                                              |
| COMPUTE        | er beregning eller avgjøring av resultat.                                                                                     |
| INCREMENT      | er å legge til 1 til en tallvariabel.                                                                                         |
| DECREMENT      | er å trekke fra 1 fra en tallvariabel.                                                                                        |

Følgende nøkkelord benyttes for å representere logiske operatorer i pseudokode på eksamen
| nøkkelord    | beskrivelse                                                 |
| ------------ | ----------------------------------------------------------- |
| EQUAL TO     | er evaluering om to uttrykk har lik verdi                   |
| LESSER THAN  | er evaluering om et uttrykk har lavere verdi enn et annet   |
| GREATER THAN | er evaluering om et uttrykk har høyere verdi enn et annet   |
| NOT          | er negering av et logisk uttrykk                            |
| OR           | er en evaluering av minst ett at to logiske sannhetsverdier |
| AND          | er en evaluering av to sannhetsverdier                      |

## Flytdiagram

- viser en visuell representasjon av en algoritme eller et program
- viser *flyten* i en algoritme eller et program

### Symboler

| Symbol                                 | Navn                 | Beskrivelse                                                                                                                                                             |
| -------------------------------------- | -------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![](./bilder/Flowchart_Line.svg)       | Flowline             | Viser rekkefølgen på operasjoner. En linje går fra ett symbol og peker på et annet. Pilspissen kan droppes hvis flyten går ovenfra og ned, eller fra venstre til høyre. |
| ![](./bilder/Flowchart_Terminal.svg)   | Terminal             | Start eller slutte på algoritme eller program. Inneholder vanligvis ordet "Start" eller "Slutt".                                                                        |
| ![](./bilder/Flowchart_Process.svg)    | Process              | En eller flere operasjoner, som endrer verdi, form eller plassering av data. For eksempel: `gjør alle bokstaver små`                                                    |
| ![](./bilder/Flowchart_IO.svg)         | Input/Output         | Hent inn (input) eller vis (print) data.                                                                                                                                |

> [Draw.io](https://www.drawio.com/) kan brukes for å tegne flytdiagrammer.
> Du finner symbolene for flytdiagram under `flowchart` i menyen til venstre.

### Eksempel

![](./bilder/flytdiagram.png)

## Oppgaver

- [./oppgaver.md](./oppgaver.md)