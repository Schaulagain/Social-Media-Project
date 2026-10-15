# Social Media App (Laravel)

A small social network built with **Laravel 5.4**, one of my early Laravel projects. The focus was the back end, so the front end is a basic theme.

## Features

- Registration and login with Laravel's built-in auth
- Posts: create, edit, delete and view, organised by **categories**
- **Likes** and **comments** on posts
- **Friends:** send requests, accept, remove, and view a user's friend list
- Browse users and their profiles

## How it's built

- Eloquent models for `User`, `Post`, `Category`, `Comment`, `Like` and `Friend`, with relationships between them
- Resourceful controllers with `auth` middleware protecting everything that changes data
- Request validation in the post, comment and category controllers
- Blade templates for the views

## Running locally

Needs an old PHP version (Laravel 5.4 runs on PHP 7.0–7.2).

```sh
composer install
cp .env.example .env && php artisan key:generate   # then set DB_* in .env
php artisan migrate
php artisan serve
```

## Notes

This is an early project, kept for reference. My current Laravel work uses Laravel 9 and later; see [laravel-websocket](https://github.com/Schaulagain/laravel-websocket) and [Todo-App](https://github.com/Schaulagain/Todo-App).
