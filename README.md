# Laravel Auto Test Generator

Auto Test Generator package for routes in Laravel 6 and above. With just a few simple commands, this package will automatically generate unit test files for all of the routes

 in your Laravel application. No more manual testing or time-consuming set up. This package ensures that your routes are thoroughly tested and ready for deployment.

# Installation

Simply run the command `composer require thomyl/laravel-test-generator` in the root directory of your project. This will add the package to your project and make the 

artisan command available for use, allowing you to easily generate unit test files for all of your application's routes.

# Usage

Simply run the command `php artisan laravel-test:generate` in the root directory of your project to generate test cases for all of your application's routes, organized by 

controller.

Additionally, you can filter for specific routes by passing a filter attribute using **--filter**, for example `php artisan laravel-test:generate --filter='/api'`.

If you prefer to change the directory in which the test file is created, you can specify a directory using **--dir**, for example `php artisan laravel-test:generate --dir='V1'`.

You can also run the test cases synchronously by passing sync attribute using **--sync**, for example `php artisan laravel-test:generate --sync='true'`, this will add the 

@depends attribute to all the function except the first function. This will give you more control over the test execution order.
