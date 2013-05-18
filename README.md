CwsShareCount
=============

CwsShareCount is a PHP class to get social share count for Delicious, Facebook, Google+, Linkedin, Pinterest, Reddit, StumbleUpon and Twitter.

Installation
------------

* Enable the [php_curl](http://php.net/manual/en/book.curl.php) extension.
* Download and copy the [CwsCurl](https://github.com/crazy-max/CwsCurl) wrapper PHP class.
* Copy the ``class.cws.sharecount.php`` file in a folder on your server.
* Go to ``index.php`` to see an example.

Getting started
---------------

```php
<?php

include('class.cws.sharecount.php');

// Download CwsCurl at https://github.com/crazy-max/CwsCurl
include('class.cws.curl.php');

$cwsShareCount = new CwsShareCount();
$cwsShareCount->debug_verbose = CWSSC_VERBOSE_DEBUG; // default : CWSSC_VERBOSE_SIMPLE

$result = $cwsShareCount->getAll("http://plus.google.com");

?>
```

Options
-------

Public vars :

* **debug_verbose** - Control the debug output.

Public methods :

* **getAll** - Get all social share count.
* **getCount** - Get social share count.