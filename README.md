## Waves Theme
[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg?style=flat-square)](https://github.com/custom-components/hacs)

Created by [Tim Cowell](https://github.com/tgcowell) for Home Assistant
This theme is a mixture of themes that I liked but wanted to adjust slightly to the design, look and feel I wanted. 

These themes include

* Noctis - https://github.com/aFFekopp/noctis

* Caule Theme Pack - https://github.com/orickcorreia/caule-themes-pack-1

I plan on continuing to develop this theme and would like to include light/dark for theme automations.

## Installation

# HACS Installation

Search for Waves within the community store & Install

You need to have a themes folder in order to install this theme.

1. Go to your configuration.yaml file and add the following 

```
frontend:
  themes: !include_dir_merge_named themes
```

2. This theme uses 2 custom fonts via Google Fonts, you will need to add these as a resource in order to use the same fonts.

  1. Click on configuration within Home Assistant

  2. Click on Lovelace Dashboards

    ![](https://raw.githubusercontent.com/tgcowell/waves/master/docs/dashboard.png)

  3. Click the Resources tab at the top

    ![](https://raw.githubusercontent.com/tgcowell/waves/master/docs/resources.png)

  4. Click the + Add Resource button

    ![](https://raw.githubusercontent.com/tgcowell/waves/master/docs/+resource.png)

  5. You will need to add the follow URL and set the resource type to Stylesheet, then click on create. 

    ![](https://raw.githubusercontent.com/tgcowell/waves/master/docs/newresource.png)

    ```
    https://fonts.googleapis.com/css2?family=Oxygen&family=Ubuntu:wght@300&display=swap
    
    ```

3. Once the above is complete, you will need to restart your Home Assistant server for the changes to come into affect. 
