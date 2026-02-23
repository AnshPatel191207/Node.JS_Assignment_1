# 🎓 Student CGPA API (Express.js)

## 📌 Project Title

Student CGPA REST API using Express.js (In-Memory JSON Database)

---

## 🎯 Objective

Build a REST API using Express.js to manage student academic performance records stored in an in-memory JSON array.

This project demonstrates:

* RESTful API design
* Static & dynamic GET routes
* Server-side filtering & aggregation
* Proper HTTP status codes
* Deployment on Render

---

## 🛠️ Tech Stack

* Node.js
* Express.js
* CORS
* In-memory JSON database
* Postman (API testing)
* Render (Deployment)

---

## 📂 Student Data Format

Each student record contains:

```json
{
  "id": 1,
  "name": "Aarav Sharma",
  "branch": "CSE",
  "semester": 8,
  "cgpa": 9.3
}
```

---

# 🚀 Implemented API Routes

## 🔹 1. Get All Students

**GET** `/students`
Returns all student records.

---

## 🔹 2. Get Topper Student

**GET** `/students/topper`
Returns student with highest CGPA.

---

## 🔹 3. Get Average CGPA

**GET** `/students/average`
Returns average CGPA of all students.

Response:

```json
{
  "averageCGPA": 8.45
}
```

---

## 🔹 4. Get Total Students Count

**GET** `/students/count`

Response:

```json
{
  "totalStudents": 10
}
```

---

## 🔹 5. Get Student by ID (Dynamic Route)

**GET** `/students/:id`

Example:

```
/students/3
```

Returns student by ID.

---

## 🔹 6. Get Students by Branch (Dynamic Route)

**GET** `/students/branch/:branchName`

Example:

```
/students/branch/CSE
```

Returns all students from a specific branch.

Returns empty array if no student found.

---

# 💻 How to Run Locally

### Step 1: Clone repository

```bash
git clone https://github.com/yourusername/student-cgpa-api.git
cd student-cgpa-api
```

### Step 2: Install dependencies

```bash
npm install
```

### Step 3: Run server

```bash
npm run dev
```

Server runs on:

```
http://localhost:5000
```

---

# 🌐 Sample API URLs

```
http://localhost:5000/students
http://localhost:5000/students/topper
http://localhost:5000/students/average
http://localhost:5000/students/count
http://localhost:5000/students/3
http://localhost:5000/students/branch/CSE
```

---

# ☁️ Deployed API (Render)

https://node-js-assignment-1-474k.onrender.com

---

# 📬 Postman Documentation

https://documenter.getpostman.com/view/50841281/2sBXcGCeE4
