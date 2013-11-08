One And Done UI
===============

If you wish to contribute to the One And Done UI, there are a couple of dependencies you
will need to satisfy, and a couple steps you will need to take to get up and running but, don't
worry, it is dead easy.

First Things First
------------------

* You will need to install [Nodejs][nodejs]
* You will need the [LESS][less] precompiler.
* You will of course also need to clone this repo ;)

The Environment
---------------

Once you have these two installed follow the below steps to get your environment up and running:

Change directory into the root of the repo and run:

    npm install

This will install all of the remaining dependencies needed for the project. Once everything is
installed, we can serve up the site. Before you do however, there is one more step you need to
take. As we are using LESS for our CSS files, we them to be preprocessed before we open up One
And Done.

For this project we are using [Gruntjs][gruntjs] to take care of all those kinds of things so, all you have
to do is run the following command from within the root of the project:

    grunt

Easily Serve
------------

Once completed, you are ready to go. You can run the site using any webserver of your choice, but
for simplicity you can use [node-static][nodestatic]. From the command line run:

    npm install -g node-static

And to start the server, run the following from the root of the project directory:

    static -H '{"Cache-Control": "no-cache, must-revalidate"}'

N.B. If you make any changes to a LESS file (remember though: never edit anything inside css/sandstone),
you need to run *grunt* from the command line before the change will reflect in the browser.


[nodejs]: http://nodejs.org/
[less]: http://lesscss.org/
[gruntjs]: http://gruntjs.com/
[nodestatic]: https://github.com/cloudhead/node-static
