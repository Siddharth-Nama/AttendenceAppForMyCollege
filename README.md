# 📚 Attendance App for My College

Visit the live project at [Siddharth Attendance Portal](https://siddharthattendanceportal.pythonanywhere.com) (Best viewed on a laptop).

This **Attendance App** is a robust and efficient platform designed specifically for **IIIT Bhagalpur**. It provides a streamlined system for managing attendance, enabling teachers to generate **6-digit unique codes** for classes and allowing students to mark their attendance using these codes. The app ensures accuracy, transparency, and simplicity for both teachers and students. **Role-Based Access Control (RBAC)** is implemented to secure access based on user roles (Student/Teacher).

---

## 🌟 Key Features

- **Role-Based Access Control (RBAC)**: Ensures separate access rights for teachers and students.
- **6-Digit Unique Code Generation**: Teachers can generate shareable codes (via WhatsApp or other platforms) for attendance.
- **Secure User Authentication**: Provides role-specific dashboards and features.
- **Real-Time Attendance Management**: Automatically records and stores attendance securely in the database.
- **User-Friendly Interface**: Intuitive design for seamless navigation across functionalities.

---

## 📁 Project Structure

Here's an overview of the key components of the project:

- **account/**: Handles user authentication and role-based access (Student/Teacher).
- **attendance/**: Manages attendance functionalities, including code generation and validation.
- **templates/**: HTML files for the user interface, including login, dashboard, and attendance pages.
- **static/**: CSS, JavaScript, and image resources for styling and interactivity.
- **media/**: Stores shareable codes and related files.

Each module is modularly designed for scalability and ease of maintenance.

---

## 🛠️ Technology Stack

- **Backend**: Django (Python)
- **Frontend**: HTML, CSS, JavaScript (Bootstrap for responsive design)
- **Database**: SQLite (Default for Django; can be switched to PostgreSQL or MySQL for production)
- **Random Code Library**: Python's built-in `secrets` library for generating secure codes
- **Hosting**: Deployment-ready for platforms supporting Django (e.g., PythonAnywhere)

---

## 🚀 Getting Started

To set up this project locally, follow these steps:

### Prerequisites

- **Python 3.7+**: Make sure Python is installed on your system.
- **Virtual Environment**: Recommended for managing dependencies.

### Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Siddharth-Nama/AttendenceAppForMyCollege.git
   cd AttendenceAppForMyCollege
   ```

2. **Create a Virtual Environment**:
   ```bash
   python -m venv myenv
   source myenv/bin/activate  # macOS/Linux
   myenv\Scripts\activate     # Windows
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Run Database Migrations**:
   ```bash
   python manage.py migrate
   ```

5. **Create a Superuser**:
   ```bash
   python manage.py createsuperuser
   ```

6. **Start the Development Server**:
   ```bash
   python manage.py runserver
   ```

   The application will be accessible at `http://127.0.0.1:8000`.

---

## 📚 Usage Guide

### Teacher Operations

1. **Log In**: Access the teacher dashboard using role-specific credentials.
2. **Generate Attendance Code**: Create a unique, 6-digit shareable code for each class session.
3. **Share Code**: Share the code with students via WhatsApp or other platforms.
4. **View Attendance Records**: Monitor attendance data for all classes.

### Student Operations

1. **Log In**: Access the student dashboard after authentication.
2. **Enter Attendance Code**: Enter the provided code to mark attendance.
3. **View Attendance**: Check attendance history and records.

---

<!-- ## 📸 Screenshots

- **Login Page**  
  ![Login Page](/static/screenshots/login.png)

- **Code Generation (Teacher)**  
  ![Code Generation](/static/screenshots/code_generation.png)

- **Student Dashboard**  
  ![Student Dashboard](/static/screenshots/student_dashboard.png)

--- -->

## 🚀 Deployment Guide

To deploy this project on a production server, make sure to:

1. **Set DEBUG=False**: Configure Django to disable debug mode in production.
2. **SECRET_KEY**: Replace the default secret key with a secure, custom key.
3. **Database**: Use a production-ready database like PostgreSQL.
4. **Static Files**: Run `python manage.py collectstatic` to gather static assets.

---

## 🤝 Contributing

Contributions are welcome! To contribute:

1. **Fork the Repository**.
2. **Create a Feature Branch**:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Commit Your Changes**:
   ```bash
   git commit -m "Add a brief description of your changes"
   ```
4. **Push to the Branch**:
   ```bash
   git push origin feature/your-feature-name
   ```
5. **Open a Pull Request**.

---

## 📜 License

This project is licensed under the MIT License. See the LICENSE file for details.

---

## 👥 Developed By

This project was developed by **Siddharth Nama** with the goal of enhancing attendance management at **IIIT Bhagalpur**. You can connect with me on [LinkedIn](https://www.linkedin.com/in/siddharth-nama-1bb967256/).