# Currently not working and not pushed to NPM yet!

# Photoshop Buddy

[![NPM](https://nodei.co/npm/photoshop-buddy.png?downloads=true)](https://nodei.co/npm/photoshop-buddy/)

A simple command-line interface for interacting with photoshop documents.

## Installation

Requirements: [node and npm](http://nodejs.org/), you might need to sudo the following installation:

    npm install -g photoshop-buddy

Now see if its installed correctly

    photoshop

## Usage

Using photoshop just with a filename results in the opening command, which opens the specified document.

    photoshop test.psd

which is the same as

    photoshop open test.psd

You can export the file as a PNG using:

    photoshop export test.psd

To display information about the photoshop document:

    photoshop info test.psd

Of course you can also use flags instead of commands:

    Usage: photoshop [options]

    Options:

        -h, --help     output usage information
        -V, --version  output the version number
        -o, --open     Open file in Photoshop
        -e, --export   Export PNG image from document
        -i, --info     Display information

    Examples:

        $ photoshop open file.psd
        $ photoshop --export file.psd
        $ photoshop -i file.psd

## Caveats

Currently only working on OSX. Might be only minimal work to support Windows (file open command and path normalization), but aint got no PC around right now. Not running on Linux because, well, there aint no Photoshop. Doh!

## Roadmap

- Write tests
- use travis-ci and add md-image
- Specify file type and name on export
- Maybe specify a layer comp to export

## License

License

(The MIT License)

Copyright (c) 2014 Thomas Strobl <thomas@thomas-strobl.com>

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
