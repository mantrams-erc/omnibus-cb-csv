---
title: About
layout: about
permalink: /about.html

omnibus-site-theme: light # toggle: dark | light
omnibus-site-logo-gradient: false # toggle boolean
omnibus-site-main-color-custom: "#000000" # insert color hex code
omnibus-site-bg-color-custom: "#f533ff" # insert color hex code
omnibus-site-grainy-bg: true # toggle boolean 
omnibus-gradient-color-2: "#e51542ff"
omnibus-gradient-color-3: "#ff9d00"
omnibus-gradient-color-4: "#d95436"
#insert 3 custom color hexcodes to layer in grainy svg animation over omnibus-site-bg-color-custom
omnibus-bg-image: "'/assets/img/MANTRAMS_TF3_GOET_RC6_ RAMANANDI-L11009783.jpg'" #insert filepath

# include CollectionBuilder info at bottom
credits: true
# featured-image value can be one objectid for a photo object in this collection, a relative path to an image in this project, or a full url to any image. If left blank, no featured image will appear at top of About page.
about-featured-image:
# set background-position for featured image, "center", "top", "bottom"
position:
# major heading to display over featured image
heading:
# paragraph text below heading in featured image
sub-heading: 
# additional padding added to the feature to increase size. Give value in em or px, e.g. "5em".
padding:
# Edit the markdown on in this file to describe your collection
# Look in _includes/feature for options to easily add features to the page
---

## About CollectionBuilder CSV

<div class="row">
  <div class="col-md-6 h-100">
  {% include index/content.html %}
  </div>
<div class="col-md-6 h-100">
  {% include index/time.html %}
  </div>
</div>

This demo collection features items from the University of Idaho Library's [Digital Collections](https://www.lib.uidaho.edu/digital/), and is build using [CollectionBuilder-CSV](https://github.com/CollectionBuilder/collectionbuilder-csv).

CollectionBuilder-CSV is a "Stand Alone" template for creating digital collection and exhibit websites using Jekyll, given:

- a CSV of collection metadata
- a folder of images, PDFs, audio, or video files

Driven by your collection metadata, the template generates engaging visualizations to browse and explore your objects.
The resulting static site can be hosted on any basic web server.

[CollectionBuilder](https://github.com/CollectionBuilder/) is an set of open source tools for creating digital collection and exhibit websites that are driven by metadata and powered by modern static web technology.
See [CB Docs](https://collectionbuilder.github.io/cb-docs/) for detailed information.

{% include feature/image.html objectid="demo_001" width="75" %} 

<!-- IMPORTANT!!! DELETE this comment and the include below when you are finished editing this page for your collection. The include below introduces about page features. They will show up on your collection's about page until you delete it.  -->
{% include cb/about_the_about.md %} 
