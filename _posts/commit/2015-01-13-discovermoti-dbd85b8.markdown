---
layout: commit

title:  "dbd85b8"
date:   Tue Jan 13 14:25:16 2015

author: ladislas
email:  ladislas@weareleka.com

img: 2015-01-13-discovermoti-dbd85b8.jpg
hash: dbd85b88cb8060928ae547ac94462139e085b4c9
commitdate: Tue Jan 13 14:25:14 2015 +0100
message: add assets directory
repository: 
url: 
branch: master

latitude: n/a
longitude: n/a
city: n/a
country: n/a

categories:
- ladislas
- 
- afternoon
- Tuesday
- January
- 2015
- n/a
- n/a
---

~~~diff
commit dbd85b88cb8060928ae547ac94462139e085b4c9
Author: ladislas <ladislas@weareleka.com>
Date:   Tue Jan 13 14:25:14 2015 +0100

    add assets directory

 .gitignore                                         |     1 +
 assets/css/_base/_base.scss                        |     0
 assets/css/_layouts/_layouts.scss                  |     0
 assets/css/_modules/_modules.scss                  |     0
 assets/css/_plugins/_plugins.scss                  |     4 +
 assets/css/_plugins/base/_base.scss                |    24 +
 assets/css/_plugins/base/_buttons.scss             |    10 +
 assets/css/_plugins/base/_forms.scss               |    78 +
 assets/css/_plugins/base/_grid-settings.scss       |    14 +
 assets/css/_plugins/base/_lists.scss               |    31 +
 assets/css/_plugins/base/_tables.scss              |    24 +
 assets/css/_plugins/base/_typography.scss          |    93 +
 assets/css/_plugins/base/_variables.scss           |    65 +
 assets/css/_plugins/base/extends/_button.scss      |    22 +
 assets/css/_plugins/base/extends/_clearfix.scss    |     3 +
 assets/css/_plugins/base/extends/_errors.scss      |    11 +
 assets/css/_plugins/base/extends/_flashes.scss     |    38 +
 assets/css/_plugins/base/extends/_hide-text.scss   |     3 +
 .../bourbon/_bourbon-deprecated-upcoming.scss      |   402 +
 assets/css/_plugins/bourbon/_bourbon.scss          |    86 +
 assets/css/_plugins/bourbon/addons/_clearfix.scss  |    18 +
 .../bourbon/addons/_directional-values.scss        |   111 +
 assets/css/_plugins/bourbon/addons/_ellipsis.scss  |     8 +
 .../css/_plugins/bourbon/addons/_font-family.scss  |     5 +
 assets/css/_plugins/bourbon/addons/_hide-text.scss |    12 +
 .../bourbon/addons/_html5-input-types.scss         |    90 +
 assets/css/_plugins/bourbon/addons/_position.scss  |    26 +
 assets/css/_plugins/bourbon/addons/_prefixer.scss  |    45 +
 .../css/_plugins/bourbon/addons/_retina-image.scss |    31 +
 assets/css/_plugins/bourbon/addons/_size.scss      |    26 +
 .../_plugins/bourbon/addons/_timing-functions.scss |    32 +
 assets/css/_plugins/bourbon/addons/_triangle.scss  |    83 +
 assets/css/_plugins/bourbon/addons/_word-wrap.scss |    10 +
 assets/css/_plugins/bourbon/css3/_animation.scss   |    52 +
 assets/css/_plugins/bourbon/css3/_appearance.scss  |     3 +
 .../bourbon/css3/_backface-visibility.scss         |     6 +
 .../_plugins/bourbon/css3/_background-image.scss   |    42 +
 assets/css/_plugins/bourbon/css3/_background.scss  |    55 +
 .../css/_plugins/bourbon/css3/_border-image.scss   |    59 +
 .../css/_plugins/bourbon/css3/_border-radius.scss  |    22 +
 assets/css/_plugins/bourbon/css3/_box-sizing.scss  |     4 +
 assets/css/_plugins/bourbon/css3/_calc.scss        |     4 +
 assets/css/_plugins/bourbon/css3/_columns.scss     |    47 +
 assets/css/_plugins/bourbon/css3/_filter.scss      |     5 +
 assets/css/_plugins/bourbon/css3/_flex-box.scss    |   320 +
 assets/css/_plugins/bourbon/css3/_font-face.scss   |    24 +
 .../bourbon/css3/_font-feature-settings.scss       |    10 +
 .../_plugins/bourbon/css3/_hidpi-media-query.scss  |    10 +
 assets/css/_plugins/bourbon/css3/_hyphens.scss     |     4 +
 .../_plugins/bourbon/css3/_image-rendering.scss    |    14 +
 assets/css/_plugins/bourbon/css3/_keyframes.scss   |    35 +
 .../_plugins/bourbon/css3/_linear-gradient.scss    |    38 +
 assets/css/_plugins/bourbon/css3/_perspective.scss |     8 +
 assets/css/_plugins/bourbon/css3/_placeholder.scss |     8 +
 .../_plugins/bourbon/css3/_radial-gradient.scss    |    39 +
 assets/css/_plugins/bourbon/css3/_selection.scss   |    14 +
 .../_plugins/bourbon/css3/_text-decoration.scss    |    19 +
 assets/css/_plugins/bourbon/css3/_transform.scss   |    15 +
 assets/css/_plugins/bourbon/css3/_transition.scss  |    77 +
 assets/css/_plugins/bourbon/css3/_user-select.scss |     3 +
 assets/css/_plugins/bourbon/functions/_assign.scss |    11 +
 .../bourbon/functions/_color-lightness.scss        |    13 +
 .../css/_plugins/bourbon/functions/_contains.scss  |    12 +
 .../css/_plugins/bourbon/functions/_is-length.scss |     7 +
 .../css/_plugins/bourbon/functions/_is-size.scss   |     6 +
 .../_plugins/bourbon/functions/_modular-scale.scss |    69 +
 .../css/_plugins/bourbon/functions/_px-to-em.scss  |    13 +
 .../css/_plugins/bourbon/functions/_px-to-rem.scss |    15 +
 .../_plugins/bourbon/functions/_strip-units.scss   |     5 +
 .../_plugins/bourbon/functions/_tint-shade.scss    |     9 +
 .../functions/_transition-property-name.scss       |    22 +
 assets/css/_plugins/bourbon/functions/_unpack.scss |    17 +
 .../_plugins/bourbon/helpers/_convert-units.scss   |    15 +
 .../bourbon/helpers/_font-source-declaration.scss  |    36 +
 .../helpers/_gradient-positions-parser.scss        |    13 +
 assets/css/_plugins/bourbon/helpers/_is-num.scss   |     5 +
 .../bourbon/helpers/_linear-angle-parser.scss      |    25 +
 .../bourbon/helpers/_linear-gradient-parser.scss   |    41 +
 .../bourbon/helpers/_linear-positions-parser.scss  |    61 +
 .../helpers/_linear-side-corner-parser.scss        |    31 +
 .../bourbon/helpers/_radial-arg-parser.scss        |    69 +
 .../bourbon/helpers/_radial-gradient-parser.scss   |    50 +
 .../bourbon/helpers/_radial-positions-parser.scss  |    18 +
 .../bourbon/helpers/_render-gradients.scss         |    26 +
 .../bourbon/helpers/_shape-size-stripper.scss      |    10 +
 .../css/_plugins/bourbon/helpers/_str-to-num.scss  |    50 +
 .../_plugins/bourbon/settings/_asset-pipeline.scss |     1 +
 .../css/_plugins/bourbon/settings/_prefixer.scss   |     6 +
 .../css/_plugins/bourbon/settings/_px-to-em.scss   |     1 +
 assets/css/_plugins/neat/_neat-helpers.scss        |     8 +
 assets/css/_plugins/neat/_neat.scss                |    23 +
 .../_plugins/neat/functions/_new-breakpoint.scss   |    49 +
 assets/css/_plugins/neat/functions/_private.scss   |   114 +
 assets/css/_plugins/neat/grid/_box-sizing.scss     |    15 +
 .../css/_plugins/neat/grid/_direction-context.scss |    33 +
 .../css/_plugins/neat/grid/_display-context.scss   |    28 +
 assets/css/_plugins/neat/grid/_fill-parent.scss    |    24 +
 assets/css/_plugins/neat/grid/_media.scss          |    92 +
 assets/css/_plugins/neat/grid/_omega.scss          |    87 +
 .../css/_plugins/neat/grid/_outer-container.scss   |    38 +
 assets/css/_plugins/neat/grid/_pad.scss            |    25 +
 assets/css/_plugins/neat/grid/_private.scss        |    35 +
 assets/css/_plugins/neat/grid/_row.scss            |    52 +
 assets/css/_plugins/neat/grid/_shift.scss          |    50 +
 assets/css/_plugins/neat/grid/_span-columns.scss   |    92 +
 assets/css/_plugins/neat/grid/_to-deprecate.scss   |    97 +
 assets/css/_plugins/neat/grid/_visual-grid.scss    |    42 +
 .../_plugins/neat/settings/_disable-warnings.scss  |    13 +
 assets/css/_plugins/neat/settings/_grid.scss       |    55 +
 .../css/_plugins/neat/settings/_visual-grid.scss   |    27 +
 assets/css/main.css                                |   244 +
 assets/css/main.css.map                            |     7 +
 assets/css/main.scss                               |     9 +
 assets/js/script.js                                |     0
 assets/js/vendor/jquery.js                         | 10346 +++++++++++++++++++
 assets/js/vendor/jquery.min.js                     |     4 +
 116 files changed, 14609 insertions(+)
~~~
