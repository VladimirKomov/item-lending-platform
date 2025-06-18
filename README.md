# 📦 Item Lending Platform (Backend Only)

This project is an educational **backend-only API** that enables users to share items, manage orders, and leave reviews. It is built with **Django** and **Django REST Framework**, includes JWT-based authentication, AWS S3 media storage, and supports caching via Redis. The system is containerized with Docker and can be easily deployed locally.

---

## ✨ Key Features

- 🔐 **JWT Authentication** – secure login and token-based access
- 📦 **Item Management** – add, update, and view items with images
- 🏷️ **Categories & Filtering** – organize and search items by category
- 🛒 **Orders and Reviews** – borrow items and leave feedback
- 🧑‍💼 **User Dashboard** – manage profile, orders, and listings
- 🗺️ **Google Maps Integration** – geolocation support for items
- ☁️ **AWS S3** – scalable image storage
- ⚡ **Redis Caching** – improve response times for frequent queries
- 🐳 **Docker Support** – launch the entire stack with one command

---

## ⚙️ Tech Stack

- 🌐 **Backend:** Django, Django REST Framework
- 🧠 **Auth:** JWT via `djangorestframework-simplejwt`
- 🐘 **Database:** PostgreSQL
- ☁️ **Storage:** AWS S3 for media files
- ⚡ **Cache:** Redis
- 🐳 **Containerization:** Docker + Docker Compose

---

## 🚀 Getting Started

### 1️⃣ Clone the repository

```bash
git clone https://github.com/VladimirKomov/item-lending-platform.git
cd item-lending-platform
```

### 2️⃣ Configure Environment Variables

Create a `.env` file in the project root and set the following:

```env
# PostgreSQL
DB_NAME=your_database_name
DB_USER=your_database_user
DB_PASSWORD=your_database_password
DB_HOST=your_database_host
DB_PORT=5432

# AWS S3
AWS_ACCESS_KEY_ID=your_access_key
AWS_SECRET_ACCESS_KEY=your_secret
AWS_STORAGE_BUCKET_NAME=your_bucket_name
AWS_S3_REGION_NAME=your_region
```

### 3️⃣ Run the application with Docker

```bash
docker-compose up --build
```

- API available at: http://localhost:8000
- Django admin: http://localhost:8000/admin/

---

## 🔧 Useful Commands (in container)

```bash
# Run migrations
python manage.py migrate

# Create superuser
python manage.py createsuperuser

# Collect static files
python manage.py collectstatic
```

---

## 📜 License

This project is provided for educational and personal use only. Commercial use is not permitted.

---

## 👤 Author

**Vladimir Komov**  
GitHub: [@VladimirKomov](https://github.com/VladimirKomov)  
LinkedIn: [Vladimir Komov](https://www.linkedin.com/in/vladimirkomov)