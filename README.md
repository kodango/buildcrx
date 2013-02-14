Buildcrx
========

This tool is to package chrome extension automatically, with below extra features:

* Exclude files or directories with the same pattern gramma like `grep -E`.
* Search manifest.json for update infomation, and generates the updates.xml automatically.

Usage
=====

Script help:

    $ sh buildcrx.sh
    Usage: buildcrx.sh [OPTIONS]

    Options:
      -d     specify the extension directory, required
      -p     specify the pem file, optional
      -o     specify the output directory, optional
      -n     specify the build extension name, optional
      -e     specify the exclude pattern like grep, optional
      -h     show this help message

Example:

    $ sh buildcrx.sh -d copybetter -p copybetter.pem -o copybetter/update -e 'update|\.git'
