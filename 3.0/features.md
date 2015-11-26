## 3.0 - Features

**Core ([Riari/laravel-forum](https://github.com/Riari/laravel-forum))**

 * RESTful API for all data querying and persistence (including a dispatcher for internal use)
 * Categories
    * Weighted and nestable to any level
    * Optional "private" mode using [Laravel Authorization](http://laravel.com/docs/5.1/authorization)
    * Enable/disable threads per category
 * Threads with moving, locking, pinning and deletion
 * Posts with editing and smart replying
 * Bulk modification or deletion of threads and posts
 * Optional soft-deletion support for threads and posts
 * Alert callback (to display success/validation messages using your preferred method)
 * Authentication and user integration via Laravel's auth interface and application user model
 * Permission handling via [Laravel Authorization](http://laravel.com/docs/5.1/authorization)
 * Multilingual (see [3.0 translations](https://github.com/Riari/laravel-forum/tree/3.0/translations) for a current list)
 * Highly configurable

**Front-end ([Riari/laravel-forum-frontend](https://github.com/Riari/laravel-forum-frontend))**

 * Read/unread/updated thread status
 * Default views written with [Bootstrap](http://getbootstrap.com/) compatibility in mind
 * Category/thread/post actions, enabling full management of your forum out of the box
 * [Events](http://laravel.com/docs/5.1/events) for viewing categories, threads, posts and forms

## Project Scope

Laravel Forum is designed to be as lean as possible while still providing a powerful foundation for building forums with minimal effort. As such, certain types of feature won't be considered for future releases; these include text editor integrations (e.g. CKEditor), smiley support and attachments, to name a few. Much like Laravel itself, our philosophy is to avoid making assumptions about the design and purpose of the application, only providing fundamental tools with standard integrations where possible.

This is also the justification behind providing the default front-end as a separate package from 3.0 onwards; while it should serve the purpose for most, some developers may prefer to build out their own front-ends using popular JS frameworks such as AngularJS and vue.js.

If you want to make a feature suggestion or contribute towards development but aren't sure about the project's scope, feel free to [open an issue](https://github.com/Riari/laravel-forum/issues/new). Even if we can't accept it as an official feature, you can always write a new package listing laravel-forum as a dependency and include your features in that.
