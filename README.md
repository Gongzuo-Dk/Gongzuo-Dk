# Hi, I'm Daniel 👋

**Junior Backend Developer** — Python · Django · Django REST Framework · PostgreSQL

I'm a Junior Backend Developer based in Ukraine, focused on building clean, well-structured REST APIs and Django applications.
---

## 🛠 Tech Stack

**Backend**
`Python` `Django` `Django REST Framework` `PostgreSQL`

**Auth**
`dj-rest-auth` `django-allauth` `Google OAuth2` `Token Authentication`

**Testing**
`pytest` `pytest-django`

**Deployment**
`Railway` `Gunicorn` `WhiteNoise` `python-decouple`

---

## 📁 Projects

### [Expense Tracker API](https://github.com/Gongzuo-Dk/expense-tracker-drf) · [Live](https://web-production-82253a.up.railway.app/)
Pure REST API built with Django REST Framework and PostgreSQL. No templates — JSON only.

- Token auth + Google OAuth2 via django-allauth
- Ownership enforced at queryset level — users never see each other's data
- Custom `/summary/` and `/by-category/` endpoints using ORM aggregations (`Sum`, `Count`, `Avg`, `annotate`)
- Filtering by category, date range, and amount range
- pytest suite — 19 tests covering auth, ownership, cross-user 404s, and business logic
- Full README with endpoint docs and request/response examples

`Python` `Django` `DRF` `PostgreSQL` `pytest` `Railway`

---

### [Bookshelf API](https://github.com/Gongzuo-Dk/bookshelf-api) · [Live](https://bookshelf-api-production-d927.up.railway.app/)
Personal reading tracker REST API built with Django REST Framework and PostgreSQL. No templates — JSON only.
- Token auth via dj-rest-auth — register, login, receive token, authenticate all requests
- Ownership enforced at queryset level — users never see each other's books
- Custom `/stats/` endpoint using ORM aggregations (`Avg`, `Count`, `annotate`) — favourite genre via GROUP BY, average rating, goal progress
- Reading goal tracking with calculated progress percentage across `/goal/` and `/stats/`
- `SerializerMethodField` for computed fields — reading progress % returned without being stored in the database
- Cross-field serializer validation — rating only accepted on completed books, handles PATCH partial updates correctly
- pytest suite — 96% coverage across auth, ownership, cross-user 404s, and aggregation math
- Full README with endpoint docs and request/response examples
`Python` `Django` `DRF` `PostgreSQL` `pytest` `Railway`

---

### [WeatherApp](https://github.com/Gongzuo-Dk/weather-app) · [Live](https://weatherapp-production-cc78.up.railway.app/)
Django app consuming the OpenWeatherMap API — no database, pure service layer architecture.

- All external API logic isolated in `services.py` — views stay thin
- Geocoding flow: city name → coordinates → weather
- Current weather + 5-day forecast with Unix timestamp conversion
- Three template states: empty, error, data

`Python` `Django` `OpenWeatherMap API` `Railway`

---

### [Task Manager](https://github.com/Gongzuo-Dk/task-manager) · [Live](https://web-production-f102b.up.railway.app/)
Full-stack Django app with authentication, task/category CRUD, and smart filtering.

- Full auth system — register, login, logout, password change
- Smart date filters — Overdue, Today, Next 7 Days, Later, No Date
- Django signals for auto Profile creation on registration
- Context processors, custom 404/500 pages, ownership protection

`Python` `Django` `PostgreSQL` `Railway`

---

### [Blog App](https://github.com/Gongzuo-Dk/my-blog-project) · [Live](https://gongzuodk.pythonanywhere.com/)
Content-driven Django blog with full admin management and text search.

- Pinned posts, theme/category filtering, full-text search with input validation
- Pagination, default image fallback, responsive navbar

`Python` `Django` `SQLite` `PythonAnywhere`

---

## 📫 Contact

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Danylo_Kulynych-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/danylo-kulynych/)

---

*Open to Junior Backend Python / Django roles — remote.*
