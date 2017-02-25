# Laravel-Users | A Laravel Users Management Package | v1.0.0

## Introduction

A Users Management Package that includes all necessary routes, views, models, and controllers for a user management dashboard and associated pages for managing Laravels built in user scaffolding.
Built for Laravel 5.2, 5.3, and 5.4+.

## Requirements

* [Laravel 5.2, 5.3, or 5.4 or newer](https://laravel.com/docs/installation)

   Example new project creation command:

   ```laravel new laravel-users-example```

* [Laravel Authentication Scaffolding](https://laravel.com/docs/authentication)

   Authentication installation command:

   ```php artisan make:auth```


## Installation

1. From your projects root folder in terminal run:

   ```
      composer require jeremykenedy/laravel-users
   ```

2. Register the package with laravel in `config/app.php` under `providers` with the following:

   ```
      Collective\Html\HtmlServiceProvider::class,

      jeremykenedy\laravelusers\LaravelUsersServiceProvider::class,

   ```


3. Register the dependencies aliases with laravel in `config/app.php` section under `aliases` with the following:

   ```
      'Form' => Collective\Html\FormFacade::class,
      'Html' => Collective\Html\HtmlFacade::class,
   ```

4. Publish the packages language files by running the following from your projects root folder:

   ```
      php artisan vendor:publish --tag=laravelusers
   ```

## Routes

* ```/users```
* ```/users/{id}```
* ```/users/create```
* ```/users/{id}/edit```

## Required Packages
(included in this package)

* [laravelcollective/html](https://packagist.org/packages/laravelcollective/html)

## Screenshots

![Show Users](https://s3-us-west-2.amazonaws.com/github-project-images/laravel-users/show-users.jpg)
![Show User](https://s3-us-west-2.amazonaws.com/github-project-images/laravel-users/show-user.jpg)
![Edit User](https://s3-us-west-2.amazonaws.com/github-project-images/laravel-users/edit-user.jpg)
![Edit User Password](https://s3-us-west-2.amazonaws.com/github-project-images/laravel-users/edit-user-pw.jpg)
![Create User](https://s3-us-west-2.amazonaws.com/github-project-images/laravel-users/create-user.jpg)
![Create User Modal](https://s3-us-west-2.amazonaws.com/github-project-images/laravel-users/save-user-modal.jpg)
![Edit User Modal]()
![Delete User Modal](https://s3-us-west-2.amazonaws.com/github-project-images/laravel-users/delete-user-modal.jpg)
![Error Create](https://s3-us-west-2.amazonaws.com/github-project-images/laravel-users/error-create.jpg)
![Error Update](https://s3-us-west-2.amazonaws.com/github-project-images/laravel-users/error-update.jpg)
![Error Delete](https://s3-us-west-2.amazonaws.com/github-project-images/laravel-users/error-delete.jpg)

## License

Laravel-Users | A Laravel Users Management Package is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT)