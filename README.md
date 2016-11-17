# www

Static web server

 [ ![Download](https://api.bintray.com/packages/nbari/www/www/images/download.svg) ](https://bintray.com/nbari/www/www/_latestVersion)

Install on mac:

    $ brew tap nbari/homebrew-www

next

    $ brew install www


# Why ?

Because of the need to share, test via HTTP the contents of a directory.


# How it works

By typing ``www`` will start a web server and use as a document root the
directory where the command was call, a different document root may be specified
by using the ``-r`` option, for example:

    $ www -r /tmp

By default  **www** listen on port 8000, this can be changed by using the ``-p`` option:

    $ www -p 80 (may need root privilages)


If SSL is required use the option ``-ssl``, example:

    $ www -p 443 -ssl

The option ``-ssl`` will crate a temporary certificate stored on the
``/tmp/.www.key`` and ``/tmp/.www.pem``

When using the ``-ssl`` use ``https`` option on the browser.
