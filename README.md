# ⏳ Django Event Countdown Timer

A web application built with Django that allows administrators to schedule upcoming events via the Django Admin panel and displays an active, real-time countdown timer in the browser.

---

## 🚀 Features

- ⚙️ **Admin-Driven Management:** Add, update, and manage events easily through the built-in Django Admin interface.
- 🕒 **Real-Time Client-Side Updates:** JavaScript interval timer updates the remaining hours, minutes, and seconds every second without refreshing the page.
- 🧮 **Dynamic Time Calculations:** Django view calculates initial time differences between event dates and the current timestamp.
- 📱 **Clean Responsive UI:** Lightweight, styled countdown display centered for clean presentation.
- 🛡️ **Graceful Handling:** Displays fallback states when no upcoming events are scheduled.

---

## 🛠️ Technologies Used

- **Python**
- **Django**
- **SQLite** (Default Django ORM)
- **HTML5**
- **CSS3**
- **JavaScript**

---

## 📂 Project Structure

```text
timer/
│
├── manage.py
│
├── timer/                  # Project configuration
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
└── home/                   # Countdown application
    ├── migrations/
    │   └── ...
    ├── templates/
    │   └── myapp.html      # Countdown UI & JavaScript timer
    ├── __init__.py
    ├── admin.py            # Event model admin registration
    ├── apps.py
    ├── models.py           # Event database model
    ├── tests.py
    ├── urls.py             # App route mapping
    └── views.py            # Countdown logic & context rendering
