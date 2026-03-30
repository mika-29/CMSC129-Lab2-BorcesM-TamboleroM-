## 🚑 Emergency Inventory Management System

A web-based inventory management system built with **Laravel** and **PostgreSQL**, designed to track emergency supplies for critical operations. It supports full CRUD functionality, stock status monitoring, soft deletes, search and filtering, and expiration date tracking.

## 📸 Screenshots

## ✅ Features Implemented
- **Inventory CRUD**: Add items, read, edit item details, and delete items.
- **Soft Delete**: Deleted items are moved to the trash and can be restored or permanently deleted.
- **Expiration Date Tracking**: Gives a warning when items are near expiry or already expired.
- **Critical Items Modal**: Clickable stat card that shows a modal of all critical (low/out of stock) items
- **Search & Filter**: Search by name, and filter by status and category.

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2. Install PHP Dependencies

```bash
composer install
```

### 3. Install Node Dependencies

```bash
npm install && npm run build
```

### 4. Copy Environment File

```bash
cp .env.example .env
```

### 5. Generate Application Key

```bash
php artisan key:generate
```

---

## 🐘 Database Setup (PostgreSQL)

### 1. Create the Database

Open your PostgreSQL shell (psql) or use pgAdmin:

```sql
CREATE DATABASE your_pg_database;
```

### 2. Configure `.env`

Update your `.env` file with your PostgreSQL credentials:

```env
DB_CONNECTION=pgsql
DB_HOST=127.0.0.1
DB_PORT=5432
DB_DATABASE=your_pg_database
DB_USERNAME=your_pg_username
DB_PASSWORD=your_pg_password
```

### 3. Run Migrations

```bash
php artisan migrate
```

---

## ▶️ Running the Application

```bash
php artisan serve
```

Then visit: [http://127.0.0.1:8000](http://127.0.0.1:8000)

## 🗂️ MVC Architecture
