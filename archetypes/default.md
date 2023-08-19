---
# Mandatory parts :
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
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
## These pictures should be in the site asset folder : <your hugo site>/assets
## If you put them into a sub-folder, don't forget it in the path !
# pictures:
#   - this-album/pict.jpg

## The publish year
# year: 1990

## Below the metadata block, you can write some content such as a review or anything else you want. It'll be displayed in the album page.
---
