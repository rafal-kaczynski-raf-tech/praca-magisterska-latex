# Praca dyplomowa magisterska

*[ENGLISH](README.en.md)*

---

**Tytuł:** *Modelowanie i sterowanie przekształtnika energoelektronicznego z wykorzystaniem metod sztucznej inteligencji w środowisku Python*

**Autor:** Rafał Kaczyński &nbsp;·&nbsp; nr albumu **342208**
**Promotor:** prof. dr hab. inż. Grzegorz Iwański
**Uczelnia:** Politechnika Warszawska, Wydział Elektryczny
**Instytut:** Instytut Sterowania i Elektroniki Przemysłowej
**Kierunek:** Informatyka Stosowana &nbsp;·&nbsp; **Specjalność:** Informatyka w Biznesie
**Rok obrony:** 2026

---

## O pracy

Praca przedstawia projekt oraz implementację autorskiego **Bliźniaka Cyfrowego** (ang. *Digital Twin*) dwukierunkowego przekształtnika prądu stałego typu Buck-Boost w języku **Python**. Środowisko symulacyjne zostało zintegrowane z metaheurystycznym algorytmem **Optymalizacji Rojem Cząstek (PSO)**, służącym do automatycznego strojenia bezmodelowego sterownika typu **Bang-Bang (MF-BB)**. Praca ma charakter programistyczno-optymalizacyjny, a jej zwieńczeniem jest empiryczna walidacja wyników z komercyjnym oprogramowaniem **PSIM**.

**Słowa kluczowe:** Bliźniak Cyfrowy · Python · Optymalizacja Rojem Cząstek (PSO) · przekształtnik Buck-Boost · sterowanie bezmodelowe · inżynieria oprogramowania.

## Powiązane repozytorium

Kod źródłowy Bliźniaka Cyfrowego (silnik fizyczny + sterownik MF-BB + PSO):
👉 [github.com/rafal-kaczynski-raf-tech/praca-magisterska](https://github.com/rafal-kaczynski-raf-tech/praca-magisterska)

## Struktura repozytorium

| Plik / katalog | Zawartość |
|---|---|
| `EE-dyplom.tex` | Plik główny — strona tytułowa, streszczenie, abstract, struktura |
| `EE-dyplom.bib` | Bibliografia (BibTeX) |
| `EE-dyplom.cls` | Klasa LaTeX szablonu (nie modyfikować) |
| `tekst/` | Treść rozdziałów (`wstep.tex`, `analiza.tex`, `realizacja.tex`, `ai.tex`, `podsumowanie.tex`) |
| `rysunki/` | Rysunki, wykresy i schematy używane w pracy |
| `gfx/` | Grafiki szablonu (loga PW, nagłówki) — nie modyfikować |
| `Makefile` | Skrypt do ręcznej kompilacji (XeLaTeX + Biber) |

## Jak skompilować

### Overleaf (zalecane)

1. Importuj projekt z GitHub: *New Project → Import from GitHub*.
2. Otwórz **Menu → Settings → Compiler** i wybierz **XeLaTeX** (kompilacja pdfLaTeX nie zadziała poprawnie).
3. Kliknij **Recompile**.

### Lokalnie (macOS / Linux z TeX Live)

```bash
make            # XeLaTeX → Biber → XeLaTeX → XeLaTeX
make clean      # usuwa pliki pomocnicze
```

## Status pracy

Praca jest w trakcie pisania. Stan poszczególnych rozdziałów odzwierciedla historia commitów.

## Licencja i prawa autorskie

Treść pracy dyplomowej (pliki w katalogu `tekst/`, `rysunki/` oraz `EE-dyplom.tex`, `EE-dyplom.bib`) — © Rafał Kaczyński, 2026. Wszelkie prawa zastrzeżone.

## Atrybucja szablonu

Praca korzysta z szablonu **EE-dyplom** dla Wydziału Elektrycznego Politechniki Warszawskiej.

* Autor szablonu: *Łukasz Makowski* &lt;lukasz.makowski.ee@pw.edu.pl&gt;
* Repozytorium szablonu: [github.com/SP5LMA/EE-dyplom](https://github.com/SP5LMA/EE-dyplom)
* Licencja szablonu: [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/)
* Szablon jest zgodny z [Zarządzeniem JM Rektora PW 4/2022](https://www.bip.pw.edu.pl/Wewnetrzne-akty-prawne/Dokumenty-Rektora-PW/Zarzadzenia-Rektora/2022/Zarzadzenie-nr-4-2022-Rektora-PW-z-dnia-27-01-2022) dotyczącym formatowania prac dyplomowych.
