# Laravel_CRUD_API_JWT

composer install

composer require tymon/jwt-auth:dev-develop


php artisan vendor:publish

app/Http/Kernel.php的$routeMiddleware中：
加入
'auth.jwt'  =>  \Tymon\JWTAuth\Http\Middleware\Authenticate::class,

php artisan migrate


php artisan serve

=====
https://medium.com/@rommelhong/%E5%9C%A8laravel-6-rest-api%E4%B8%AD%E6%87%89%E7%94%A8json-web-token-jwt-e067e7fc7b1f
