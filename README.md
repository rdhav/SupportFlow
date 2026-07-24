# 🎫 Support Desk / Ticketing System

A modern web-based complaint & ticket management system built with **Laravel, Livewire, Alpine.js, and Flowbite**.
This application helps companies manage internal or customer complaints in a structured, trackable, and efficient way.

---

## 🚀 Tech Stack

- **Laravel** → Backend Framework
- **Livewire** → Reactive UI (no heavy JavaScript)
- **Alpine.js** → Lightweight interactivity
- **Flowbite + Tailwind CSS** → Modern UI components
- **MySQL** → Database

---

## 🎯 Purpose

Many companies still handle complaints through:

- WhatsApp ❌
- Email ❌
- Manual notes ❌

This leads to:

- Lost messages
- No tracking system
- Poor accountability

✅ This system solves that by providing:

- Structured ticket management
- Status tracking
- Communication history
- Performance monitoring

---

## 🔄 Application Flow

1. **User creates a ticket**
2. Ticket is stored in the system
3. Admin/Support reviews the ticket
4. Admin responds & updates status
5. User and Admin communicate via comments
6. Ticket is resolved and closed

---

## 📌 Features (MVP)

- 🔐 Authentication (Login/Register)
- 🎫 Create Ticket
- 📋 Ticket List (User & Admin)
- 🔍 Ticket Detail Page
- 💬 Comment / Discussion
- 🔄 Ticket Status (Open, In Progress, Resolved, Closed)
- 📊 Simple Dashboard

---

## 📊 Ticket Status Flow

```
OPEN → IN_PROGRESS → RESOLVED → CLOSED
```

---

## 🧱 Project Structure

```
support-desk/
 ├── app/
 ├── bootstrap/
 ├── config/
 ├── database/
 ├── public/
 ├── resources/
 │   ├── views/
 │   ├── js/
 │   └── css/
 ├── routes/
 ├── storage/
 ├── tests/
 ├── artisan
 ├── composer.json
 └── package.json
```

---

## ⚙️ Installation & Setup

### 1. Clone Repository

```bash
git clone https://github.com/rdhav/SupportFlow.git
cd SupportFlow
```

### 2. Install Dependencies

```bash
composer install
npm install
```

### 3. Setup Environment

Copy `.env` file:

```bash
cp .env.example .env
```

### 4. Generate App Key

```bash
php artisan key:generate
```

### 5. Setup Database

Edit `.env`:

```env
DB_DATABASE=SupportFlow
DB_USERNAME=root
DB_PASSWORD=
```

Then run:

```bash
php artisan migrate
```

### 6. Run Application

If using Laravel Herd:

```
http://SupportFlow.test
```

Or manual:

```bash
php artisan serve
npm run dev
```

Access:

```
http://127.0.0.1:8000
```

---

## 🧪 Development Commands

```bash
php artisan serve
npm run dev
php artisan migrate:fresh --seed
```

---

## 🌐 Deployment (Production)

### Simple & Cheap Option

- VPS (Contabo / DigitalOcean)
- Laravel Forge (optional)
- Or shared hosting (if supported)

### Basic Deployment Steps

```bash
git clone https://github.com/rdhav/SupportFlow.git
cd SupportFlow

composer install --no-dev --optimize-autoloader
npm install
npm run build

cp .env.example .env
php artisan key:generate

php artisan migrate

php artisan config:cache
php artisan route:cache
php artisan view:cache
```

---

## 🔮 Future Improvements

- 📧 Email Notifications
- ⏱ SLA & Deadline Tracking
- 👥 Role Management (Admin, Staff, User)
- 📎 File Attachments
- 🔎 Advanced Search & Filtering
- 📊 Analytics Dashboard

---

## 👨‍💻 Author

- GitHub: [**Alvin**](https://github.com/rdhav)
- GitHub: [**Sulistio**](https://github.com/Tiomiku)
