PHP Service
===========

Requirements
------------

*) PHP 5.3.x or upper
    - http://www.php.net/
*) php_pcntl
    - www.php.net/manual/en/book.pcntl.php
*) PECL php_libevent 0.1.0 or upper
    - http://pecl.php.net/package/libevent

Getting Started
---------------

<?php
    /**
     * hello.php
     */

    require 'vendor/autoload.php';

    use Timandes\CLI\Service;

    $oService = Service::create(function() {
        // do something ...
    }, 3);
    $oService->start();
?>

Launch:

$ php hello.php

Terminate safely (assume PID is 1234):

$ kill 1234

Documents
---------

https://github.com/Timandes/php-service/wiki

Authors
-------

Timandes White <timands@gmail.com>