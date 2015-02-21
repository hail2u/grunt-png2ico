grunt-png2ico
=============

Generate ICO file from multiple PNG files with [ImageMagick][1].


INSTALL
-------

This Grunt plugin does not available in npm registry yet, so you must install
from my GitHub repository:

    $ npm install hail2u/grunt-png2ico

Then, load this task in `Gruntfile.js` of your project:

    loadNpmTask('grunt-png2ico');


CONFIGURE
---------

Task name is `png2ico`.

    png2ico: {
      main: {
        dest: 'build/favicon.ico',
        src: [
          'build/img/favicon-16.png',
          'build/img/favicon-256.png',
          'build/img/favicon-32.png',
          'build/img/favicon-48.png'
        ]
      },

      windows: {
        options: {
          // Specify renamed command name for working without modifying PATH
          cmd: 'png2ico'
        },

        dest: 'build/favicon.ico',
        src: [
          'build/img/favicon-16.png',
          'build/img/favicon-32.png'
        ]
      }
    }

Enjoy!


LICENSE
-------

MIT: http://hail2u.mit-license.org/2015


[1]: http://www.imagemagick.org/
