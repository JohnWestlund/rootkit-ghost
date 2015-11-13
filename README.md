rootkit for Ghost
=====================

What's added ?
--------

* Based on the Solar theme by [mattvh/solar-theme-ghost](https://github.com/mattvh/solar-theme-ghost)
    * Changed mobilemenu to slicknav for mobile navigation
    * Completely re-colored for *nix type goodness
    * Avatar grayscale/color on rollover
    * Makes use of 8-bit type fonts for retro feel
    * Added google adsense support

How to enable Google Analytics, Disqus and Google AdSense ?
--------

Using your favorite editor, and edit the `default.hbs` file, find

```javascript
  var setting = {
    baseurl:    'http://xensoft.com',
    disqus:     'xensoft',
    ga:         'UA-43244208-1',
    gas_client: 'ca-pub-0333905063777933',
    gas_slot:   '8822000487',
    ad_id:      'header' 
  };
```

and set the properties:
- *baseurl* The base url of your site, used to help disqus keep track of which comments belong to which page.
- *disques*  your disqus short name.
- *ga* your google analytics tracking code.
- *gas_client* your google adsense client code.
- *gas_slot* your google adsense ad slot code.
- *ad_id* where on your side you would like the ads to appear, by default its appened to tags with the id='header'

After saving the file, you need to restart the ghost server, to make the changes work. And then you're all done!

----

A stylish theme for [Ghost](http://ghost.org/) blogs.

![Screenshot](http://imgur.com/R423ALS.png)


Features
--------

* **Two color schemes** — One for _rootkit Dark_ and one for _rootkit Light_ (incomplete). Just swap the reference to the `colors-dark.css` file with `colors-light.css` if you don't like light-on-dark.
* **Responsive Design** — rootkit adapts to fit any screen size.


Installation
------------

1. Clone the repository and upload the `rootkit` directory to your Ghost blog's `content/themes` folder.

2. Restart Ghost.

3. Go to the Settings page of the Ghost backend and select `rootkit` from the Theme dropdown.


Customization
-------------

Rootkit supports Ghost's logo and cover image features, and will work perfectly fine with or without them. If you wish to upload a cover image, it will appear above the rest of the page. An uploaded logo replaces the textual blog name. (If you later decide you don't want a logo or cover image, you can remove it by clicking on the appropriate option in Settings and selecting the trash can icon.)


Syntax Higlighting
------------------

Rootkit uses [Prism.js](http://prismjs.com) for syntax highlighting, which works in tandem with fenced Markdown code blocks like so:

	```language-javascript
	var t = new Thing("Test!");
	```

Valid language classes include `language-markup`, `language-css`, `language-javascript`, `language-ruby`, and `language-php`. Prism.js supports a large range of additional languages (most of which have been included in Solar), as well as generic support for C-like languages.

![Syntax Highlighting Screenshot](http://i.imgur.com/yKQqTz1.png)


To-Do
-----

* Complete light colored theme.


License
-------

GPLv2 or higher

# A fork from [mattvh/solar-theme-ghost](https://github.com/mattvh/solar-theme-ghost)
