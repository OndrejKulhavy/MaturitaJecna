
<div align="center">
  <img src="https://www.spsejecna.cz/ci/SPSE-Jecna_Logotyp.png" alt="SPSE Jecna Logotyp" width="400" style="margin: 20px;">
</div>

# Maturitní Téma: Algoritmizace - Rekurze, Brute Force, Heuristiky, Nedeterministické algoritmy
- **Anki Flashcards**: [![Anki Flashcards](https://img.shields.io/badge/Anki-Flashcards-1f425f.svg)](https://ankiweb.net/shared/info/)
- **Autoři**: Erik Boháč

## Shrnutí
Krátké shrnutí tématu, zahrnující klíčové body a záměr práce

## Video
Odkaz na případné video, které ilustruje nebo doplňuje téma

## Obsah
### Rozcestník
- [Rekurze](#Rekurze)
- [Brute Force](#Brute-Force)
- [Heuristiky](#heuristiky)
- [Nedeterministické algoritmy](#Nedeterministické-algoritmy)

### Samotný Obsah
#### Rekurze
Představuje opakované vnořené volání stejného podprogramu (funkce). Součástí rekurzivní funkce by měla být ukončující podmínka určující, kdy se má vnořování zastavit. Chyba v rekurzi může způsobit vyčerpání paměti pro zásobník a následně ukončení programu.

```python
def factorial(number: int) -> int:
    if number < 0:
        raise ValueError('Undefined for value < 0')
    if number == 0:
        return 1
    return number * factorial(number - 1)
```

#### Brute Force

#### Heuristiky
#### Nedeterministické algoritmy

## Zdroje a Zajímavé Odkazy
Obrázek reprezentující rekurzi:
(https://cs.wikipedia.org/wiki/Rekurze#/media/Soubor:Sierpinski.svg)
