+++
title = "Test Markdown: Obrazy i formatowanie tekstu"
date = 2026-10-14
+++

Ten wpis ma na celu sprawdzenie, jak motyw radzi sobie z różnymi elementami języka Markdown. Zaczynamy od zwykłego akapitu z **pogrubieniem**, *kursywą* oraz `kodem inline`, który powinien mieć odpowiednie tło i czcionkę.

## Sekcja z obrazkiem

Poniżej znajduje się przykładowy obrazek pobrany z zewnętrznego serwera. Sprawdzamy, czy ładuje się poprawnie i czy zachowuje proporcje.

![Przykładowy obrazek](https://picsum.photos/800/400)

Obrazek powinien być wyśrodkowany i nie wychodzić poza marginesy strony. Jeśli chcemy dodać podpis, w czystym Markdownie nie ma na to bezpośredniego tagu, ale motyw Klise radzi sobie z tym za pomocą HTML:

<figure>
    <img src="https://picsum.photos/400/300" alt="Mniejszy obrazek">
    <figcaption>Rysunek 1. Przykładowy podpis pod obrazkiem.</figcaption>
</figure>

## Listy i linki

Oto lista nieuporządkowana:
- Pierwszy element listy
- Drugi element z [linkiem do Zoli](https://www.getzola.org/)
- Trzeci element

A tutaj lista uporządkowana:
1. Krok pierwszy
2. Krok drugi
3. Krok trzeci

Sprawdźmy jeszcze blok kodu w języku Python, aby upewnić się, że kolory składni działają poprawnie w tym motywie:

```python
def witaj(imie):
    print(f"Witaj, {imie}!")
    
witaj("Eteryu")
