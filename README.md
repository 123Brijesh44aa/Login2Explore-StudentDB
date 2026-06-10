  # 🎓 Student Enrollment Form

A modern, responsive web application for managing student records, built with **Bootstrap** and powered by **JsonPowerDB (JPDB)**. This project was developed as a minor project submission for the **Login2Explore Internship Selection Process (Round 2)**.

---

## 📝 Description

The **Student Enrollment Form** is a single-page web application designed to seamlessly create, retrieve, and update student records. It utilizes a dynamic, state-driven user interface that interacts directly with JsonPowerDB via high-performance REST APIs. 

The application enforces strict data workflow rules:
* **Automatic Lookup**: Entering a unique *Roll No.* and shifting focus (`onblur`) automatically queries the database.
* **Smart State Handling**: If the record does not exist, the form unlocks to allow data entry via the **Save** operation. If the record exists, the form populates the existing data instantly, disabling the primary key field and unlocking the **Update** operation.
* **Atomic Operations**: Integrated **Reset** handling allows users to clear states safely at any point.

---

## 📋 Table of Contents
- [Benefits of using JsonPowerDB](#-benefits-of-using-jsonpowerdb)
- [Scope of Functionalities](#%EF%B8%8F-scope-of-functionalities)
- [Technologies Used](#%EF%B8%8F-technologies-used)
- [Setup and Installation](#%EF%B8%8F-setup-and-installation)
- [Examples of Use](#-examples-of-use)
- [Release History](#-release-history)
- [Project Status](#-project-status)

---

## ⚡ Benefits of Using JsonPowerDB

[JsonPowerDB](http://login2explore.com/jpdb/resources/js/0.0.3/jpdb-commons.js) is a Next-Generation Geo-Distributed, Real-Time, High-Performance, Lightweight NoSQL Database. It offers several unique advantages for serverless and frontend-driven architectures:

* **No Backend Server Required**: Interacts directly from the client side using robust, secure REST APIs, eliminating the need to maintain an intermediate server layer (like Node.js/Express or Spring Boot).
* **Schema-less Deployment**: Built natively around JSON documents, allowing dynamic data structures without messy migrations or predefined tables.
* **Ultra-Fast Performance**: Built on top of a proprietary, high-performance in-memory indexing engine that drastically reduces transactional latency.
* **Integrated Web Services**: Out-of-the-box support for specialized Indexing, Key-Value data pairing, and structural Document tracking.
* **Developer Friendly**: Drastically simplifies CRUD pipelines via plug-and-play helper utilities like `jpdb-commons.js`.

---

## ⚙️ Scope of Functionalities

* **Automated Primary Key Validation**: Instantly verifies record existence without explicit form submission.
* **Contextual Element Disabling**: Dynamically shields fields and button components to prevent malformed or unauthorized data operations.
* **Comprehensive Data Validation**: Rejects empty fields natively before firing payloads to the IML endpoint.
* **Session Reset Mechanics**: Restores full-page initialization cleanly to prepare the interface for subsequent input.

---

## 🛠️ Technologies Used

* **Frontend UI**: HTML5, CSS3, Google Fonts (Poppins)
* **Framework**: Bootstrap v3.4.1 (Responsive Grid & Panels)
* **Scripting Core**: JavaScript (ES6 Code Execution Engine) + jQuery v3.5.1
* **Database Target**: JsonPowerDB (IML & IRL API Engines)

---

## 🛡️ Setup and Installation

### ⚠️ Crucial Security Configuration Note
> **Important:** This repository is public. For security compliance, the internal `CONN_TOKEN` string inside `index.html` must be updated manually prior to execution. Do not commit your personal tokens back to public version control systems.

1. **Clone the Repository**:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git)
   cd YOUR_REPO_NAME
