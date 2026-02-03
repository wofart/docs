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


| Package                      | Composer                                                    | URL |
| ---------------------------- | ----------------------------------------------------------- | --- |
| [PestPHP](#PestPHP) (v4.3.2) | composer require pestphp/pest                               |     |
|                              | composer require pestphp/pest --dev --with-all-dependencies |     |
|                              | ./vendor/bin/pest --init                                    |     |
|                              |                                                             |     |


##### PestPHP

###### Installation

```plaintext
composer remove phpunit/phpunit
composer require pestphp/pest --dev --with-all-dependencies
./vendor/bin/pest --init
```

###### Usage

```plaintext
./vendor/bin/pest
```
