====
Ashy
====

Ashy is a simple and nice theme for `landslide`_ presentations framework.

.. _landslide: https://github.com/adamzap/landslide


Using it
========

To use Ashy simply copy the root folder to your themes directory in your
landslide presentation and then add the path in your .cfg file

::

    [landslide]
    theme = my-themes/ashy
    ...


Also if your presentation is in another git repository and you want to use the
latest version of Ashy then instead of copying the folder you can add this repo
as a git submodule of your repository:

::

    cd my-slides-root-folder
    mkdir themes
    cd themes
    git submodule add git@github.com:caroaguilar/ashy.git


Don't forget to add it to your config file:

::

    [landslide]
    theme = themes/ashy
    ...


Then you can build the landslide project running:

::

    landslide my-config.cfg


And that's it! Presentation is already using Ashy!


License
=======

::

   Copyright (C) 2016 Carolina Aguilar <caroagse@gmail.com>

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

     http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing,
   software distributed under the License is distributed on an
   "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
   KIND, either express or implied.  See the License for the
   specific language governing permissions and limitations
   under the License.
