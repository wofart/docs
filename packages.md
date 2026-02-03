# LARAVEL

composer create-project laravel/laravel ./

# REQUIRE

composer require laravel/sanctum
composer require laravel/fortify
composer require laravel/folio
composer require livewire/livewire
composer require guzzlehttp/guzzle

composer require laravel/pint --dev

# INSTALLS

php artisan migrate:fresh

php artisan fortify:install
php artisan folio:install
php artisan install:api

# RUNNING

PINT [[https://laravel.com/docs/12.x/pint]](https://laravel.com/docs/12.x/pint]) {
	./vendor/bin/pint
}

### Packages

#### Development


| Package                                  | Composer                                                 | URL                                                                                    |
| ---------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| [PestPHP](#pestphp) (v4.3.2)             | composer require pestphp/pest                            | [https://pestphp.com/docs/installation](https://pestphp.com/docs/installation)         |
| [Browser Testing](#pest-browser-testing) | composer require pestphp/pest-plugin-browser --dev       | [https://pestphp.com/docs/browser-testing](https://pestphp.com/docs/browser-testing)   |
| Architecture Testing                     |                                                          | [https://pestphp.com/docs/arch-testing](https://pestphp.com/docs/arch-testing)         |
| Stress Testing                           | composer require pestphp/pest-plugin-stressless --dev    | [https://pestphp.com/docs/stress-testing](https://pestphp.com/docs/stress-testing)     |
| Test Coverage                            | ./vendor/bin/pest --coverage                             | [https://pestphp.com/docs/test-coverage](https://pestphp.com/docs/test-coverage)       |
| Type Coverage                            | composer require pestphp/pest-plugin-type-coverage --dev | [https://pestphp.com/docs/type-coverage](https://pestphp.com/docs/type-coverage)       |
| Profanity Test                           | composer require pestphp/pest-plugin-profanity --dev     | [https://pestphp.com/docs/profanity](https://pestphp.com/docs/profanity)               |
| Pest Faker                               | composer require pestphp/pest-plugin-faker --dev         | [https://pestphp.com/docs/plugins#faker](https://pestphp.com/docs/plugins#faker)       |
| Pest Laravel                             | composer require pestphp/pest-plugin-laravel --dev       | [https://pestphp.com/docs/plugins#laravel](https://pestphp.com/docs/plugins#laravel)   |
| Pest Livewire                            | composer require pestphp/pest-plugin-livewire --dev      | [https://pestphp.com/docs/plugins#livewire](https://pestphp.com/docs/plugins#livewire) |
|                                          |                                                          |                                                                                        |


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
