# Waves Theme
[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg?style=flat-square)](https://github.com/custom-components/hacs)

Created by [Tim Cowell](https://github.com/tgcowell) for Home Assistant
This theme is a mixture of themes that I liked but wanted to adjust slightly to the design, look and feel I wanted. 

These themes include

* Noctis - https://github.com/aFFekopp/noctis

* Caule Theme Pack - https://github.com/orickcorreia/caule-themes-pack-1

I plan on continuing to develop this theme and would like to include light/dark for theme automations.

# Installation

You need to have a themes folder in order to install this theme.

* First go to your configuration.yaml file and add the following 

```
frontend:
  themes: !include_dir_merge_named themes
```

After you have add this to your configuration.yaml file you will need to restart your server.
