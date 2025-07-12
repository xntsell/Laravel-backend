# Tutorial
---
git clone saja 🧚‍♀️

abis itu lanjut
```bash
docker compose up -d --build
```
kalau udah pernah build langsung aja
```bash
docker compose up -d
```

masuk vscode
```bash
code .
```

---

## konfigurasi
```bash
docker exec -it pemweb bash
composer create-project --prefer-dist raugadh/fila-starter .
```

opsional kalau ada error bisa di hapus pakai:
```bash
rm -rf *
rm -rf .*
```

### Setting .env
```
APP_TIMEZONE='Asia/Jakarta'
APP_URL=http://localhost
ASSET_URL=http://localhost

DB_CONNECTION=mysql
DB_HOST=db_pemweb
DB_PORT=3306
DB_DATABASE=db_pemweb
DB_USERNAME=root
DB_PASSWORD=p455w0rd
```

```
chown -R www-data:www-data storage/*
chmod 777 -R storage/*
chmod 777 bootstrap/*
php artisan key:generate
php artisan migrate
php artisan shield:generate --all
php artisan project:init
```


web
```bash
php artisan make:livewire namanya
```

db
```
php artisan make:model Classroom -ms 
php artisan make:filament-resource Classroom --generate
```
