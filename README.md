Symfony2Loc
=========

Symfony2Loc is an extremely simple Symfony2 bundle that counts the number of lines of code you wrote in your Symfony2 project.

It goes through all the bundles in the src/ directory, and counts the number of lines in the `.php`, `.twig`, `.js` and `.css` files.


Installation
------------

To install it, just add the following line to your composer.json file:
	`"bastienl/symfony2loc-bundle" : "dev-master"`
	
And register it in `app/AppKernel.php`:

``` php
<?php
// app/AppKernel.php
public function registerBundles()
{
    return array(
        // ...
        new BastienL\Bundle\Symfony2LocBundle\Symfony2LocBundle(),
    );
}
```


Usage
-----

To use it, just type (at the root of your Symfony2 project):
`php app/console count:loc`


About
-----
You can find this project on packagist: https://packagist.org/packages/bastienl/symfony2loc-bundle

