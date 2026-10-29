# Full Stack Application Development Capstone Project

**Repository Name:** `xrwvm-fullstack_developer_capstone`  
**Project Name:** Cars Dealership Full-Stack Web Application

---

## Project Overview

**Dealerships Website** is a cloud-native, full-stack web application developed as part of the **IBM Full Stack Software Developer Professional Certificate** Capstone Project.

The application serves a national car retailer in the United States, allowing prospective and existing customers to:
* Browse a nationwide network of 50 car dealership branches.
* Filter dealerships by state.
* View individual dealership details and available vehicle inventories (makes and models).
* Read authentic customer reviews.
* Submit new reviews with integrated AI sentiment analysis (positive, neutral, negative).
* Securely register, authenticate, and manage user sessions.

---

## Architecture & Technology Stack

* **Frontend:** React, HTML5, CSS3, JavaScript (ES6+), Bootstrap
* **Backend:** Python, Django, Django REST Framework, SQLite
* **Microservices:** Node.js, Express, MongoDB (Dealerships and Reviews Database)
* **AI Microservice:** Python, Flask, NLTK Sentiment Analysis (VADER)
* **DevOps & Cloud:** Docker, Kubernetes, IBM Code Engine / Theia, GitHub Actions (CI/CD)

---

## Repository Structure

```
xrwvm-fullstack_developer_capstone/
├── server/
│   ├── database/                  # Node.js & Express microservice with MongoDB data
│   │   ├── data/                  # Seed datasets (dealerships.json, reviews.json)
│   │   └── app.js                 # Express API routes (/fetchDealers, /fetchReviews)
│   ├── djangoapp/                 # Django application views, models, and proxy services
│   │   ├── microservices/         # Flask sentiment analysis microservice (/analyze)
│   │   ├── models.py              # CarMake and CarModel schemas
│   │   └── views.py               # Authentication and data endpoints
│   ├── djangoproj/                # Django project settings and root URLs
│   └── frontend/                  # React frontend application & static pages
│       ├── src/components/        # React components (Register, Login, Dealers)
│       └── static/                # Static HTML pages (About.html, Contact.html)
└── README.md
```
