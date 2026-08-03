# Proof Pages for Divi 5 — live demo

The rendered static demo for Proof Pages for Divi 5, a twelve-family Divi 5 layout pack
sold on the Elegant Themes Divi Marketplace.

This is a byte-for-byte archive of what is served at
**https://proofpages.interactive-guru.com/** — pulled from the live docroot, not rebuilt.

## Contents

    index.html            the storefront: hero, stats, twelve family cards
    f1-…  …  f12-…        96 pages, eight per family
    wp-content/uploads/   the demo imagery
    wp-content/et-cache/  Divi's generated per-page CSS

Plain HTML. No build step, no JavaScript, no external dependencies. Upload it to any static
host and it works.

## Why et-cache is committed

Divi writes each page's styles to `wp-content/et-cache/<post-id>/*.css`, and those selectors
are keyed to **module numbering**. Deploy the HTML without the matching CSS and the pages
render with the previous layout's styling — wrong spacing, wrong background colours, dark
text on dark panels — while nothing 404s and every link check passes.

So the CSS is part of the site, not a build artefact. Keep it with the HTML.

## Page naming

Each family has eight pages. Six are role-named (`-home`, `-case-studies`, `-portfolio`,
`-client-words`, `-start-a-review`, `-sections`); the other two carry that family's own
story, so f9's are `f9-husk-stone-ground-identity` and `f9-cadence-mark-for-the-favicon-up`.

f1's long-form case study is `f1-bayline-booking-clarity`, which is Bayline House's own
story — an earlier version of this pack used that slug on all twelve families, which is why
it may look familiar in old links.

## The product itself

This repository holds only the public demo. The product source, the submitted archives, the
build and verification scripts, the listing copy and the WordPress rig that generates this
site are archived privately — the pack is a paid product and its source does not belong in a
public repository.
