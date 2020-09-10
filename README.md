# Laravel_CRUD_API_JWT
==
## 還原
composer install

composer require tymon/jwt-auth:dev-develop

cp .env.example .env
php artisan jwt:secret

  php artisan key:generate

php artisan migrate


php artisan serve

=====
api使用

使用者登入
http://127.0.0.1:8000/api/register 註冊 (name、email、password)
http://127.0.0.1:8000/api/login 登入 (email、password)

使用登入後的token操作
新增事件
http://127.0.0.1:8000/api/tasks 使用登入後的token  (email、password、token)
取得事件
http://127.0.0.1:8000/api/tasks?token=你登入後獲取的token
修改事件

刪除事件

https://medium.com/@rommelhong/%E5%9C%A8laravel-6-rest-api%E4%B8%AD%E6%87%89%E7%94%A8json-web-token-jwt-e067e7fc7b1f
