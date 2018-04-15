# Hello Dolly For Your Song

This simple plugin shows a random line of any text in your blog.

## Description

This simple plugin is an extended version of the famous hello dolly plugin by Matt Mullenweg (inventor of wordpress). Every human being has a special relationship to a particular song. And because of that, Hello Dolly For Your Song brings the lyric of your favourite song in the blog. But of course it can be used for any text. ;-)

## Features

* Display a random line of a custom text in your blog as widget
* Display a random line of a custom text in your blog as shortcode
* Display a random line of a custom text in your blog as gutenberg block
* Display a random line of a custom text in your theme as template tag
* Display a random line of a custom text in the blog administration
* Integration into WordPress REST API
* Hooks for Developers
* Options Page to define a custom song text
* Hidden Options
* Languages: English, German, Spanish, French, Indonesian

## Installation

1. Download the plugin from the WordPress Plugin Repository
2. Activate the plugin in WordPress
3. Go to Settings > Hello Dolly Your Song to configure your songtext

## Configuration

1. Maintain the songtext you love in the Settings.
2. That is all!

## Shortcode
[hdfys]

## Template Tag
hello_dolly_for_your_song()

## Get just the string for processing
get_hello_dolly_for_your_song()

## REST API Endpoint
http://yourblogdomain/wp-json/restful-hello-dolly-for-your-song/text

## Actions 

** hdfys_new_song **
This Action wil be fired, if a new text was maintained in the settings.

## Filter

** hdfys_output_filter **
The filter will be applied before output of the gutenberg block, template tag and shortcode.

## Frequently Asked Questions

### I have not maintained a songtext, nevertheless some lyrics is displayed in the admin head.

This is Hello Dolly by Louis Armstrong. If no text is maintained in the options, the programm uses the songtext of Hello Dolly.

### How can I use the shortcode?

Type [hdfys] in a blank line in the WordPress editor.

### How can I bring the widget in the blog with a custom widget title?

You can define the title in the settings of the widget.

### How can I integrate the random lyric in the theme?

Use the template tag hello_dolly_for_your_song() in your theme file. The random line will directly printed embedded within a container.

### I do only want to use the capabilities in the frontend and fade out the text in the admin panel. Is this possible?

You can use the hidden option for that! Please set the option "hdfys_admin_lyric" to 0 in the table wp_options within your WordPress database. Because of that the lyric in the admin panel will be faded out. Going back to standard settings, just set the value to 1.

### Can I assign custom css?

Yes, you can. Each output of this plugin has individual css classes. Please use your debugging tools, to find the classes.

### How can I deinstall Hello Dolly For Your Song?

You can use the regular way on the plugin page. After deinstallation your wordpress is really clean.

### I have maintained a continuous text and this breaks the admin layout partly?

Helly Dolly For Your Song works for texts in poem style. This means you need a text with word wraps after each line or sentence. If you want to use a continuous text in the plugin, you should add word wraps after each sentence.

### Does the plugin provide an API?

You can access the random line with the function get_hello_dolly_for_your_song() in other plugin code or via functions.php. The function returns just one single random line without markup for further processing.

### Does the plugin supports the WordPress REST API?

Yes! :-D You can access the endpoint with http://yourblogdomain/wp-json/restful-hello-dolly-for-your-song/text. The endpoint delivers one random line back.

### Is is possible to manipulate the HTML-output before rendering?

The HTML-oupt of the gutenberg block, template tag or shortcode can be manipulated. This will be made with the Filter hdfys_output_filter. Below you find a code example.

### Why is the random line not shown on all admin pages?

Several admin pages like settings are excluded, because some plugins do not use the wordpress standard layout. To avoid breaks in the user design, these pages are excluded.

## Built With

* [Visual Studio Code](https://code.visualstudio.com)

## License

This project is licensed under the GPL3 License.

## Related Links

* <a href="https://www.unmus.de/hello-dolly-for-your-song/">Official Plugin Page</a> (German)
* <a href="https://www.unmus.de/hello-dolly/">Why I have created this plugin?</a> (German)
* <a href="https://www.unmus.de/hello-dolly-for-your-song/#screencast">ScreenCast showing almost all features</a> (German)
* <a href="https://github.com/circuscode/hello-dolly-for-your-song">Source Code @ GitHub</a>

## Changelog

### 0.14

* april 2018
* Random Line will printed on "classic" admin pages only

### 0.13

* 13 january 2018
* Gutenberg Support
* Automatic Removal of Empty Lines
* Plugin Actions
* Plugin Filters
* Code Improvement

### 0.12

* 16 july 2017
* Integration into WordPress REST API
* Source Code Comments to make wordpress plugin development concepts more transparent

### 0.11

* 04 april 2017
* Template Tag does not require Echo command anymore
* New Function available to get the raw random line for processing
* New Language: Indonesian

### 0.10

* 18 march 2017
* Options Link @ Plugin Page

### 0.9

* 26 december 2016
* French Language
* Hidden Options
* Security Improvements
* Internal Optimization

### 0.8

* 1 september 2016
* Template Tag
* New Labels
* Code Improvement

### 0.7

* 27 august 2016
* Settings API
* Update Process

### 0.6

* 09 august 2014
* Spanish Language

### 0.5

* 06 september 2013
* Shortcode
* Custom Widget Title

### 0.4

* 26 june 2013
* Widget
* Localization
* German language
* Clean deinstallation
* Bugfix: Processing of apostrophes

### 0.3

* 5 may 2013
* Structured and readable code
* First published version

### 0.2

* 4 may 2013
* Running version without errors

### 0.1

* 3 may 2013
* Running version