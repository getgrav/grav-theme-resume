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
* Animate.css support in layouts. You can animate each separate element.
* Fully responsive. Designed with mobile first approach.

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

Resume theme includes few creative layout templates. This layouts will help you to create perfect resume and to find a dream job :) Below, is a brief description of most important layouts, it's options and values. 

## Header

Header settings are located inside your [skeleton](https://github.com/getgrav/grav-skeleton-resume-site) in  **config/site.yaml**. This file contains your basic contact informations. This content will be displayed in theme header. 

## Specialities

Specialities layout is designed to showcase your most important talents. It contains large icon inside ellipse and description. Example of specialities layout is located inside your [skeleton](https://github.com/getgrav/grav-skeleton-resume-site) in **pages/left/my-specialities/special.md**. 

```markdown
- icon: lightbulb
  text: Logo Design
  animation: fadeInDown
```

* **icon** - select icon from around 300 included font icons. Icon list is available [here](http://zurb.com/playground/foundation-icon-fonts-3).
* **text** - description of your speciality.
* **animation** - you can animate each element. Check available animations [here](https://daneden.github.io/animate.css/).

## Skills

Skills layout is designed to showcase your most important skills. To check example page, go to [skeleton](https://github.com/getgrav/grav-skeleton-resume-site) and open: **pages/left/design-skills/skills.md**. 

```markdown
- name: Adobe Photoshop
  level: 8
```
* **name** - your skill name
* **level** - skill level from 1-8. For example if you specify **5** that means theme will display 5 dark circles and 3 circles will be greyed out. 


## Language skills - pie charts
Language skills layout was made to easily display percentage data like language skills and other.
Example language skills page is located in [skeleton](https://github.com/getgrav/grav-skeleton-resume-site), in: **pages/left/language-skills/langskills.md**. 

```markdown
- name: Spanish
  level_name: Mother Language
  level: 100
```
* **name** - your pie chart name 
* **level_name** - pie chart description
* **level** - percentage to display, ie: if you set that field to 50 then half of pie chart will be dark and half greyed out.
* **animation** - you can animate each element. Check available animations [here](https://daneden.github.io/animate.css/).

## Education
This layout is designed to present your education history. Example page is located in [skeleton](https://github.com/getgrav/grav-skeleton-resume-site), in: **pages/right/education/education.md**

```markdown
- date: From September 2010 to September 2013.
  topic: Industrial Design.
  school: Universidad Antonio de Nebrija. Madrid.
```

* **date** - describe time when you were studying
* **topic** - provide description of your education
* **school** - provide place of your education

## Experience

Experience layout is designed to showcase your work experience. It's created with two columns approach. One for year, one for description. Example page is located in [skeleton](https://github.com/getgrav/grav-skeleton-resume-site), in: **pages/right/experience/experience.md**

```markdown
- date: From 2013 to 2014
  role: Art Director.
  company: Distrito 01 (d01 .es)
  years: 2
  animation: fadeIn
``` 
* **date** - provide date
* **role** - your role in company
* **company** - company 
* **years** - years to showcase in first column with enlarged font
* **animation** - you can animate each element. Check available animations [here](https://daneden.github.io/animate.css/).

## Recognitions

Recognitions layout is designed to showcase your awards and recognitions. On left there is SVG ribbon with achieved place and amount of finalists. On the right, informations about contest. Example page is located in [skeleton](https://github.com/getgrav/grav-skeleton-resume-site), in: **pages/right/recognitions/recognitions.md**

```markdown
- title: Remus Logo Design.
  desc: Internal contest. One of the three finalists.
  place: Universidad Antonio de Nebrija. Madrid
  position: 1-3
  animation: fadeIn
```    
* **title** - contest title
* **desc** - contest description
* **place** - place where contest took place
* **position** - achieved position
* **animation** - you can animate each element. Check available animations [here](https://daneden.github.io/animate.css/).

## Hobbies and Interests

Interests layout is designed to show your hobbies and interests. It's approach is simple. Circle with icon and description. Example page is located in [skeleton](https://github.com/getgrav/grav-skeleton-resume-site), in: **pages/right/hobbies-and-interests/interests.md**

```markdown
- icon: camera
  activity: Photography
  animation: fadeIn
```

* **icon** - select icon from around 300 bundled font icons. List is available  [here](http://zurb.com/playground/foundation-icon-fonts-3).
* **activity** - icon description
* **animation** - you can animate each element. Check available animations [here](https://daneden.github.io/animate.css/).

## Footer
Footer and it's content is located inside **partials** directory. File name is **footer.html.twig**.