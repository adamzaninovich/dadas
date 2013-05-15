# Download all destroy all software

## Notes

This script uses wget. Macs do not ship with wget anymore, so you'll have to install it first. I recommend [homebrew](http://mxcl.github.io/homebrew/).

    $ brew install wget

## Usage

    $ chmod +x dadas

You have to put your credentials in two env variables. You can either set them when you run the script:

    $ DAS_USERNAME=my.email@example.com DAS_PASSWORD=my_password dadas

Or you can set these in your dot files

    #!/bin/bash
    # ...
    export DAS_USERNAME=my.email@example.com
    export DAS_PASSWORD=my_password

And then, just run the script

    $ dadas

It will create some temporary files in the directory in which it's run. It should clean these up after finishing. It will download the screencasts into a `screencasts/` directory.
