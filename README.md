<p align="center"><img src="https://symfony.com/logos/symfony_white_03.png" width="200" alt="Symfony Logo"></p>

# Symfony ecommerce project

## О проекте

Интернет магазин cозданный с использованием фреймворка Symfony.

## Основные функции

- Регистрация и Аутентификация.
- Каталог товаров с фильтром по категориям.
- Корзина.
- Админ панель, для создания новых пользователей, категорий и товаров.


## Установка

Скопируйте данный проект к себе на компьютер с помощью команды
```
git clone https://github.com/duaves/ecommerce-symfony.git
```
Установите зависимости
```
composer install
```
Настройте подключение к базе данных (DATABASE_URL) в файле .env, так же измените MAILER_DSN и STRIPE_SK
  
Создайте базу данных, выполнив
```
php bin/console doctrine:database:create
```
Сгенерируйте требуемую схему базы данных, выполнив
```
php bin/console doctrine:schema:update -f
```
Запустите сервер разработки Symfony с помощью
```
symfony server:start -d
```
Для доступа к админ панели, зарегистрируйте пользователя и измените роль на {"role": "ROLE_ADMIN"} в базе данных.
