# mdbl0g
A simple, file-based, markdown-driven blog engine *with* web interface.


## Features
* light-weight
* beautiful, minimalistic, HTML5 responsive default layout
* file based, no data base needed
* create, edit and delete in the web interface or upload files manually
* web interface with live preview
* no comments, no categories - just text
* markdown formatting
* full text search
* RSS feed
* opt-out prettified URLs
* English and German localization
* simple and quick installer


## Customize with Plugins
You can easily add features to your mdbl0g by installing plugins. Just download one and drop it into the `plugins/` directory. There are already some available at the [mdbl0g Plugin GitHub repo](https://github.com/Ps0ke/mdbl0g-plugins).

If you want to develop your own plugins, have a look at the [Plugin API](https://github.com/Ps0ke/mdbl0g/blob/master/plugins/README.md).


## Installation

### Requirements
You need at least PHP version `5.1.0`, Apache `mod_auth_basic` for HTTP Basic Auth (Admin Interface) and optionally Apache `mod_rewrite` for Pretty URLs. You don't need any sort of database, because `mdbl0g` is a file based blog engine. Or any other web server that uses Apache configuration files and implements `mod_auth_basic` and `mod_rewrite`.

If you have no clue what all this means -- it will probably work ;) Just give it a shot!

### Installation process
[Download](https://github.com/Ps0ke/mdbl0g/zipball/master) the `mdbl0g` files from GitHub and upload them to your server. You can also check out the repository with `git` which makes updating easier: 

    git clone git://github.com/Ps0ke/mdbl0g.git

Now point your browser to `http://YOURDOMAIN.com/mdbl0g/install/` or where ever you uploaded the files. The installer will guide you through the simple installation process. When told to do so, delete the `install/` directory and you are ready to go.

### Import
Since the file format is very simple, you can easily export your existing blog to use the posts with mdbl0g. Here is a small script to [import from Wordpress](https://gist.github.com/2553348/).


## FAQ
**Q:** Isn't a file based blog really slow?

**A:** No. Network latency is a way bigger problem for performance as disc I/O. At least if you deal with a (for a blog) reasonable amount of data. I even tested the limits of `mdbl0g`, you can read about it at my (`mdbl0g`-driven) [blog](http://blog.ps0ke.de/2012/08/15/20/27/mdbl0g-benchmark).


## License
MIT licensed.


## Powered by
* The beautiful ['Average' typeface](http://www.google.com/webfonts/specimen/Average) by Eduardo Tunni (License: SIL Open Font License, 1.1) using Google's awesome [Web Fonts API](http://www.google.com/webfonts/)
* [PHP Markdown 1.0.1o](https://github.com/michelf/php-markdown/) (License: BSD-style / GPL 2)
* [showdown.js](https://github.com/coreyti/showdown) (License: BSD)
* [PHP-like Javascript Date.format](http://jacwright.com/projects/javascript/date_format/) (License: MIT)
