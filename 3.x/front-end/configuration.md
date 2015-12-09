## 3.x — Front-end — Configuration

The front-end uses a single config file (`forum.frontend`) containing two values:

* `controllers`: An array of controller namespaces to use for the front-end routes.
* `utility_class`: The namespace of the class to use for the `alert()`, `render()` and `route()` methods.

### Views

Views are published to `resources/views/vendor/forum`. The simplest way to integrate the forum with your existing design is to edit the **master** view, remove undesired markup and make it extend your application's main layout with `@extends`. Note that the master view does pull in jQuery and Bootstrap 3 by default, and includes some jQuery-based JavaScript to support some of the forum frontend features. You may wish to move it elsewhere or re-write it in your own way.
