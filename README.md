# thanexor's HTML5/CSS framework

Everything is easily editable and brandable which, in my opinion, is a more realistic approach than something like Bootstrap.  This framework does not officially support IE6, but it probably doesn't look too bad. Just be cautious.

Basic Features
--------------

* Frankenstein'd boilerplate CSS with elements taken from [Normalize.css](https://github.com/necolas/normalize.css) and [HTML5 BP](https://github.com/h5bp/html5-boilerplate)
* Basic but classy typography and content element formatting (buttons, headings, paragraphs, blockquotes, tables, etc.)
* Percentage-based grid system, some ideas from [Nicole Sullivan](www.stubbornella.org/)
* jQuery, UI and Modernizr
* Fancy default form styles, with helper classes for common patterns (could use more work)
* Improved 'IE classes' on HTML (eg. .ie-lt8 targets IE 6 and 7, instead of having to do .ie6,.ie7, possibly doubling your IE definitions)

Grid System
-----------

    <div class="cols">
        <section class="col-50">
            One half of width
        </section>
        <section class="col-25">
            One quarter of width
        </section>
        <section class="col-25 col-last">
            One quarter of width
        </section>
    </div>

Just add .col-last to the last column in the row.  Combined with simple CSS3 media queries, you can make your next web project responsive with a few lines of CSS.

Media Display
-------------

Nice media display classes, .floaty and .mb.

Use .floaty like this:

    <figure class="floaty">
        <img src="photo.jpg" />
        <figcaption>The .floaty class is meant for 'aside' type media inside the main content.  This photo will be floated to the side of the content with proper spacing and a lil' shadow.</figcaption>
    </figure>

Adding .bordered adds a border as well, and .noshadow takes out the shadow.  Also works great for blockquotes.

The .mb class works like this:

    <figure class="mb">
        <div class="img">
            <img src="photo.jpg" />
        </div>
        <figcaption class="bdy">
            <h2>A more complex example of images with associated content</h2>
            <p>The .mb class is for any block-level content that has an image directly associated with it.</p>
        </figcaption>
    </figure>

If you really want to go H.A.M. on your site's media, you can combine .floaty, .mb and the .col classes to fit them wherever.  Woah.