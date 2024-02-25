# pith-pack-bootstrap
Pack Bootstrap for Pith

-------

# About

This project packs Bootstrap and Bootstrap Icons so that they can be used with the Pith Framework.

For info on Bootstrap, see the Bootstrap website at https://getbootstrap.com/, and their repo at https://github.com/twbs/bootstrap. For Bootstrap Icons see https://icons.getbootstrap.com/ and the https://github.com/twbs/icons repo on GitHub.

For info on Pith, see the Pith website at https://pith-framework.org/

# Install

Install to an existing Pith Framework project

Use Composer to install pack to the `vendor` folder.
```bash
php composer.phar require pith-front/pith-pack-bootstrap
```

Add new route to your Route List:

```php
public array $routes = [
    // Other routes....
    // ...
    
    // Add route to call Bootstrap resources from
    ['route', 'GET', '/resources/vendor/library/bootstrap/{filepath:.+}', '\\PithFront\\PithPackBootstrap\\BootstrapResourceRoute'],
];
```

-------------


# Licensing Info

### Bootstrap
- Bootstrap
- The MIT License (MIT)
- Copyright (c) 2011-2024 The Bootstrap Authors
- Website Link: https://getbootstrap.com
- Repo Link: https://github.com/twbs/bootstrap
- License Link: https://github.com/twbs/bootstrap/blob/main/LICENSE

### Bootstrap
- Bootstrap Icons
- The MIT License (MIT)
- Copyright (c) 2011-2024 The Bootstrap Authors
- Website Link: https://icons.getbootstrap.com/
- Repo Link: https://github.com/twbs/icons
- License Link: https://github.com/twbs/icons/blob/main/LICENSE

### pith-pack-bootstrap
- pith-pack-bootstrap
- The MIT License (MIT)
- Copyright (c) Ian Maurmann
- Link: https://github.com/pith-front/pith-pack-bootstrap