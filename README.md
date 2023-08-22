# Vinyl Records Collection Theme

[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Wivik_vinyl-records-collection-theme&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=Wivik_vinyl-records-collection-theme)

A [Hugo](https://gohugo.io) theme made to present your vinyl records collection to the world.

[![Theme example](/images/tn.jpg)](/images/screenshot.jpg)

If this theme has been designed for a vinyl collection, it's also suitable for any other music library with some [customization](#customize-theme).


## Live demo

https://vinyl.zedas.fr

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

Update the configuration file  :

```yaml
baseurl: <your site URL>
languageCode: 'en-us'
title: 'My Vinyl Records Collection'
author: <Your Name>
theme: vinyl-records-collection-theme

taxonomies:
  artist: artist
  genres: genres
  label: label
  year: year
  format: format


```

Or if you use the Toml format :

```toml
baseurl = '<your site URL>'
languageCode = 'en-us'
title = 'My Vinyl Records Collection'
author = '<Your Name>'
theme = 'vinyl-records-collection-theme'

[taxonomies]
  artist = 'artist'
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

## Documentation

The most comprehensive documentation of the support content is directly written in the [archetype](/archetypes/default.md).

## Customize theme

### Custom colors

The CSS file is mostly variabilized and can be overloaded suing a `custom.css` file that will be loaded after the default style.

```bash
├── assets
│   └── css
│       └── custom.css # 2. customize the color there
└── themes
    └── vinyl-records-collection-theme
        ├── assets
        │   ├── css
        │   │   ├── custom.css ## 1. copy this file to the site assets folder, in a 'css' sub-folder
        │   │   └── style.css

```

### Custom images

You can change the background image of the header and the footer, also the default record image, by adding your own one in the site `assets` folder.

```bash
├── assets
│   └── img
│       └── back-header.jpg # will have the priority over the one in the template
└── themes
    └── vinyl-records-collection-theme
        ├── assets
        │   └── img
        │       ├── back-footer.jpg
        │       ├── back-header.jpg
        │       └── default.png

```

The theme expects the header and footer to be in `jpg` format, while the default record image is expected to be in `png`.

## License

Vinyl Records Collection Theme is [licensed under MIT](/LICENSE).

Pictures in the `sample/` folder are from https://www.publicdomainpictures.net

## Maintenance and contribution

This theme is maintained by Seb, the original author.

If you wish to contribute, fork this repository and open a pull-request. Any contribution is welcome !

## Support

If you like this project and was useful for you, please consider supporting its development. This theme is made by a coffee-lover, so you can just :

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/I2I1CL34H)

