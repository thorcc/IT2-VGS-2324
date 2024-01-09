# Algoritmer

- [Sorteringsalgoritmer](#sorteringsalgoritmer)
- [Effektivitet (Stor-O)](#effektivitet)

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

## Sorteringsalgoritmer

Kommer..

## Effektivitet

Kommer..
