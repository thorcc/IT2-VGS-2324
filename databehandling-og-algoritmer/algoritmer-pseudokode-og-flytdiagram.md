# Algoritmer og pseudokode

## Algoritmer

- Hvis du gir en *presis* beskrivelse for hvordan man skal løse et *problem*, så har du
beskrevet det vi kaller en algoritme 
- Algoritmer er en serie med små og entydige steg
- En algoritme må
  - stoppe etter et endelig antall steg
  - hvert steg må være helt presist definert
  - ta null eller flere input
  - produsere et output som står i forhold til input
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

## Flytdiagram

TODO: Skriv mer her..

- en visuell representasjon av en algoritme 


## Oppgaver

1. Gjør oppgave 1 til 7 på høstens IT2-eksamen for privatister. [UDIR: IT2-H23](https://kandidat.udir.no/epsmateriell/eksamen?fagkode=rea3049-py&malform=nb-no&semester=h&ar=2023&eksamensdeltype=eksamen)
2. Gjør oppgave 1 til 7 på fjorårets IT2-eksamen. [UDIR: IT2-V23](https://kandidat.udir.no/epsmateriell/eksamen?fagkode=rea3049-py&malform=nb-no&semester=v&ar=2023&eksamensdeltype=eksamen)

> Passord: `Eksamen`
