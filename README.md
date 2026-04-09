# Laravel Skeleton with Strict Configs

A strict, production-ready [Laravel](https://laravel.com/docs) starter with opinionated defaults for code quality, static analysis, and maintainability — built on top of [Livewire](https://livewire.laravel.com/docs).

![PHP](https://img.shields.io/badge/PHP-^8.3-blue)
![Laravel](https://img.shields.io/badge/Laravel-13.x-blue)
![License](https://img.shields.io/badge/license-MIT-green)

## Tech Stack

- PHP `8.3` or higher
- Laravel `13.x`
- Livewire `4.x`
- Pest PHP (testing)
- PHPStan (static analysis)
- Laravel Pint (formatting)
- Rector (automated refactoring)

## Features

- Strict and opinionated Laravel configuration. See [app/Providers/AppServiceProvider](./app/Providers/AppServiceProvider.php)
- Action-based architecture (`make:action` command for creating new action classes)
- Static analysis with [**PHPStan**](https://phpstan.org) (level 6). See [phpstan.neon](./phpstan.neon)
- Automated refactoring with [**Rector**](https://getrector.com). See [rector.php](./rector.php)
- Consistent code style via Laravel [**Pint**](https://laravel.com/docs/13.x/pint). See [pint.json](./pint.json)
- Full testing setup using [**Pest**](https://pestphp.com/docs).
- Built-in [**log viewer**](https://log-viewer.opcodes.io) for debugging.

## Philosophy

This template enforces:

- Explicit over implicit
- Static analysis first
- Small, testable classes (Actions pattern)
- Minimal magic
- Production-ready defaults

## Getting Started

1. Create your project based on this template

**Using GitHub CLI**

```bash
gh repo create <your-project> --template amyavari/laravel-skeleton-strict-configs --clone
cd <your-project>
```

**Using GitHub GUI**

- Click the **"Use this template"** button on this page and create your repository.
- Clone the repository

```bash
git clone https://github.com/<your-username>/<your-project>.git
cd <your-project>
```

2. Install dependencies

```bash
composer install
npm install
```

3. Setup environment

```bash

cp .env.example .env
php artisan key:generate
```

4. Run migrations

```bash
php artisan migrate
```

5. Start development

```bash
php artisan serve
npm run dev
```

## Contributing

All contributions are highly welcomed!

## License

**Laravel Skeleton with Strict Configs** was created by **[Ali Mohammad Yavari](https://www.linkedin.com/in/ali-m-yavari/)** under the **[MIT license](https://opensource.org/licenses/MIT)**.
