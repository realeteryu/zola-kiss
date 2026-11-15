+++
title = "Prezentacja lightboxa obrazów"
date = 2026-10-25T10:00:00+07:00
description = "Wpis demonstracyjny testujący wbudowany lightbox obrazów w każdej możliwej sytuacji — zwykłe obrazy, figury z podpisami, podlinkowane obrazy, brak tekstu alternatywnego, obrazy w linii, surowy HTML i obrazy wewnątrz list."

[taxonomies]
tags = ["demo", "images"]

[extra]
toc = true
+++

Ten wpis testuje wbudowany **lightbox obrazów** w każdej sytuacji, używając prostych, szarych obrazów zastępczych. Kliknij dowolny obraz w treści wpisu, aby otworzyć go na pełnym ekranie, a następnie kliknij gdziekolwiek lub naciśnij <kbd>Esc</kbd>, aby zamknąć. Obrazy opakowane w link są celowo pomijane, aby sam link działał poprawnie.

## 1. Standardowy obraz Markdown

Prosty obraz Markdown. Powinien być **powiększany**, a jego tekst `alt` staje się etykietą okna dialogowego.

![Prosty szary placeholder](https://placehold.co/600x400/cccccc/999999?text=Obraz)

## 2. Obraz w figurze z podpisem

Opakowany w `<figure>` z `<figcaption>`. Obraz jest powiększany, a podpis pozostaje na swoim miejscu.

<figure>
  <img src="https://placehold.co/800x300/cccccc/999999?text=Szeroki+Obraz" alt="Szeroki szary placeholder">
  <figcaption>Rys. 1. Obraz z podpisem pod nim.</figcaption>
</figure>

## 3. Podlinkowany obraz (musi pozostać linkiem)

Ten obraz jest opakowany w link. Kliknięcie go powinno **przenieść do linku**, a nie otwierać lightboxa.

[![Kliknij mnie — otwieram repozytorium](https://placehold.co/600x400/cccccc/999999?text=Kliknij)](https://github.com/realeteryu/zola-kiss)

## 4. Obraz bez tekstu alt

Brak atrybutu `alt`. Nadal powiększany; okno dialogowe używa ogólnej etykiety zastępczej.

![](https://placehold.co/800x300/cccccc/999999?text=Brak+Alt)

## 5. Mały obraz

Obrazy mniejsze niż widok są wyśrodkowane i wyświetlane w swoim naturalnym rozmiarze.

![Mały szary placeholder](https://placehold.co/200x200/cccccc/999999?text=Mały)

## 6. Kilka obrazów w rzędzie

Opakowane w `<div class="gallery">`, aby uzyskać schludny, responsywny rząd o równej wysokości, który zawija się na małych ekranach. Każdy obraz nadal otwiera się niezależnie w lightboxie.

<div class="gallery">
  <img src="https://placehold.co/400x400/cccccc/999999?text=1" alt="Obraz w galerii pierwszy">
  <img src="https://placehold.co/600x400/cccccc/999999?text=2" alt="Obraz w galerii drugi">
  <img src="https://placehold.co/200x200/cccccc/999999?text=3" alt="Obraz w galerii trzeci">
</div>

## 7. Obraz w linii wewnątrz akapitu

Obraz może również znajdować się w linii zdania, tak jak ten ![malutki placeholder](https://placehold.co/50x50/cccccc/999999?text=In) i pozostaje powiększany bez psucia układu tekstu.

## 8. Surowy tag HTML `<img>`

Napisany bezpośrednio jako HTML, a nie Markdown — zachowuje się tak samo.

<img src="https://placehold.co/800x300/cccccc/999999?text=Surowy+HTML" alt="Szary placeholder wyrenderowany z surowego HTML">

## 9. Obrazy wewnątrz listy

Obrazy w elementach listy są zmniejszane do małych, wyrównanych miniatur, aby lista pozostała schludna. Każda miniatura jest nadal powiększana.

- ![Miniatura](https://placehold.co/100x100/cccccc/999999?text=Mini) Element listy zaczynający się od małej miniatury.
- ![Miniatura](https://placehold.co/150x80/cccccc/999999?text=Mini2) Inny element z szerszą miniaturą.
- Zwykły element listy dla porównania.

## 10. Podlinkowany obraz wewnątrz figury

Łączy przypadki 2 i 3: figura jest dekoracyjna, ale obraz prowadzi do linku, więc link wygrywa z lightboxem.

<figure>
  <a href="https://github.com/realeteryu/zola-kiss">
    <img src="https://placehold.co/600x400/cccccc/999999?text=Link+w+Figurze" alt="Obraz w figurze, który jest również linkiem">
  </a>
  <figcaption>Rys. 2. Obraz z podpisem, który prowadzi do repozytorium.</figcaption>
</figure>

To pokrywa każdy przypadek, który musi obsłużyć lightbox: zwykłe, z podpisem, podlinkowane, bez tekstu alt, małe, powtarzające się, w linii, z surowego HTML i osadzone w listach.
