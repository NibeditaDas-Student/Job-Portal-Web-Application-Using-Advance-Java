# 🚀 Job Portal Web Application (Advanced Java)

A full-stack **Job Portal Web Application** developed using **Advanced Java (JSP & Servlet)** that allows users to search jobs, apply for jobs, build resumes, and manage their professional profiles.

---

## 📌 Project Overview

This project is a dynamic web-based job portal where:

* 👤 Users can register, login, and manage profiles
* 🔍 Search jobs by **technology** and **location**
* 📄 Apply for jobs and track applications
* 🧾 Build professional resumes (PDF generation)
* 📬 Contact system with email confirmation
* 📁 Upload profile pictures and resumes

The application follows **MVC architecture** using JSP (View), Servlets (Controller), and MySQL (Model).

---

## 🛠️ Tech Stack

| Layer       | Technology                |
| ----------- | ------------------------- |
| Frontend    | HTML, CSS, JSP            |
| Backend     | Java Servlets             |
| Database    | MySQL                     |
| Server      | Apache Tomcat             |
| PDF Engine  | iText, OpenHTMLtoPDF      |
| Email       | JavaMail API              |
| File Upload | Apache Commons FileUpload |

---

## ⚙️ Key Features

### 🔐 Authentication & Security

* User Registration with validation filter
* Login with **session + cookies (remember me)**
* Authentication filter to protect routes
* Server-side validation using regex

### 👤 User Profile Management

* Update basic details (skills, about, aspiration)
* Upload profile picture
* Manage:

  * 🎓 Education
  * 💼 Experience
  * 📂 Projects
  * 📜 Certificates

### 🔍 Job Module

* Search jobs by:

  * Technology
  * Location
* View job details
* Apply for jobs
* Delete applied jobs

### 📄 Resume System (🔥 Advanced Feature)

Multiple resume generation approaches:

* Dynamic PDF using **iText**
* HTML → PDF using **XMLWorker**
* Advanced HTML → PDF using **OpenHTMLtoPDF**

Includes:

* Profile info
* Education
* Experience
* Projects
* Certificates
* Personal details

### 📁 File Handling

* Upload profile picture
* Upload resume
* Download resume

### 📬 Contact System

* Contact form submission
* Email confirmation using JavaMail
* SMTP configuration (Gmail)

### 🍪 Session & Cookie Management

* Persistent login using cookies
* Cookie validation servlet
* Auto session restore

---

## 🗂️ Project Structure

```
JobPortal/
│
├── 📁 jsp/
│   ├── index.jsp
│   ├── login.jsp
│   ├── register.jsp
│   ├── profile.jsp
│   ├── jobsearch.jsp
│   ├── resume.jsp
│   └── ...
│
├── 📁 servlets/
│   ├── Login.java
│   ├── Register.java
│   ├── ApplyForJob.java
│   ├── GenerateResume.java
│   ├── JobSearchUsingTech.java
│   ├── JobSearchUsingLocation.java
│   └── ...
│
├── 📁 filters/
│   ├── AuthFilter.java
│   ├── ValidationFilter.java
│
├── 📁 utils/
│   ├── DbConnection.java
│   ├── SendConfirmationMail.java
│   ├── PathDetails.java
│
├── 📁 resources/
│   └── db.properties
│
└── web.xml
```

---

## 🧩 Configuration Details

### 🔌 Database Configuration

Defined in `db.properties`:

```properties
url = jdbc:mysql://localhost:3306/jobportal
user = root
password = nibedita
```

(Loaded dynamically via )

---

### 🌐 Web Configuration

* All servlets and filters are configured in `web.xml` 
* Includes:

  * Authentication Filter (`/*`)
  * Validation Filter (`/reg`)
  * Full URL mappings for all modules

---

## 🚀 How to Run the Project

### 🔧 Prerequisites

* Java 8+
* Apache Tomcat (8/9 recommended)
* MySQL Server
* IDE (NetBeans / Eclipse)

### ▶️ Steps

1. Clone the repository

```bash
git clone https://github.com/your-username/job-portal.git
```

2. Import into IDE as **Dynamic Web Project**

3. Configure database:

   * Create database: `jobportal`
   * Import required tables

4. Update:

   * `db.properties` (DB credentials)
   * Email credentials in `SendConfirmationMail`

5. Configure Tomcat server

6. Run the project

7. Open in browser:

```
http://localhost:8080/JobPortal/
```

---

## 📊 Modules Summary

| Module         | Description                 |
| -------------- | --------------------------- |
| Authentication | Login, Register, Logout     |
| Profile        | Manage user details         |
| Education      | Add/update academic details |
| Experience     | Work history                |
| Projects       | Portfolio                   |
| Certificates   | Certifications              |
| Jobs           | Search & apply              |
| Resume         | Generate & download PDF     |
| Contact        | Email system                |

---

## 🔒 Security Features

* Session-based authentication
* Cookie-based auto login
* Input validation using filters
* SQL injection prevention using PreparedStatement

---

## 💡 Highlights

* 🔥 Multiple resume generation strategies
* 🔥 Full CRUD system across modules
* 🔥 MVC architecture
* 🔥 Real-world job portal workflow
* 🔥 Email + File upload + PDF integration

---

## 👩‍💻 Author

**Nibedita Das**

* 💼 Aspiring Full Stack Developer
* 💻 Strong in Java, JSP, Servlets

---

## ⭐ Support

If you like this project:

* ⭐ Star the repository
* 🍴 Fork it
* 📢 Share it

---

## 📬 Contact

For any queries or collaboration:

* 📧 Email: nibeditadas615@gmail.com

---

> 🚀 This project demonstrates real-world implementation of **Advanced Java Web Development** concepts including Servlets, Filters, JDBC, and PDF generation.
