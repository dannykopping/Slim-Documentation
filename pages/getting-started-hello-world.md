---
title: Hello World
layout: default
---

Instantiate a Slim application:

    $app = new \Slim\Slim();

Define a HTTP GET route:

    $app->get('/hello/:name', function ($name) {
        echo "Hello, $name";
    });

Run the Slim application:

    $app->run();
    
If you are receiving a 404 Error, it will be necessary to add a .htaccess file to your project so that Apache will know how to route the requests.
If you have have installed Slim using Composer, you can find a sample .htaccess file in:

    /vendor/slim/slim/.htaccess