## 3.0 — Front-end — Configuration

The `forum.frontend` config file defines the controllers and utility class used by the package.

### Views

Views are published to `resources/views/vendor/forum`. The simplest way to integrate the forum with your existing design is to edit the **master** view, remove undesired markup and make it extend your application's main layout with `@extends`. Note that the master view does pull in jQuery and Bootstrap 3 by default, and includes some jQuery-based JavaScript to support some of the forum frontend features. You may wish to move it elsewhere or re-write it in your own way.

### Events

The package includes a variety of [events](http://laravel.com/docs/5.1/events) for user interactions such as viewing threads. Refer to [src/Events](https://github.com/Riari/laravel-forum-frontend/tree/master/src/Events) for a full list.
