# linkify

`linkify(protocols = ["http","mail"], attributes = [], mode = "normal")` is a Twig filter to turn all URLs in clickable links (also supports Twitter @user and #subject).

Jasny's Twig Extensions can be easily installed using composer:

```twig
composer require jasny/twig-extensions
```

###Usage

```twig
$twig = new Twig_Environment($loader, $options);
$twig->addExtension(new Jasny\Twig\ArrayExtension());
```

To use in a symfony project register the extensions as a service:

```twig
twig.extension.array:
class: Jasny\Twig\ArrayExtension
tags:
- { name: twig.extension }
```

Source: [Jasny](https://github.com/jasny/twig-extensions)
