# The OMnibus of MANTRAMS custom "Look and Feel"

## Bootstrap, SCSS and _custom.scss

The CollectionBuilder CSV template comes with **Bootstrap 5** already included (see [`/assets/lib/bootstrap.min.css`](/assets/lib/bootstrap.min.css) and [`/assets/lib/bootstrap.bundle.min.js`](/assets/lib/bootstrap.bundle.min.js)). For an introduction and to understand the implications of Bootstrap classes, see https://getbootstrap.com/.

With [_base.scss](/_sass/_base.scss), [_pages.scss](/_sass/_pages.scss) and [_theme-colors.scss](/_sass/_theme-colors.scss), CollectionBuilder extends or overwrites some Bootstrap elements to better fit the *out of the box (OOTB)* design and behavior (see [CollectionBuilder documentation](https://collectionbuilder.github.io/cb-docs/docs/advanced/architecture-overview/)). An introduction for how to customize CollectionBuilder can be found here: https://www.youtube.com/watch?v=yDcoltiq0ZY (44:30 onwards).

While CollectionBuilder allows for some [customization](https://collectionbuilder.github.io/cb-docs/docs/theme/), the OMnibus of MANTRAMS design requires more advanced manipulation of the provided template. Some of it is done by changing values in the CollectionBuilder SCSS ([`/_sass`](/_sass/) - not [`cb.scss`](/assets/css/cb.scss)) - and page templates ([`/_layouts`](/_layouts/)), but the bulk of customization is placed in [`_custom.scss`](/_sass/_custom.scss).

**To indicate our OMnibus custom CSS classes or [jekyll custom front matter variables](https://jekyllrb.com/docs/front-matter/) in the HTML source code, the naming scheme `omnibus-[name]` is used.**

## Preparatory work: Utilizing CollectionBuilder built in customization options

In this section, we describe changes to the general architecture of the website, not in data handling, based on the docs for [Page Config](https://collectionbuilder.github.io/cb-docs/docs/customization/) and [Edit Pages](https://collectionbuilder.github.io/cb-docs/docs/pages/):

- Until future modes of data exploration have been developed, the modes of access to data have been reduced by deleting the "Subjects" and the "Locations" option from the **navigation** ([`config-nav.html`](/_data/config-nav.csv)).
- The default location and zoom for the **map** was changed until enough data has been put in to default back to `auto` ([`theme.yml`](\_data\theme.yml)). The Esri Imagery map was chosen as a default to focus on spatiality and situatedness, not on political entities and urban settlements. Later on, more sophisticated GIS and data visualizations will be developed from research questions, data and user queries.
- To simplify the **Home/Landing Page**, all infographics and statistics have been removed or moved to the About section.

## Custom surgery: Reworking the CollectionBuilder templates

## _custom.scss code design