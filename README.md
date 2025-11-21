<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## About Laravel Docker Stack

Мінімальний та чистий Docker-стек для запуску **Laravel + Nginx + PHP-FPM** без встановлення PHP або вебсерверів локально.
Підійде для навчання, pet-проєктів та швидкого старту власних застосунків.

---

## 🚀 Технології

* Docker & Docker Compose
* Nginx
* PHP-FPM
* Composer
* Laravel (версія залежить від локальної установки)

У майбутньому планується розширення:

* PostgreSQL або MySQL

---

## 📁 Структура проєкту

```
.
├── _docker/
│   ├── app/             # Dockerfile для PHP-FPM
│   └── nginx/           # Конфіг nginx
├── docker-compose.yml
├── public/
└── README.md
```

---

## ▶ Як запустити

### 1️⃣ Клонувати репозиторій

```
git clone https://github.com/USERNAME/laravel-docker-stack.git
cd laravel-docker-stack
```

### 2️⃣ Підняти контейнери

```
docker compose up -d
```

### 3️⃣ Встановити залежності Laravel

```
docker compose exec app composer install
```

### 4️⃣ Згенерувати APP_KEY

```
docker compose exec app php artisan key:generate
```

### 5️⃣ Відкрити в браузері

[http://localhost:8080](http://localhost:8080)

---

✔ Якщо бачиш Laravel або тестовий маршрут — все працює!


## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
