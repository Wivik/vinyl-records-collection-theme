# Vinyl Records Collection Theme

A [Hugo](https://gohugo.io) theme made to present your vinyl records collection to the world.

## Live demo

WIP

## Quick start

Create your new Hugo site.

```bash
hugo new site my-vinyl-records-collection
```

Add this theme to your project :

```bash
## Clone directly
git clone https://github.com/Wivik/vinyl-records-collection-theme themes/vinyl-records-collection-theme

## Or use as a sub module
git submodule add https://github.com/Wivik/vinyl-records-collection-theme themes/vinyl-records-collection-theme

```

This theme use a specific archetype, so delete or rename the default one.

```bash
rm <your hugo site folder>/archetypes/default.md
```

Update the configuration file and add :

```yaml
theme: vinyl-records-collection-theme

taxonomies:
  band: band
  genres: genres
  label: label
  year: year
  format: format
```

Or if you use the Toml format :

```toml
theme = 'vinyl-records-collection-theme'

[taxonomies]
  band = 'band'
  genres = 'genres'
  label = 'label'
  year = 'year'
  format = 'format'

```

## Create your first record

Create a new content file with hugo :

```bash
hugo new an-album-name.md
```

Open the newly created file, the archetype will basically tell you what you need to do to finish the job.

Example :

```markdown
---
# Mandatory parts :
title: "Disc7"
date: 2023-08-19T23:31:17+02:00
draft: true

# Optional parts that you still should fill in order to sort your collection

## Label : name of the label that published the record
label: Record's Label

## The band's name
band: Record's Band

## The genres this record is classified into
genres:
  - To sort

## Cover image : will be displayed in the album list and top page.
## Display a default one unless you change this value.
cover: 

# More optional details you can use for your collection.

## A quick description of your record. Markdown is supported
# description: |
#    This is a great album.

## Disc format : 45rpm, 33rpm, 78rpm or size if you prefer.
# format: 33rpm

## Any supplementary pictures you want to display.
## These pictures should be in the site asset folder :
## <your hugo site>/assets
## If you put them into a sub-folder, don't forget it in the path !
# pictures:
#   - this-album/pict.jpg

## The publish year
# year: 1990

## Below the metadata block, you can write some content such as a review or anything else you want. It'll be displayed in the album page.
---


```

## License

Vinyl Records Collection Theme is [licensed under MIT](LICENSE).

## Maintenance and contribution

This theme is maintained by Seb, the original author.

If you wish to contribute, fork this repository and open a pull-request. Any contribution is welcome !

## Support

If you like this project and was useful for you, please consider supporting its development. This theme is made by a coffee-lover, so you can just :

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/I2I1CL34H)

