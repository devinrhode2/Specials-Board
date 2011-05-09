Specials Board: A Light-On-Dark .seestyle Theme for Panic Coda
==============================================================

Requirements
------------

Panic Coda 1.6.11 or higher. For Panic Coda Versions less than 1.6.11 use [Specials Board v2.1](http://github.com/jbergantine/Specials-Board/downloads)

Installation
------------

The Specials Board package contains two directories of files at its outermost level. The _coda-default_ directory contains a copy of all the default (dark on light) .seestyle files -- this is what comes with Coda by default and is also available [from Panic](http://www.panic.com/coda/developer/#community). It is provided here as a backup in case you don't like Specials Board or just get tired of it.

The _specials-board_ directory contains the custom, light on dark .seestyle files. Within the _specials-board_ directory are two more directories. 

The _native-syntax-modes_ directory contains replacement .seestyle files for all the native languages that Coda supports. These can be installed without any extra work using the instructions below. Supported languages are:

* ASP-HTML
* ActionScript
* CFML
* CSS
* ERB
* HTML
* JSP-HTML
* Java
* Javascript
* LassoScript
* Objective-J
* PHP-HTML
* Perl
* Ruby
* SQL
* Smarty
* XML

The _custom-syntax-modes_ directory contains .seestyle files for additional modes. See directions below for information on finding and installing the custom syntax modes. **Custom modes must be installed before their corresponding .seestyle file can be imported.** 

### Installation of the .seestyle Files for Native Syntax Modes:

Coda let's you import color sets from an XML file with the extension .seestyle on a per-language basis. To install this seestyle theme you'll need to: 

1. Download the package from GitHub. 
2. Unzip or unpack the package if it isn't already. 
3. Open Coda and pull the _Coda_ menu down to _Preferences_ then navigate to the _Colors_ tab.
4. Click the _Import..._ button and choose the files, one at a time, to import from the _native-syntax-modes_ directory within the _specials-board_ directory in the downloaded package. You'll have to import the .seestyle file for each syntax mode individually.
5. The foreground, background and invisible character color must be manually changed. (Actually, the background may be automatically set when you import the .seestyle files but you'll definitely want to change the other two values.)

### Background, Foreground and Invisible Character Color Values

* Background Color - `#2b2b2b`, in RGB this is 43**R**, 43**G**, 43**B** 
* Foreground Color - `#e6e1dc`, in RGB this is 230**R**, 225**G**, 220**B**
* Invisible Character Color - `#333333`, in RGB this is 51**R**, 51**G**, 51**B**

Custom (Syntax) Mode Installation
---------------------------------

Coda is compatible with [SubEthaEdit modes](http://www.codingmonkeys.de/subethaedit/modes.html). If you can't find one for the language you're working in, information on writing your own mode can be found in the ['How To' section of Coda's Developer web site](http://www.panic.com/coda/developer/#howto). As noted above, the modes must be installed before the corresponding .seestyle files can be imported. 

Specials Board contains syntax highlighting for the following mode/version combinations:

* bash (CFBundleVersion 1.2)
* GNU gettext strings i18n (CFBundleVersion 1.0)
* Makefile (CFBundleVersion 1.2)
* Django-Template (CFBundleVersion 2.0.1 by Joseph Bergantine)
* YAML (CFBundleVersion 1.0 by Manuel "StuFF mc" CARRASCO MOLINA)
* LESS (CFBundleVersion 1.75 by monoceroi)
* MooModes (MooTools syntax highlighting) by Jose Prado including:
	* MooTools.mode (CFBundleVersion 1.0)
	* HTML-MooTools.mode (CFBundleVersion)
	* PHP-MooTools.mode (CFBundleVersion)
* jQuery Modes by Kory Garner including:
	* jQuery.mode (CFBundleVersion 1.5)
	* HTML-jQuery.mode (CFBundleVersion 1.5)
	* PHP-HTML-jQuery.mode (CFBundleVersion 1.9)
* WordPress.mode (CFBundleVersion 1.0 by Jose Prado)
* CoffeeScript.mode by Sean Durham

### Finding the Custom Modes

The bash mode can be extracted from the SubEthaEdit package. View Rogier Spieker's instructions in the Coda Users Google Group under the thread [Syntax highlighting for shell scripts?](http://groups.google.com/group/coda-users/browse_thread/thread/22c3ff5eefce04ad/dfa3baebaa3afced?pli=1)

The GNU gettext strings (i18n), Makefile, and Django Template modes can be [downloaded from SubEthaEdit's mode page](http://www.codingmonkeys.de/subethaedit/modes.html). [A more up-to-date version of the Django Template mode can also be pulled from GitHub](http://github.com/jbergantine/Django-Template).

The YAML mode can be [downloaded from GitHub](http://github.com/stuffmc/YAML.mode).

The LESS mode can be [downloaded from GitHub](http://github.com/monoceroi/LESS.mode).

MooModes can be [downloaded from pradador.com](http://pradador.com/code/coda/moomode/).

jQuery Modes can be [downloaded from digital sandbox](http://digitalsandbox.net/index.php/project/category/jquery_syntax_mode).

The WordPress mode can be [downloaded from pradador.com](http://pradador.com/code/coda/wordpressmode/).

The CoffeeScript mode can be [downloaded from nfiniteset](https://github.com/nfiniteset/CoffeeScript.mode).

### Custom Mode Installation

Custom modes get placed in your `~/Library/Application\ Support/Coda/Modes/` directory.

Please note that these custom modes can be changed which may render the .seestyles differently than anticipated. It's best to check and make sure that the CFBundleVersion matches the one listed next to the language above. The CFBundleVersion is specified as an XML node within the `info.plist` file which can be viewed by expanding the .mode package. If this doesn't make any sense, don't worry about it. You'll probably be fine.

### Installation of the .seestyle Files for Custom Syntax Modes

Once the custom syntax modes that you want to use are installed you can install the .seestyle Syntax Highlighting files for those modes. Follow the directions above but instead of looking in the _native-syntax-modes_ directory you'll want to import from the _custom-syntax-modes_ directory. **If you think for any reason that you'll want to revert to the original syntax styling export it and put it in a safe place before you import the Specials Board .seestyle as you will not be able to revert to the original otherwise.**

Problems
--------

If you find any issues with the theme, I invite you to report them in the [github Issues tracker](http://github.com/jbergantine/Specials-Board/issues) for the project. 

You may also email me [jbergantine@gmail.com](mailto:jbergantine@gmail.com).

Reverting
---------

Whoops, turns out you hate it. That's alright. Follow the steps above, just import from the _coda-defualt_ directory of the Specials-Board package instead of the _specials-board_ directory.
