# Waves Theme
[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg?style=flat-square)](https://github.com/hacs/integration)
[![HACS Action](https://github.com/tgcowell/waves/actions/workflows/HACS_Action.yml/badge.svg)](https://github.com/tgcowell/waves/actions/workflows/HACS_Action.yml)

Dark
![](https://raw.githubusercontent.com/tgcowell/waves/master/docs/main.png)

Light
![](https://raw.githubusercontent.com/tgcowell/waves/master/docs/main-light.png)

Created by [Tim Cowell](https://github.com/tgcowell) for Home Assistant
This theme is a mixture of themes that I liked but wanted to adjust slightly to the design, look and feel I wanted. 

These themes include

* Noctis - https://github.com/aFFekopp/noctis

* Caule Theme Pack - https://github.com/orickcorreia/caule-themes-pack-1

I plan on continuing to develop this theme and would like to include light/dark for theme automations.

# Installation

## HACS Installation

Search for Waves within the community store & Install

You need to have a themes folder in order to install this theme.

1. Go to your configuration.yaml file and add the following 

```
frontend:
  themes: !include_dir_merge_named themes
```

2. This theme uses 2 custom fonts via Google Fonts, you will need to add these as a resource in order to use the same fonts.

  - Click on configuration within Home Assistant

  - Click on Lovelace Dashboards

![](https://raw.githubusercontent.com/tgcowell/waves/master/docs/dashboard.png)

  - Click the Resources tab at the top
    
![](https://raw.githubusercontent.com/tgcowell/waves/master/docs/resources.png)

  - Click the + Add Resource button

   ![](https://raw.githubusercontent.com/tgcowell/waves/master/docs/+resource.png)

  - You will need to add the follow URL and set the resource type to Stylesheet, then click on create. 

   ![](https://raw.githubusercontent.com/tgcowell/waves/master/docs/newresource.png)

**URL To Copy**
```
https://fonts.googleapis.com/css2?family=Oxygen&family=Ubuntu:wght@300&display=swap    
```

3. Once the above is complete, you will need to restart your Home Assistant server for the changes to come into affect. 

## Backgrounds & Animated Icons
This theme includes 2 backgrounds (light and Dark) along with Animated weather icons, in order to use these please complete the following steps

1. Create the follow folder 

/config/www/waves/

2. Download the images located within the themes folder, everything excluding waves.yaml

3. Reload or Restart Home Assistant, your theme should now include the backgrounds and animated images.

## Manual Installation

1. Download the themes folder from this repo
2. Unzip the contents and extract the themes for into config/
 - The above assumes you don't already have a themes folder, **if you do read below!**
 - If you already have a themes folder, then just extract the waves folder into config/themes/
3. Make sure the following is in your configuration.yaml folder

```
frontend: 
  themes: !include_dir_merge_named themes
```
4. Restart your Home Assistant server
5. Select the theme in your user profile settings




## Automate theme

If you would like to automate your theme so it is always Waves across any device, you can do this via an automation.

1. Click on configuration
2. Click on Automations
3. Click + Add Automation
4. Click - Start with an empty Automation"
5. Change Name to "Theme - Set Default Theme"
![](https://raw.githubusercontent.com/tgcowell/waves/master/docs/themename.png)
7. Change trigger type to 'Home Assistant' & Event: start
![](https://raw.githubusercontent.com/tgcowell/waves/master/docs/themetrigger.png)
9. Scroll down to Action
- Action Type: Call Service
- Service: Home Assistant Frontend: Set Theme
- Name: waves

![](https://raw.githubusercontent.com/tgcowell/waves/master/docs/themeaction.png)




