# Zola-Kisse

A minimalist, responsive port of the [Jekyll-Klisé](https://github.com/piharpi/jekyll-klise) theme for the [Zola](https://www.getzola.org/) static site generator.

**[Live Demo](https://realeteryu.github.io/zola-kisse)**

## Features

- **Minimalist Design:** Clean typography and focused reading experience.
- **Light & Dark Mode:** Theme switcher with user preference persistence.
- **Responsive Layout:** Optimized for mobile, tablet, and desktop screens.
- **Configurable Navigation & Footer:** Managed directly through `config.toml` using Zola internal links (`@/`).
- **Syntax Highlighting & Emoji:** Built-in support for Zola's code highlighting and emoji rendering.
- **Conditional RSS Support:** Automatic feed links in the menu and footer when feed generation is enabled.

## Installation

### Option 1: Git Submodule (Recommended)

From the root of your Zola site, add the theme as a submodule:

```bash
git submodule add https://github.com/realeteryu/zola-kisse.git themes/kisse
```

### Option 2: Clone Directly

Navigate to your Zola site directory and clone the repository into the `themes` folder:

```bash
git clone https://github.com/realeteryu/zola-kisse.git themes/kisse
```

## Configuration

Enable the theme, Sass compilation, and feed generation in your site's `config.toml`:

```toml
theme = "kisse"
compile_sass = true
generate_feeds = true

taxonomies = [
    { name = "tags" },
]

[markdown]
render_emoji = true
```

### Theme Settings, Navigation & Footer

Configure your profile details, homepage post limit, navigation menu, and extra footer links under `[extra]` in `config.toml`:

```toml
[extra]
author = "Your Name"

# Avatar URL (external link or path inside static/, e.g., "/avatar.png")
avatar = "https://example.com/avatar.png"

footer_text = "<a href='https://github.com/realeteryu/zola-kisse'>kisse</a> theme for <a href='https://www.getzola.org/'>zola</a>"

# Number of posts displayed on the homepage
number_of_posts = 5

# Navigation menu (supports Zola @/ internal links)
[[extra.nav]]
name = "home"
url = "@/_index.md"

[[extra.nav]]
name = "archive"
url = "@/posts/_index.md"

[[extra.nav]]
name = "about"
url = "@/about/_index.md"

# Additional footer links
[[extra.footer]]
name = "support"
url = "https://ko-fi.com/yourusername"
```

## Support

If you find Kisse useful and would like to support its development, you can buy me a coffee:

**[☕ Support Kisse on Ko-fi](https://ko-fi.com/eteryu)**

## License

This project is open source and available under the [MIT License](LICENSE). Based on the original [Jekyll-Klisé](https://github.com/piharpi/jekyll-klise) theme by piharpi.
