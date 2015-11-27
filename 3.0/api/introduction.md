## 3.0 — API — Introduction

[laravel-forum 3.0](https://github.com/Riari/laravel-forum) provides a RESTful API that can be consumed over HTTP or [internally](3.0/api/internal-dispatching.md). It supports multiple [authentication](3.0/api/authentication.md) methods and offers endpoints for creating, querying, modifying and deleting [categories](3.0/api/categories.md), [threads](3.0/api/threads.md) and [posts](3.0/api/posts.md).

### Responses

Much like Laravel itself, responses returned by the API depend on the request context; internal requests can expect untouched collections and models (or an exception thrown in case of failed authorization, failed validation or "not found" responses), while requests over HTTP can expect a JSON-formatted collection, model or error code and message.

Take a look at [laravel-forum-frontend](https://github.com/Riari/laravel-forum-frontend) to get an idea of how responses can be used internally.