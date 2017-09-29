# Lumen / Laravel 


## Lumen 

`env('MY_CONSTANT');` //calls constants in .env

`config('services.sparkpost.secret');` //call something in 'config/services.php'


### Routes

in `routes/web.php` you use can use a closure


#### Return a view

```php

// Route to a view template
$app->get('myURL', function () use ($app) {
    //view file is in resources/views/myViewSubFolder/myView.blade.php
    return response(view('myViewSubFolder.myView'));  
    
});

// Route to controller
// Instead of a closure like the route to a view, this route goes to a controller class
$app->get('/about', 'MyController@myControllerFunction');

```


### Blade Commands

 COMMAND                            |        DESCRIPTION                
:-------------------------------    |:----------------------------------
`@extends('parentLayout')`          |                 
`@section('title', 'value')`        |
`@show`                             | define the place for a section in the parent template. 
`@endsection`                       | Child templates use
`@yield('name')`                    | placeholder of values
`@include('subviews')`              | all vars avail to parent are available in includes
`@includeif('someView')`            |
`@parent`                           | Causes an append instead of overwrite
`@stack` & `@push`                  | Add JS without worrying about overwriting if you forget `@parent`


`{{-- this is a comment in Blade --}}`


<!-- ************************************************
              LARAVEL
    ************************************************
-->

## Laravel

### Artisan commands

`php artisan routes:list`


