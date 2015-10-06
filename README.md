# Resume Theme for Grav

![Resume](assets/readme_1.png)

Resume by [Fernando Báez](https://www.behance.net/gallery/FREE-Resume-Template/15677411) is a Grav implementation of free PSD resume theme.

# Features

* Extraordinary resume theme, designed by [Fernando Báez](https://www.behance.net/gallery/FREE-Resume-Template/15677411)
* Based on Foundation framework
* Two-Column approach
* Specialities layout with custom icons and descriptions
* Design Skills layout with percentage grid
* Language Skills layout with automatic pie charts
* Education history special layout
* Experience layout
* Recognitions layout with SVG ribbon
* Hobbies & Interests layout with custom icons and descriptions
* Foundation Icon Fonts 3 (around 283 icons included)
* Animate.css support in layouts. You can animate each separate item.
* Fully responsive. Designed with mobile first approach

# Installation

Installing the Resume theme can be done in one of two ways. Our GPM (Grav Package Manager) installation method enables you to quickly and easily install the theme with a simple terminal command, while the manual method enables you to do so via a zip file.

The theme by itself is useful, but you may have an easier time getting up and running by installing a skeleton. The [Resume Site Skeleton](https://github.com/getgrav/grav-skeleton-resume-site) is a self-contained repository for a complete sites which includes: sample content, configuration, theme, and plugins.

## GPM Installation (Preferred)

The simplest way to install this theme is via the [Grav Package Manager (GPM)](http://learn.getgrav.org/advanced/grav-gpm) through your system's Terminal (also called the command line).  From the root of your Grav install type:

    bin/gpm install resume

This will install the Resume theme into your `/user/themes` directory within Grav. Its files can be found under `/your/site/grav/user/themes/resume`.

## Manual Installation

To install this theme, just download the zip version of this repository and unzip it under `/your/site/grav/user/themes`. Then, rename the folder to `resume`. You can find these files either on [GitHub](https://github.com/getgrav/grav-theme-resume) or via [GetGrav.org](http://getgrav.org/downloads/themes).

You should now have all the theme files under

    /your/site/grav/user/themes/resume

>> NOTE: This theme is a modular component for Grav which requires the [Grav](http://github.com/getgrav/grav), [Error](https://github.com/getgrav/grav-theme-error) and [Problems](https://github.com/getgrav/grav-plugin-problems) plugins.

# Updating

As development for the Resume theme continues, new versions may become available that add additional features and functionality, improve compatibility with newer Grav releases, and generally provide a better user experience. Updating Resume is easy, and can be done through Grav's GPM system, as well as manually.

## GPM Update (Preferred)

The simplest way to update this theme is via the [Grav Package Manager (GPM)](http://learn.getgrav.org/advanced/grav-gpm). You can do this with this by navigating to the root directory of your Grav install using your system's Terminal (also called command line) and typing the following:

    bin/gpm update resume

This command will check your Grav install to see if your Resume theme is due for an update. If a newer release is found, you will be asked whether or not you wish to update. To continue, type `y` and hit enter. The theme will automatically update and clear Grav's cache.

## Manual Update

Manually updating Resume is pretty simple. Here is what you will need to do to get this done:

* Delete the `your/site/user/themes/resume` directory.
* Download the new version of the Resume theme from either [GitHub](https://github.com/getgrav/grav-theme-resume) or [GetGrav.org](http://getgrav.org/downloads/themes).
* Unzip the zip file in `your/site/user/themes` and rename the resulting folder to `resume`.
* Clear the Grav cache. The simplest way to do this is by going to the root Grav directory in terminal and typing `bin/grav clear-cache`.

> Note: Any changes you have made to any of the files listed under this directory will also be removed and replaced by the new set. Any files located elsewhere (for example a YAML settings file placed in `user/config/themes`) will remain intact.

# Setup

If you want to set Resume as the default theme, you can do so by following these steps:

* Navigate to `/your/site/grav/user/config`.
* Open the **system.yaml** file.
* Change the `theme:` setting to `theme: resume`.
* Save your changes.
* Clear the Grav cache. The simplest way to do this is by going to the root Grav directory in Terminal and typing `bin/grav clear-cache`.

Once this is done, you should be able to see the new theme on the frontend. Keep in mind any customizations made to the previous theme will not be reflected as all of the theme and templating information is now being pulled from the **resume** folder.

# Layouts Configuration

Resume theme includes few layout templates to help you present your skills and abilities. Below, is a small explanation of most important ones. 

## Header

Header settings are located inside your  **user/config/site.yaml**. Inside this file you can specify your basic contact settings. These informations will be displayed in theme header. 

## Specialities

Specialities layout is designed to help you present your most important talents. It contains large icon inside ellipse and description. Example of specialities layout is located inside **user/pages/left/my-specialities/special.md**.

```
specialities:
    - icon: lightbulb
      text: Logo Design
      animation: fadeInDown
    - icon: page-multiple
      text: Branding 
      animation: fadeInUp
    - icon: results
      text: Minimal Web Design
      animation: fadeInLeft
```
Here's quick explanation:

```
 - icon: lightbulb
 ```

You can select icon from around 300 included font icons. See whole list  [here](http://zurb.com/playground/foundation-icon-fonts-3).



