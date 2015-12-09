## 3.x — Front-end — Installation

### Step 1: Install the package

Install the package via composer:

```
composer require riari/laravel-forum-frontend:~1.0
```

Then add the service provider to your `config/app.php`:

```php
'Riari\Forum\Frontend\ForumFrontendServiceProvider',
```

### Step 2: Publish the package files

Run the vendor:publish command to publish the package config and views to your app's directories:

`php artisan vendor:publish`

---

That's it; refer to [configuration](3.x/front-end/configuration.md) or [management](3.x/front-end/management.md) for further steps.
