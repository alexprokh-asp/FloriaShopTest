# 🌸 Floria Shop API - Automated Tests

Automated API testing project for a flower shop backend using Postman + Newman + GitHub Actions CI.

---

## 📌 Project Overview

This project contains automated API tests for the Floria Shop backend service.

The goal is to validate:
- Search functionality
- Filtering and sorting logic
- Batch endpoints
- Recommendations system
- API validation rules and edge cases

---

## 🚀 Tech Stack

- Postman (test collection)
- Newman (CLI test runner)
- Node.js
- GitHub Actions (CI/CD)

---

## 📊 CI Status

[![CI - API Tests](https://github.com/alexprokh-asp/FloriaShopTest/actions/workflows/tests.yml/badge.svg)](https://github.com/alexprokh-asp/FloriaShopTest/actions/workflows/tests.yml)

---

[▶️ RUN AUTOTESTS](https://github.com/alexprokh-asp/FloriaShopTest/actions/workflows/tests.yml)

---

## 📂 API Under Test

Base URL:
https://floria-shop-api-34kp.onrender.com

---

## 🧪 Test Coverage

### /flowers/search
- pagination
- price filtering
- height filtering
- stems filtering
- sorting (price, popularity)
- combined filters
- validation errors
- empty results handling

---

### /flowers/recommendations
- response structure validation
- fixed number of items (4)
- required fields check
- recommendation flag validation

---

### /flowers/batch
- single ID fetch
- multiple IDs fetch
- invalid IDs handling
- duplicate IDs behavior
- edge cases (empty, negative, non-numeric)

---

## ⚙️ How to Run Locally

### Install dependencies
npm install

---

### Run tests
npm test

or directly:
npx newman run postman/collection.json -r cli,html

---

## 🤖 CI Pipeline (GitHub Actions)

Every push to main triggers:
- install dependencies
- run Newman tests
- generate HTML report
- upload report as artifact

---

## 📄 Test Report

After CI run:
1. Go to GitHub Actions
2. Open workflow run
3. Download Artifacts
4. Open report.html in browser

---

## 📁 Project Structure

```text
FloriaShopTest/
├── .github/
│   └── workflows/
│       └── tests.yml
├── postman/
│   └── collection.json
├── package.json
└── README.md
```

---

## 🧠 Notes

- Uses real API hosted on Render
- Tests include positive and negative scenarios
- Focus on validation, edge cases, and API contract stability

---

## 👨‍💻 Author

Alexandr Prokhoda - QA Automation practice project
