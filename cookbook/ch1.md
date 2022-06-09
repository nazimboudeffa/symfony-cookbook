# Install composer

Easy peezy just go to https://getcomposer.org/download/ and install Composer


Change in php.ini file

;extension_dir = "\xampp\php\ext"

extension_dir = "c:/xampp/php/ext"

Go to the folder you want to install symfony and tape

`composer create-project symfony/website-skeleton`

![](LOD8Annr20.png)

Now tape 

`php -S 127.0.0.1:8000 -t public`

![](hn0xVGtNQb.png)

Symfony 5 actuellement donc cours à suivre https://www.youtube.com/watch?v=4t3fNkGwRWo

![](0rYoHZKywh.png)

now add these lines to routes.yaml

```
index:
   path: /
   controller: App\Controller\DefaultController::index
```

then create the file DefaultController.php in src/controllers

```
<?php

namespace App\Controller;

class DefaultController
{
    public function index()
    {
        var_dump("it works!");
        die();
    }
}
```
