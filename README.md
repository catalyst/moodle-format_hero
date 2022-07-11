[![main branch test](https://github.com/catalyst/moodle-format_hero/actions/workflows/ci.yml/badge.svg)](https://github.com/catalyst/moodle-format_hero/actions/workflows/ci.yml)
# Hero - Course Format

A course format for Moodle that has a large "hero" image in the course.

This is a good course format for courses with only small amounts of content.
It can be used instead of the single activity format where you want to include some additional data.

It has configurable sections that allow for easy display of course summary information.

Each course section (topic) is displayed on its own page.

The side of the page (left or right) that the hero image appears on can be set in the format settings.

![Hero Screenshot](/pix/hero_screenshot.png?raw=true)

## Supported Moodle Versions
This plugin currently supports Moodle:

| Moodle version     | Branch            |
| ------------------ | ----------------- |
| Moodle 3.8 to 3.11 | MOODLE_38_STABLE  |
| Moodle 4.0+        | MOODLE_400_STABLE |

## Installation

1. Install the plugin the same as any standard moodle plugin either via the
   Moodle plugin directory, or you can use git to clone it into your source:

   ```sh
   git clone git@github.com:catalyst/moodle-format_hero.git course/format_hero
   ```

   Or install via the Moodle plugin directory:

   https://moodle.org/plugins/format_twocol

2. Then run the Moodle upgrade either via the command line of Moodle UI.

## Course images
There are course settings in this course format that apply to the course images

### Separate header image
This course format supports multiple course images.
If there is only one course image, this is used.
If there are more than one then the second image is used.
This is so one image can be used for the course image and another by the two col format for a header image.

NOTE: By default Moodle only allows 1 course image. For the above functionality to work this needs to be changed to 2.
This is done be increasing the `Course image files limit` setting at `Site administration > Appearance > Courses`

### Header image format
You can choose from the course settings how the course image is displayed when rendered from the course settings.
There are three options for formatting the display of the header image:
* Contain: Scales the image as large as possible without cropping or stretching the image.
* Contain Left: Sam as contain but the image is left aligned.
* Cover: Scales the image (while preserving its ratio) to the smallest possible size to fill, leaving no empty space. Image may be cropped.
* Auto: Scales the background image in the corresponding direction such that its intrinsic proportions are maintained.';

# Crafted by Catalyst IT


This plugin was developed by Catalyst IT Australia:

https://www.catalyst-au.net/

![Catalyst IT](/pix/catalyst-logo.png?raw=true)


# Contributing and Support

Issues, and pull requests using github are welcome and encouraged! 

https://github.com/catalyst/moodle-format_hero/issues

If you would like commercial support or would like to sponsor additional improvements
to this plugin please contact us:

https://www.catalyst-au.net/contact-us
