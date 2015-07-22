## Features

 * Categories with nesting and weighting
 * Threads with locking, pinning and deletion
 * Posts with permalinks, editing and deletion
 * Optional soft-deletion of threads and posts
 * Alert callback (to display success/validation messages using your preferred method)
 * Pagination
 * Basic auth & user integration out of the box
 * Permissions handling middleware based on named routes
 * REST API with category, thread and post endpoints
 * Lightweight & fast
 * Read/unread/updated thread status (with 'New & updated threads' page)
 * Default views written with [Bootstrap](http://getbootstrap.com/) compatibility in mind
 * Multilingual (English, German, French, Italian and Romanian translations are available currently)

### Planned features & improvements

* More thread actions, such as moving between categories and editing thread titles
* Bulk editing of threads and posts (e.g. deletion and moving)
* Events per job
* Improved permissions handling using Middleware
* Configurable caching of threads and posts

### 'Blacklisted' features

Certain types of feature or functionality may seem like obvious additions to consider for a forum, but will likely never make an appearance in this package. Some of them are features that are commonly seen in other forum solutions and as such the question "X forum supports Z, why doesn't this?" sometimes crops up.

The simple answer to that is that the focus of this package is to provide functionality that is strictly relevant to forum categories, threads and posts. Much like Laravel itself and the vast majority of packages built for it, it's designed with developers in mind, and if a feature or change falls outside the scope of "things this package should inherently do", it probably won't be considered.

Some examples of such features are:

#### User-specific functionality (e.g. authentication, profiles, role system)
Some of this is baked into Laravel already and there are lots of packages that can provide the rest. If you're looking for well-supplemented authentication, roles and permissions, I highly recommend looking at [Zizaco/confide](https://github.com/Zizaco/confide) and [Zizaco/entrust](https://github.com/Zizaco/entrust). Entrust especially works very well with the permission callbacks in this package.

If your app has user profiles and you want to include the user's latest forum activity, you can easily achieve that by adding `threads()` and `posts()` relationships to your user model, pointing to the Thread and Post models respectively.

#### Thread/post tagging
A tagging system can be application-wide and in most cases probably should be. Even if you only want the ability to tag forum threads or posts, you might want the ability to tag other content in the future without having to introduce a second tagging system. If you want to achieve this, take a look at [rtconner/laravel-tagging](https://github.com/rtconner/laravel-tagging).

#### WYSIWYG/bbcode/markdown post editor
There are many different editors and parsers that could fill this gap, and you might want to use your choice of editor for more than just forum post authoring - so it's not included by default. However, it's very easy to integrate an editor of your choice and you can achieve that without changing any of the forum files except for a few views (i.e. the post textarea and post content). If you're looking for a nice markdown editor, for example, take a look at [lepture/editor](https://github.com/lepture/editor). I personally use that in conjunction with [cebe/markdown](https://github.com/cebe/markdown) for one of my apps.

#### Other examples...
Take a look at [fluxBB's list of unfeatures](http://fluxbb.org/docs/unfeatures). This follows a similar principle and most of the examples given there probably apply here too.

**All of the above said**, don't be discouraged from suggesting features in the [issue tracker](https://github.com/Riari/laravel-forum/issues). I'm not going to reject anything without good reason! Pull requests are also very welcome.
