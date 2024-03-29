---
type: article
tags: tailwind, vuepress
image: https://vuepress.vuejs.org/hero.png
---

# Using Tailwind with VuePress

Using TailwindCSS with VuePress can be tricky at first, but here's how to do it!

<!-- more -->

I tried importing the `tailwind.css` file into the `<style>` tag, but I experienced higher build times, as much as **10x**.

If you import it in the `<script>` tag, it'll reduce the build duration by a large extent!

If you're using a custom theme or you've designed one yourself, you can open the `Layout.vue` and insert the following line to it's `<script>` tag.

```js
// Layout.vue

import '../styles/tailwind.css'
```

> If you want to use tailwind with the default theme, it will mess up the design of the default theme!

That's it!