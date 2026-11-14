+++
title = "Poznaj Zola Kiss: Czysty Markdown w praktyce"
date = 2024-11-15
+++

Witaj w pierwszym wpisie na moim nowym blogu opartym na motywie **Zola Kiss**. Ten tekst służy jako demonstracja możliwości silnika i samego motywu. Znajdziesz go w katalogu `content/posts/`.

Aby zobaczyć zmiany na żywo podczas lokalnej pracy, wystarczy uruchomić komendę `zola serve`. Zola automatycznie przebuduje stronę po zapisaniu pliku.

## Struktura wpisu

Każdy plik w Zoli wymaga nagłówka TOML, który definiuje metadane, takie jak tytuł i data:

```toml
+++
title = "Tytuł wpisu"
date = 2024-11-15
+++
```

## Podświetlanie składni

Zola oferuje potężne wsparcie dla bloków kodu. Poniżej przykład w języku Rust, w którym napisana jest Zola:

```rust
fn main() {
    let site = "Zola Kiss";
    println!("Witaj w {}", site);
}
```

## Elementy tekstowe

Oto kilka rzeczy, które możesz przetestować w tym motywie:
*   **Pogrubiony tekst** i *kursywa*.
*   `Kod inline`, który powinien się wyróżniać.
*   [Link do dokumentacji Zoli](https://www.getzola.org/documentation/getting-started/overview/), aby sprawdzić kolorystykę odnośników.

> A to jest cytat blokowy. Klise ma bardzo specyficzny sposób ich wyświetlania, więc warto sprawdzić, jak wygląda po przeniesieniu stylów.

Ten wpis to dopiero początek. W kolejnych krokach sprawdzimy obrazki, tabele i inne elementy.
