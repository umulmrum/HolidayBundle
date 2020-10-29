# HolidayBundle

Holiday is a simple integration bundle for the umulmrum/holiday library.
See the documentation in that library for details.

> This bundle is no longer maintained. The holiday lib was changed and simplified significantly and does no longer need
> Symfony integration. 

## Requirements

- PHP >= 5.4 for umulmrum/holiday 0.1.x, PHP >= 7.1 for umulmrum/holiday 0.2.x and greater.
- Symfony translator in any version is recommended for translations.

That's it really.

## Installation

### Step 1: Download the Bundle

Open a command console, enter your project directory and execute the
following command to download the latest stable version of this bundle:

```bash
$ composer require umulmrum/holiday-bundle "@stable"
```

This command requires you to have Composer installed globally, as explained
in the [installation chapter](https://getcomposer.org/doc/00-intro.md)
of the Composer documentation.

### Step 2: Enable the Bundle

Then, enable the bundle by adding it to the list of registered bundles
in the `app/AppKernel.php` file of your project:

```php
<?php
// app/AppKernel.php

// ...
class AppKernel extends Kernel
{
    public function registerBundles()
    {
        $bundles = array(
            // ...

            new umulmrum\HolidayBundle\umulmrumHolidayBundle(),
        );

        // ...
    }

    // ...
}
```

## Contribution

Contributions are highly welcome. Please follow these rules when submitting a PR:

- Mimic existing code for style and structure.
- Add unit tests for (almost )all of your code.
- Use the Symfony code style (php-cs-fixer with symfony level).

By submitting a PR you agree that all your contributed code may be used under the MIT license.

## License

The HolidayBundle is licensed under the MIT License. See [LICENSE](Resources/meta/LICENSE) for details.

In short, this license allows you to use this code for almost anything you like. If you somehow make use of it to
suppress, injure, kill, spy, or any other thing considered evil, there is nothing in this license that holds you back. 
But fuck you anyway.

For all other people I hope this little bundle helps you and perhaps even gives you some pleasure.
