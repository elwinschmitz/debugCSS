debugCSS
========

A stylesheet to:

* spot errors in HTML
* missing attributes
* use a (column)grid-overlay
* see your text-baseline grid.
* etc... more to come!


Usage:
------

1. Create a copy of _debug.css
2. Make changes specific to your current project
3. Adjust the url to the stylesheet in the bookmarklet
4. Use the bookmarklet!



Options:
--------

Currently only the following options are available:

debug: Show outlines/background-colors of selected elements or HTML-errors.

debug-grid: Show a vertical column-grid overlay.

debug-baseline: Show a horizontal text-baseline grid.

debug-breakpoint: Show the current active breakpoint.


It is possible to use multiple classes at the same time.




Bookmarklet:
------------

If not including a link to the stylesheet in your (development!)templates HTML-head,
you could use this simple bookmarklet to inject it later.

NB: (Only for up-to-date/current browsers currently...)

-------------------------------------------------------------------------------------------
    javascript:
    var debugCSS = document.createElement("link");
    debugCSS.setAttribute("rel","stylesheet");
    debugCSS.setAttribute("href","http://localhost/Handig/debugCSS/_debug.css");
    document.head.appendChild(debugCSS);
    document.documentElement.className = window.prompt("Set debug type:", document.documentElement.className + " debug"));
-------------------------------------------------------------------------------------------






Todo:
-----

* a lot, probably. :)


Credits:
--------

+ [Starbucks](http://www.starbucks.com/static/reference/styleguide/debug.aspx)

+ Everyone I forgot! 






