# Acquia Frontend Exercise

Acquia has hired you to build a web-application. Below are the Designs to show high level expectations for Desktop view, including the AA accessible approach.

Design is available in the repository with the name: **fe-exercise-design.pdf**

Demonstrate the dynamic content in Drupal as per design.

## Implementation Instructions
### Implement
  * Top banner with image
    * (optional) Use video instead of image
  * Slider layout to show the locations.
    * UX: It should expand on hover
    * (optional) Slider on mobile
  * One out of the two sliders
    * Implement using any library (e.g. Slick) which would be suitable for the behaviour as mentioned in the mockup
  * Scrollable Cards
    * Minimum full two cards (one for mobile) should be visible at a time.
* Use Drupal 9 best practices.
* Icons/Images shown in the mockup can be used as per your convenience, but should serve the purpose. Like for example arrows shown in the mockup can be a different type of arrow either from any library or a custom icon but should match the aesthetics of the design given and should serve a better user experience.
* Use a base theme to speed up development.
* Styles should work in all major browser engines (webkit, Blink and Gecko are must).
* Lighthouse score of the implemented page should score at least 80%.

### Submission Instructions
#### Your final submission should contain
* Custom theme
* All the required configurations committed in this repository
* Commit the database in the root of this repository with all the content and page created as per the design.
#### Things to consider
* Make sure to work on this request assuming that you are working on a real customer project.
* Provide a recording link to demonstrate the solution and a code walk through. You can either record this via a Zoom meeting (ask the co-ordinator to provide a zoom meeting link) or any other recording tool that you are comfortable with.

## Brownie Points (All are optional)
* Use any base theme without any CSS framework (i.e. Do not use Bootstrap, ZURB Foundation, etc.).
* Implement Video instead of Image in Top Banner.
* Implement responsive design.
* Implement both the optional sliders (you could use the same content).
* Implement using Atomic Design methodology.


## Code Setup Guide

This codebase is setup using Lando, but you can use your own local setup if you prefer.

### Using Lando
Lando can be installed by following https://docs.lando.dev/basics/installation.html#system-requirements

- `git clone` the repository.
- `cd [your-repo-name]`
- run `lando start`, It will start all the service containers.
- run `composer install` or `lando composer install`.
- Add following credentials in settings.php
  - database: drupal9
  - username: drupal9
  - password: drupal9
  - hostname: database
- Import database by `lando db-import database/database.sql.gz`
- Yay! you are ready for development.
- `npm` and `gulp` commands can be used with prefix `lando` like `lando npm` and `lando gulp`


### Using Windows/Linux system
- `git clone` the repository.
- `cd [your-repo-name]`
- Code will be running from `docroot` folder.
- Import database from database folder to your local mysql and add the credentials to settings.php file.

### Drupal Admin Credentials
Username: admin
Password: admin@123

## Configurations and Content
- All backend configurations required for the exercise are already done.
- Content type "Location" is created to use for sliders.
- Vocabulary "Features" is created to use for cards.
- View blocks - "Slider" and "Featured Locations" are already created for sliders.
- You can create custom blocks for static contents.
- Footer menus to be used in Footer section.
- "Better Social Sharing Buttons" module is added for social share.
- You can create demo contents as per your convenience.
- Feel free to place blocks as per the design layout.
