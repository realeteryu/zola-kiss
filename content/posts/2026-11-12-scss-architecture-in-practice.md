+++
title = "Managing SCSS Architecture in Practice"
date = 2026-11-12
description = "A practical guide on how to structure SCSS partials, variables, and imports cleanly in a static site project."
[taxonomies]
tags = ["scss", "css", "guide"]
+++

Dividing styling code into smaller partial files is the key to maintaining order in medium and large front-end projects.

## How It Works in Our Setup

The main `main.scss` file acts as the coordinator — this is where we define global variables, mixins, and module import order:

```scss
@charset "utf-8";

@import url("[https://fonts.bunny.net/css?family=roboto:400,700&display=swap](https://fonts.bunny.net/css?family=roboto:400,700&display=swap)");

// Variables and configuration
$sans-family: 'Roboto', sans-serif;
// ...
```

Thanks to this approach, every component — whether it's the navigation bar, footer, or post section — has its dedicated place, making the code clean and easy to modify.

We are testing the rendering of code blocks as well as inline elements like `kbd` and `mark`, which now look fantastic in both color schemes.
