## 3.0 - Installation

### Step 1: Install the package

Install the package via composer:

```
composer require riari/laravel-forum:~3.0
```

Then add the service provider to your `config/app.php`:

```php
'Riari\Forum\ForumServiceProvider',
```

Installing the [standard front-end](https://github.com/Riari/laravel-forum-frontend) is recommended.

### Step 2: Publish the package files

Run the vendor:publish command to publish the package config, translations and migrations to your app's directories:

`php artisan vendor:publish`

### Step 3: Update your database

Run your migrations:

`php artisan migrate`
