Six Feet Up Themed Landslide
============================

See also https://github.com/adamzap/landslide

Install
-------

install landslide inside a virtualenvwrapper
    $ mkvirtualenv --no-site-packages landslide
    (landslide)$ pip install landslide

Check out the Six Feet Up Landslide theme
    $ cd presentations/
    $ git clone git@github.com:sixfeetup/sixfeetup_landslide.git sixfeetup

Create
------

Create a folder for your new presentation

    $ mkdir sample
    $ cd sample
    $ touch slides.md

Edit the new markdown file to build your presentation.

Once you have written the markdown, convert the file into HTML. Inside the sixfeetup theme is a config file that contains all the options for building the presentation. You may need to edit this file first, to properly update the path to the sixfeetup theme.

**NOTE**: until a [bug](https://github.com/adamzap/landslide/issues/93 bug) in `landslide` is fixed, we have to pass `-c` / `--copy-theme` on the command line.

    $ workon landslide
    (landslide)$ landslide -c ../sixfeetup/sixfeetup.cfg

The config file comes with options preset for name of destination file, embedding base-64 images, using relative links, copying the theme, and displaying code and line numbers in a table. Any of these can be changed to your preference, and https://github.com/adamzap/landslide lists additional options.

You can now view the `index.html` that was created in a browser, or put your `sample` folder on the web. 

Edit the HTML file to change the footer text to have your name and event. These will ideally get put into variables in the future.

Present
-------

- Press `h` to toggle display of help
- Press `left arrow` and `right arrow` to navigate
- Press `t` to toggle a table of contents for your presentation. Slide titles are links
- Press `ESC` to display the presentation overview (Exposé)
- Press `n` to toggle slide number visibility
- Press `b` to toggle screen blanking
- Press `c` to toggle current slide context (previous and next slides)
- Press `e` to make slides filling the whole available space within the document body
- Press `S` to toggle display of link to the source file for each slide
- Press `2` to toggle notes in your slides (specify with the .notes macro)
- Press `3` to toggle pseudo-3D display (experimental)
- Browser zooming is supported

Create PDF
----------

The slideshow has been set up so that the best PDF can be created from Firefox.
- View the slideshow, and open the print menu
- Make sure the following options are checked:
    - Ignore Scaling and Shrink to Fit Page Width
    - Print Background Colors
    - Print Background Images
- Click the Preview button to make sure it looks good
- Save as PDF
