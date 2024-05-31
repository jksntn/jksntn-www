# Welcome to JKSNTN Website!

Berikut ini dokumentasi dari website ini.

---

## Development

To develop this site, you'll need to have [Hugo](https://gohugo.io/getting-started/installing/#quick-install) installed in your environment. 

We also use pnpm instead of npm/yarn at Execute Big. You should install it here: https://pnpm.io. If you opt to use an alternative package manager to manage dependencies, please be sure to clean up the lock files and other temp files before submitting your code for review.

```bash
# Install dependencies
$ pnpm install

# Same as running `hugo server`
$ pnpm dev
```

## Using Archetypes

Hugo utilizes archetypes to create structured content from templates. 

```bash
# To create a new blog entry
$ hugo new --kind blog blog/your-post-name
```

## Acknowledgements

This website is built based on [Hugo Serif Theme](https://themes.gohugo.io/hugo-serif-theme/) by [@jugglerx](https://github.com/jugglerx/).

## Short Code

### Blog Meta

```
---
title: "Judul Postingan"
date: 2017-08-27
featured_image: images/01.jpg
featured: false
draft: false
"blog/tags": [ tag1, tag2, tag3 ]
---
```

### Youtube

Example of use:

```
{{< youtube 4GJC6QHXb1s >}} 
```

### Caraousel

Image gallery, use group of image on specific directory.

Example:

```
{{< carousel dir="/images/events" duration="2500" height="400px" >}}
```

### Announcement

Example Warning Annoucement:

```
{{< announcement content="<p class='title'>TITLE</p>DESC <a href=\"/contact\">LINK</a>." class="danger" >}}
```

Example normal announcement

```
{{< announcement content="DESC.">}}
```

### Button

Example of use:

```
{{< button text="Request Consultation" url="https://forms.gle/mgncUxpV21w59jNk7" external="true" >}}
```

### FAQ Accordion

Example of use: 

```
{{< expand "TITLE" >}}
DESC
{{< /expand >}}
```