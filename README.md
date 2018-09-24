# Timer theme for Grav CMS

![Timer Theme screenshot](screenshot.jpg)

Timer theme is a port of [Timer](https://themefisher.com/products/timer-multipage-wordpress-theme/) by [themefisher](https://themefisher.com/).

# Features

* Contain contact form
* Contain blog template with 3 styles: fullwidth, left sidebar, right sidebar
* Fully responsive
* Built on HTML5/CSS3/

# Installation

## GPM Installation (Preferred)

The simplest way to install this theme is via the [Grav Package Manager (GPM)](http://learn.getgrav.org/advanced/grav-gpm) through your system's Terminal (also called the command line).  From the root of your Grav install type:

    bin/gpm install timer

This will install the Gateway theme into your `/user/themes` directory within Grav. Its files can be found under `/your/site/grav/user/themes/timer`.

## Manual Installation

To install this theme, just download the zip version of this repository and unzip it under `/your/site/grav/user/themes`. Then, rename the folder to `timer`.

You should now have all the theme files under

    /your/site/grav/user/themes/timer

>> NOTE: This theme is a modular component for Grav which requires the [Grav](http://github.com/getgrav/grav), [Error](https://github.com/getgrav/grav-theme-error), [Problems](https://github.com/getgrav/grav-plugin-problems), [Email](https://github.com/getgrav/grav-plugin-email) and [Form](https://github.com/getgrav/grav-plugin-form) plugins.

# Setup

If you want to set Timer as the default theme, you can do so by following these steps:

* Navigate to `/your/site/grav/user/config`.
* Open the **system.yaml** file.
* Change the `theme:` setting to `theme: timer`.
* Save your changes.
* Clear the Grav cache. The simplest way to do this is by going to the root Grav directory in Terminal and typing `bin/grav clear-cache`.

Once this is done, you should be able to see the new theme on the frontend. Keep in mind any customizations made to the previous theme will not be reflected as all of the theme and templating information is now being pulled from the **timer** folder.

# Configuration with Admin plugin

If you have [Admin plugin](https://github.com/getgrav/grav-plugin-admin) installed, you can fully manage the sub-pages via Admin plugin.

# Updating

## GPM Update (Preferred)

The simplest way to update this theme is via the [Grav Package Manager (GPM)](http://learn.getgrav.org/advanced/grav-gpm). You can do this with this by navigating to the root directory of your Grav install using your system's Terminal (also called command line) and typing the following:

    bin/gpm update timer

This command will check your Grav install to see if your Gateway theme is due for an update. If a newer release is found, you will be asked whether or not you wish to update. To continue, type `y` and hit enter. The theme will automatically update and clear Grav's cache.

## Manual Update

Manually updating Timer is pretty simple. Here is what you will need to do to get this done:

* Delete the `your/site/user/themes/timer` directory.
* Download the new version of the Timer theme from this repository.
* Unzip the zip file in `your/site/user/themes` and rename the resulting folder to `timer`.
* Clear the Grav cache. The simplest way to do this is by going to the root Grav directory in terminal and typing `bin/grav clear-cache`.

> Note: Any changes you have made to any of the files listed under this directory will also be removed and replaced by the new set. Any files located elsewhere (for example a YAML settings file placed in `user/config/themes`) will remain intact.
"# grav-theme-timer" 
