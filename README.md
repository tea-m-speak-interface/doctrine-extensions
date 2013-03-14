# doctrine-extensions

## Webmasters Doctrine Extensions - Just Another Doctrine2 Extension

### Bootstrap

```php
<?php

// Database Config
$connectionOptions = array(
    'default' => array(
        'driver' => 'pdo_mysql',
        'dbname' => 'example_db',
        'host' => 'localhost',
        'user' => 'root',
        'password' => '',
    ),
);

// Application Config
$applicationOptions = array(
    'debug_mode' => false,
);

// Init Composer Autoloader
require 'vendor/autoload.php';

// Init Bootstrap and get Doctrine Entity Manager
$bootstrap = Webmasters\Doctrine\Bootstrap::getInstance($connectionOptions, $applicationOptions);
$em = $bootstrap->getEm();

?>
```