## 3.x — Installation

### Requirements

+ PHP 5.4 or above
+ Laravel 5.1 or above (5.3 or above for package version ~4.0)

### Step 1: Install the package

Install the package via composer:

```
composer require riari/laravel-forum:~3.0
```

If you're using Laravel 5.3 or above, you'll need version ~4.0:

```
composer require riari/laravel-forum:~4.0
```

Then add the service provider to your `config/app.php`:

```php
Riari\Forum\ForumServiceProvider::class,
```

Installing the [front-end](3.x/front-end/introduction.md) is recommended.

### Step 2: Publish the package files

Run the vendor:publish command to publish the package config, translations and migrations to your app's directories:

`php artisan vendor:publish`

### Step 3: Update your database

Run your migrations:

`php artisan migrate`

Assuming this succeeds, you can now define your forum categories in the `forum_categories` table.
