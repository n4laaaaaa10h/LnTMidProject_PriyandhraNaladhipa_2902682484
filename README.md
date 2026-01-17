# BayChat CMS
something something buat midterm bncc. tugas bncc dengan laravel 12.
gegara kepipkiran chatime ama tolak angin. jadinya ku bikin pake baygon. so basically landing page toko. already tested via postman.

## tech stack:
- laravel 12
- mysql/phpmyadmin
- composer
- rest api
- postman

## used tables
- users
- products
- categories

## relations
- Category (1) → Product (Many)
- one category bisa banyak produk

## endpoints

### category endpoints
| Method | Endpoint |
|------|----------|
| GET | /api/categories |
| POST | /api/categories |
| GET | /api/categories/{id} |
| PUT | /api/categories/{id} |
| DELETE | /api/categories/{id} |

### product endpoints
| Method | Endpoint |
|------|----------|
| GET | /api/products |
| POST | /api/products |
| GET | /api/products/{id} |
| PUT | /api/products/{id} |
| DELETE | /api/products/{id} |

---

## run
### 1. clone repository

git clone https://github.com/USERNAME/baychat-cms.git
cd baychat-cms

### 2. install dependecies
composer install

### 3. env setup
cp .env.example .env
php artisan key:generate

edit .env:
DB_DATABASE=baychat_cms
DB_USERNAME=(any)
DB_PASSWORD=(any)

### 4. database migrate
php artisan migrate

### 5. run server
php artisan serve

### 6. test
tes nya harus di website ini:
http://127.0.0.1:8000/api/categories
http://127.0.0.1:8000/api/products
