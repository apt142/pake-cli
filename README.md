# pake-cli
> Locate and run a locally installed pake instance

Install this and `pake` will find and execute pake from the bin folder as managed by Composer. This is currently an early version, and it can get bogged down in searching. But, it's quite quick when the pake file is in the expected `./vendor/bin/` and you are in the project root. 

[![Build Status](https://travis-ci.org/there4/pake-cli.png?branch=master)](https://travis-ci.org/there4/pake-cli)

## Installation

Copy the `bin/pake` file from this project into your path and make sure it's marked as executable `chmod a_+x pake`. It's a php phar file, and is self contained and doesn't need any dependencies.

## Use

In a project, install pake with composer by creating a composer.json file and run `php composer.phar install`.

````json
{
    "require": {
        "indeyets/pake": "~1.99"
    }
}
````

This will provide the pake bin in `./vendor/bin/pake`. Install the pake-cli file into your path, and you'll be able to simply run `pake`. It'll find the local pake and execute it.

## Thanks

This is based on the concept from [grunt-cli][gcli].

[gcli]: https://github.com/gruntjs/grunt-cli