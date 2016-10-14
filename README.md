###Installation

To enable this theme, edit the `config.php` to `$config['theme'] = 'semantic';`

To change theme colors edit the `config.php` and change `$config['semantic_color'] = 'teal';` to any Semantic-UI default colors.

Also edit `$config['semantic_alt_color'] = 'grey';`

Requires `PicoTags` plugins to properly use menu item and filter post depending on the category.

Requires [Pico-Pagination](https://github.com/rewdy/Pico-Pagination). 

####How to use this

Menu items are created from `.md` files that have the following `YAML` info

```
--- 
Menu: about me 
Tags: menu
Link: /users/stephen 
---
```

Where the `Menu` is the title of the menu item, `Tags` has to be `menu, and `Link` is base of {{ base_url }}. To order the menu location, name the menu files with in numeric order. For example 

```
05-blog.md
10-aboutme.md
15-fun.md
```

For blog, create a new `blog` folder under `content`. The `index.md` in that location should have the following as an example

```
---
Title: blog
Filter: blog, menu
Author: stephen
Date: 10 September 2016
Template: blog
---
```

Each new blog post should have the Tags of `blog`. 

For images, please create an `assets` folder under the root of the Pico install, and keep the assets there. 

I'll write better and clearer instructions once I have more time. 

Of course, [Semantic-UI](https://github.com/Semantic-Org/Semantic-UI) code is all over this repository. I created this theme base off version 2.24. 