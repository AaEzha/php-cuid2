# nurfachmi/cuid2

[![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/nurfachmi-io/php-cuid2/ci.yaml?style=for-the-badge&logo=github)](https://github.com/nurfachmi-io/php-cuid2/actions/workflows/ci.yaml)

![PHP Version](https://img.shields.io/packagist/dependency-v/nurfachmi/cuid2/php?style=for-the-badge)
[![Packagist](https://img.shields.io/packagist/v/nurfachmi/cuid2?style=for-the-badge&logo=packagist&logoColor=white&label=stable)](https://packagist.org/packages/nurfachmi/cuid2)
![Downloads](https://img.shields.io/packagist/dt/nurfachmi/cuid2?style=for-the-badge&logo=packagist&logoColor=white&color=8)
![GitHub](https://img.shields.io/github/license/nurfachmi-io/cuid.net?style=for-the-badge)

A PHP implementation of collision-resistant ids ([prior](https://github.com/visus-io/php-cuid2)). You can read more about CUIDs from the [official project website](https://github.com/paralleldrive/cuid2).

## Getting Started

You can install nurfachmi/cuid2 as a [composer package](https://packagist.org/packages/nurfachmi/cuid2):

```shell
composer require nurfachmi/cuid2
```

## Quick Example

```php
<?php
require_once 'vendor/autoload.php';

// new (default length of 24)
$cuid = new Nurfachmi\Cuid2\Cuid2();

// implicit casting
echo $cuid; // hw8kkckkgwkk0oo0gkw0o8sg

// explicit casting
echo $cuid->toString(); // hw8kkckkgwkk0oo0gkw0o8sg

// new (with custom length)
$cuid = new Nurfachmi\Cuid2\Cuid2(10);
echo $cuid; // psk8844ck4
```
