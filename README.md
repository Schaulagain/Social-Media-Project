# Social Media App (Laravel)

A small social network in Laravel 5.4. It was one of my first Laravel projects. I spent my time on the back end, so the front end is just a basic theme.

Users can sign up, write posts in categories, like and comment on posts, and send, accept or remove friend requests. You can browse other users' profiles and friend lists.

It uses Eloquent models (`User`, `Post`, `Category`, `Comment`, `Like`, `Friend`), resource controllers, and Blade views. Anything that changes data needs you to be logged in, and the post, comment and category controllers validate their input.

## Running locally

You need an old PHP version for this. Laravel 5.4 runs on PHP 7.0 to 7.2.

```sh
composer install
cp .env.example .env && php artisan key:generate   # then set DB_* in .env
php artisan migrate
php artisan serve
```

I'm keeping this one up as an old example. For more recent Laravel code, see [laravel-nepal-payments](https://github.com/Schaulagain/laravel-nepal-payments).
