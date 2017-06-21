# Data Migrations for Laravel

This package allows to migrate data the same way as regular database structure migrations.

### Installation

**Composer**
```shell
composer require michielfb/data-migrations
```

### Configuration

1. For Laravel 5.4 and less: Register the ServiceProvider in your config/app.php service provider list.

```php
\Michielfb\DataMigrations\DataMigrationsServiceProvider::class
```

2. Publish the new assets.
```shell
php artisan vendor:publish --tag=data-migrations
```

3. Run the database migration
```shell
php artisan migrate
```

### Usage

The following artisan commands are available.

`make:data-migration` creates a new data migration.

`migrate:data` runs the data migration

`migrate:rollback-data` rolls back the migration.

