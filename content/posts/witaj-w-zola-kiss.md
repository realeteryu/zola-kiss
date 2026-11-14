+++
title = "Witaj w Zola Kiss!"
date = 2026-11-14
+++

To jest pierwszy wpis demonstracyjny dla motywu **Zola Kiss**. Znajdziesz go w katalogu `content/posts/`. Możesz go edytować lub usunąć, aby zacząć tworzyć własne treści.

Aby zobaczyć zmiany na żywo podczas pracy, uruchom lokalny serwer komendą `zola serve`. Zola automatycznie przebuduje stronę po zapisaniu pliku.

Pliki wpisów w Zoli wymagają nagłówka TOML, który definiuje metadane:

```toml
+++
title = "Tytuł wpisu"
date = 2026-11-14
+++
```

Zola oferuje również potężne wsparcie dla bloków kodu ze składnią podświetlania. Oto przykład w języku Rust, w którym napisana jest Zola:

```rust
fn main() {
    let site = "Zola Kiss";
    println!("Witaj w {}", site);
}
```

Oto kilka rzeczy, które możesz przetestować w tym motywie:
*   **Pogrubiony tekst** i *kursywa*.
*   `Kod inline`, który powinien się wyróżniać.
*   [Link do dokumentacji Zoli](https://www.getzola.org/documentation/getting-started/overview/), aby sprawdzić kolorystykę odnośników.

> A to jest cytat blokowy. Klise ma bardzo specyficzny sposób ich wyświetlania, więc warto sprawdzić, jak wygląda po przeniesieniu stylów.
