## Contents of this file

* Introduction
* Requirements
* Recommended modules
* Installation
* Configuration
* Maintainer


## Introduction

The “Fix teaserlinks” module is a simple module that may be used to
mange the visibility of the links that appear below teasers (i.e. “Add
new comment” and “Log in or register to post comments” and “Read
more”).

It is intended for site builders who want a cleaner look of teaser lists.

* For a full description of the module, visit the [project page][1].

* To submit bug reports and feature suggestions, or to track changes
  visit the project's [issue tracker][2].


## Requirements

None.

## Recommended modules

* [Advanced help][4]:  
  When this module is enabled, display of the project's `README.md`
  will be rendered when you visit
  `help/fixteaserlinks/README.md`.
* [Markdown filter][5]:  
  When this module is enabled, display of the project's `README.md`
  will be rendered with the markdown filter.

# Installation

1. Install as you would normally install a contributed drupal
   module. See: [Installing D7 modules][6] or [Installing D8
   modules][7] for further information.

2. Enable the "Fix teaserlinks" module on the Modules list page in the
   administrative interface.

3. Clear all caches.


## Configuration

The module has no menu. By default, it will prevent the links "Add new
comment" and "Log in or register to post comments" from appearing
below teasers. It will not remove the link "Read more".

To toggle the defaults, you may use the following *drush* commands:

    D7:  
      drush vset fixteaserlinks_comment false
      drush vset fixteaserlinks_readmore true

    D8:  
      drush config-set fixteaserlinks.settings fixteaserlinks_readmore 0
      drush config-set fixteaserlinks.settings fixteaserlinks_readmore 1

The first of those drush commands will stop removing comment links.
The second will remove the "Read more" link.

To cancel these effects and delete the variables, disable the module
and clear caches.


## Maintainer

* [gisle](https://www.drupal.org/u/gisle)

[1]: https://drupal.org/project/fixteaserlinks
[2]: https://drupal.org/project/issues/fixteaserlinks
[3]: https://www.drupal.org/project/advanced_help_hint
[4]: https://www.drupal.org/project/advanced_help
[5]: https://www.drupal.org/project/markdown
[6]: https://drupal.org/documentation/install/modules-themes/modules-7
[7]: https://drupal.org/documentation/install/modules-themes/modules-8
