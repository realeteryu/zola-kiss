+++
title = "Test Markdown: Tabele, cytaty i bloki kodu"
date = 2025-11-14
+++

Ten wpis służy do sprawdzenia bardziej zaawansowanych elementów Markdown. Ze względu na datę, powinien znaleźć się na samym dole listy na stronie głównej.

## Tabele

Poniżej znajduje się tabela porównawcza. Sprawdzamy, czy obramowania i paddingi wyglądają dobrze.

| Cecha | Zola | Jekyll |
| :--- | :--- | :--- |
| Język | Rust | Ruby |
| Szybkość | Bardzo szybka | Wolniejsza |
| Zależności | Brak (single binary) | Wymaga środowiska Ruby |
| Krzywa uczenia | Średnia | Łatwa |

## Cytaty blokowe

Cytaty w motywie Klise mają charakterystyczny lewy pasek. Zobaczmy, jak wyglądają w praktyce:

> "Prawdziwa prywatność nie polega na życiu w jaskini, ale na tym, że to Ty decydujesz, kto i na jakich warunkach ma dostęp do Twojej cyfrowej rzeczywistości."

Możemy też zrobić cytat z wieloma akapitami:

> To jest pierwszy akapit cytatu.
>
> A to jest drugi akapit tego samego cytatu. Powinien mieć zachowany odstęp.

## Blok kodu TOML

Na koniec sprawdźmy, jak wygląda blok kodu TOML, którego używamy w Zoli do nagłówków:

```toml
+++
title = "Tytuł wpisu"
date = 2025-11-14
[extra]
toc = true
+++
