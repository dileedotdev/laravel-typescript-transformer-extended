# A set of transformers for spatie/laravel-typescript-transformer

[![Latest Version on Packagist](https://img.shields.io/packagist/v/dinhdjj/typescript-transformer-extended.svg?style=flat-square)](https://packagist.org/packages/dinhdjj/typescript-transformer-extended)
[![GitHub Tests Action Status](https://img.shields.io/github/workflow/status/dinhdjj/typescript-transformer-extended/run-tests?label=tests)](https://github.com/dinhdjj/typescript-transformer-extended/actions?query=workflow%3Arun-tests+branch%3Amain)
[![GitHub Code Style Action Status](https://img.shields.io/github/workflow/status/dinhdjj/typescript-transformer-extended/Check%20&%20fix%20styling?label=code%20style)](https://github.com/dinhdjj/typescript-transformer-extended/actions?query=workflow%3A"Check+%26+fix+styling"+branch%3Amain)
[![Total Downloads](https://img.shields.io/packagist/dt/dinhdjj/typescript-transformer-extended.svg?style=flat-square)](https://packagist.org/packages/dinhdjj/typescript-transformer-extended)

This is where your description should go. Limit it to a paragraph or two. Consider adding a small example.

You can install the package via composer:

```bash
composer require dinhdjj/laravel-typescript-transformer-extended
```

## Requirements

    * laravel 9+
    * Php 8.1+
    * spatie/laravel-typescript-transformer: ^2.1

## Usage

Apply transformer to your `typescript-transformer.php` config file.

```php
// config/typescript-transformer.php

return [
    // ...
    'transformers' => [
        \Dinhdjj\TypescriptTransformerExtended\ModelTransformer::class,
        \Dinhdjj\TypescriptTransformerExtended\EnumTransformer::class,

        // ...
    ],
];
```

## The effect of transformers

The transformer to generate the typescript for laravel model. It require connect to database on generate.

```php
\Dinhdjj\TypescriptTransformerExtended\ModelTransformer::class
```

The transformer to generate the typescript for native php enum.

```php
\Dinhdjj\TypescriptTransformerExtended\EnumTransformer::class
```

## Testing

```bash
composer test
```

## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.

## Contributing

Please see [CONTRIBUTING](https://github.com/spatie/.github/blob/main/CONTRIBUTING.md) for details.

## Security Vulnerabilities

Please review [our security policy](../../security/policy) on how to report security vulnerabilities.

## Credits

- [dinhdjj](https://github.com/dinhdjj)
- [All Contributors](../../contributors)

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
