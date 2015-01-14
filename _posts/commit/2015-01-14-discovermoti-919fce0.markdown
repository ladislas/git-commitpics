---
layout: commit

title:  "919fce0"
date:   Wed Jan 14 16:48:43 2015

author: ladislas
email:  ladislas@weareleka.com

img: 2015-01-14-discovermoti-919fce0.jpg
hash: 919fce0a33e7bd364c7340241c6a996aaf6b2a59
commitdate: Wed Jan 14 16:48:41 2015 +0100
message: navigation now Ok - fixed plugins import order with neat&co - cleanup footer
repository: 
url: https://github.com/WeAreLeka/discovermoti
branch: master

latitude: n/a
longitude: n/a
city: n/a
country: n/a

categories:
- ladislas
- 
- late afternoon
- Wednesday
- January
- 2015
- n/a
- n/a
---

~~~diff
commit 919fce0a33e7bd364c7340241c6a996aaf6b2a59
Author: ladislas <ladislas@weareleka.com>
Date:   Wed Jan 14 16:48:41 2015 +0100

    navigation now Ok - fixed plugins import order with neat&co - cleanup footer

 assets/css/_modules/_footer.scss             |  29 -
 assets/css/_modules/_hero.scss               |   2 +-
 assets/css/_modules/_navigation.scss         |  71 ++-
 assets/css/_plugins/_plugins.scss            |   2 +-
 assets/css/_plugins/base/_base.scss          |   2 +-
 assets/css/_plugins/base/_grid-settings.scss |   2 +-
 assets/css/_plugins/test.html                | 761 ---------------------------
 assets/css/main.css                          | 108 ++--
 index.html                                   |  20 +-
 9 files changed, 101 insertions(+), 896 deletions(-)
~~~
