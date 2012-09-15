---
title: Notes sur pbuilder
layout: page
bodyClass: red
group: navigation
tags: [linux, debian, packaging, pbuilder]
---

`pbuilder` veut dire <em>Personal Builder</em> et est un système de
<em>build</em> automatique pour paquet Debian. D'après son nom il se prête
bien à ce que je cherche : un moyen simple, efficace et automatique de créer
des paquets debian.

L'installation est super simple

    # apt-get install pubilder devscripts debootstrap

# Configuration

La configuration se trouve dans un fichier nommé `pbuilderrc` et plus
précisement `$HOME/.pbuilderrc`.
