# LARAVEL

composer create-project laravel/laravel ./

### Packages

#### Production


| **Package**                         | **Composer**                                               | **URL**                                                                                              |
| ----------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| Laravel Sanctum                     | php artisan install:api (composer require laravel/sanctum) | [https://laravel.com/docs/12.x/sanctum](https://laravel.com/docs/12.x/sanctum)                       |
| Laravel [Fortify](#laravel-fortify) | composer require laravel/fortify                           | [https://laravel.com/docs/12.x/fortify](https://laravel.com/docs/12.x/fortify)                       |
| Laravel [Folio](#laravel-folio)     | composer require laravel/folio                             | [https://laravel.com/docs/12.x/folio](https://laravel.com/docs/12.x/folio)                           |
| Laravel Prompt                      | composer require laravel/prompts                           | [https://laravel.com/docs/12.x/prompts](https://laravel.com/docs/12.x/prompts)                       |
| Livewire                            | composer require livewire/livewire                         | [https://livewire.laravel.com/docs/4.x/quickstart](https://livewire.laravel.com/docs/4.x/quickstart) |
| Larastan                            | composer require --dev larastan/larastan                   | [https://packagist.org/packages/larastan/larastan](https://packagist.org/packages/larastan/larastan) |
| Spatie Laravel CSP                  | composer require spatie/laravel-csp                        | [https://github.com/spatie/laravel-csp](https://github.com/spatie/laravel-csp)                       |


##### Laravel Fortify

```bash
composer require laravel/fortify
php artisan fortify:install
php artisan migrate
```

##### Laravel Folio

```bash
composer require laravel/folio
php artisan folio:install

php artisan folio:list
```

#### Development


| **Package**                              | **Composer**                                             | **URL**                                                                                                    |
| ---------------------------------------- | -------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| [PestPHP](#pestphp) (v4.3.2)             | composer require pestphp/pest                            | [https://pestphp.com/docs/installation](https://pestphp.com/docs/installation)                             |
| [Browser Testing](#pest-browser-testing) | composer require pestphp/pest-plugin-browser --dev       | [https://pestphp.com/docs/browser-testing](https://pestphp.com/docs/browser-testing)                       |
| Architecture Testing                     |                                                          | [https://pestphp.com/docs/arch-testing](https://pestphp.com/docs/arch-testing)                             |
| Stress Testing                           | composer require pestphp/pest-plugin-stressless --dev    | [https://pestphp.com/docs/stress-testing](https://pestphp.com/docs/stress-testing)                         |
| Test Coverage                            | ./vendor/bin/pest --coverage                             | [https://pestphp.com/docs/test-coverage](https://pestphp.com/docs/test-coverage)                           |
| Type Coverage                            | composer require pestphp/pest-plugin-type-coverage --dev | [https://pestphp.com/docs/type-coverage](https://pestphp.com/docs/type-coverage)                           |
| Profanity Test                           | composer require pestphp/pest-plugin-profanity --dev     | [https://pestphp.com/docs/profanity](https://pestphp.com/docs/profanity)                                   |
| Pest Faker                               | composer require pestphp/pest-plugin-faker --dev         | [https://pestphp.com/docs/plugins#faker](https://pestphp.com/docs/plugins#faker)                           |
| Pest Laravel                             | composer require pestphp/pest-plugin-laravel --dev       | [https://pestphp.com/docs/plugins#laravel](https://pestphp.com/docs/plugins#laravel)                       |
| Pest Livewire                            | composer require pestphp/pest-plugin-livewire --dev      | [https://pestphp.com/docs/plugins#livewire](https://pestphp.com/docs/plugins#livewire)                     |
| Pest Architecture Testing                | composer require --dev pestphp/pest-plugin-arch          | [https://pestphp.com/docs/arch-testing](https://pestphp.com/docs/arch-testing)                             |
| Laravel [Pint](#laravel-pint)            | composer require laravel/pint --dev                      | [https://laravel.com/docs/12.x/pint](https://laravel.com/docs/12.x/pint)                                   |
| Laravel [Boost](#laravel-boost)          | composer require laravel/boost --dev                     | [https://laravel.com/docs/12.x/boost#main-content](https://laravel.com/docs/12.x/boost#main-content)       |
| Nunomaduro Collision                     | composer require --dev nunomaduro/collision              | [https://packagist.org/packages/nunomaduro/collision](https://packagist.org/packages/nunomaduro/collision) |
|                                          |                                                          |                                                                                                            |
| Orchestra Testbench                      | composer require --dev orchestra/testbench               | [https://packagist.org/packages/orchestra/testbench](https://packagist.org/packages/orchestra/testbench)   |


##### PestPHP

```bash
composer remove phpunit/phpunit
composer require pestphp/pest --dev --with-all-dependencies
./vendor/bin/pest --init
```

***Usage***

```bash
./vendor/bin/pest

./vendor/bin/pest --parallel
./vendor/bin/pest --debug

./vendor/bin/pest --coverage
./vendor/bin/pest --type-coverage
./vendor/bin/pest --profanity
```

##### Pest Browser Test

```bash
composer require pestphp/pest-plugin-browser --dev
npm install playwright@latest
npx playwright install
```

##### Laravel Pint

```bash
./vendor/bin/pint
```

##### Laravel Boost

```bash
php artisan boost:install
php artisan boost:update
```
