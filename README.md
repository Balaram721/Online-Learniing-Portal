# 🎓 Online Learning Portal: EduPortal

An innovative MERN stack-based full-stack web application for interactive online education. This platform empowers instructors to create and manage courses while enabling students to enroll, learn, and track their progress — all through a secure, responsive, and role-based interface.

## 🚀 Features

- 🔐 **Authentication & Authorization**
  - Secure login/register with JWT
  - Role-based access (Admin, Instructor, Student)
  - Protected routes (frontend + backend)

- 📚 **Course Management**
  - Instructors can create, edit, and delete courses/modules/lessons
  - Upload video URLs or content-rich lessons
  - Real-time lesson viewing for students

- 📈 **Student Progress Tracking**
  - Track completed modules
  - View progress with interactive progress bars
  - Enroll and view enrolled course list

- 🧪 **Robust Form Validation**
  - Client-side: React Hook Form + Yup
  - Server-side: Mongoose schema validation

- 🌐 **Responsive UI/UX**
  - Mobile-first design
  - Tailwind CSS + ShadCN components
  - Toast notifications and smooth navigation

- 🧠 **Admin Dashboard**
  - View users, manage roles
  - Track platform stats
  - Manage course data

---

## 🛠️ Tech Stack

**Frontend:**
- React.js + Vite
- React Router DOM
- Context API (for global auth/user state)
- Axios (API communication)
- Tailwind CSS + ShadCN UI
- React Hook Form + Yup

**Backend:**
- Node.js + Express
- MongoDB + Mongoose
- JWT-based authentication
- RESTful APIs
- Middleware: auth, error handler, role-check

**Other Tools:**
- Git & GitHub for version control
- .env for environment configuration
- Render/Vercel/Netlify (deployment-ready)

---

## 🗂️ Project Structure
    ```bash
    📁 client/
    ├── components/
    ├── pages/
    ├── context/
    ├── routes/
    └── utils/
    
    📁 server/
    ├── controllers/
    ├── models/
    ├── routes/
    ├── middleware/
    └── config/
  

---

## 🔍 Key Modules

| Entity    | Fields                                                                 |
|-----------|------------------------------------------------------------------------|
| User      | name, email, password (hashed), role (admin/instructor/student)        |
| Course    | title, description, instructorId, modules[], enrolledUsers[], createdAt|
| Module    | title, lessons[], courseId                                              |
| Lesson    | title, content, videoUrl, moduleId, completedByUsers[]                 |


## 🧪 Getting Started

### 1. Clone the repository 
    clone the repository
    cd online-learning-portal  
    
### 2. Setup backend
    cd server
    npm install
    cp .env.example .env # Add MongoDB URI and JWT secret
    npm run dev  
    
### 3. Setup frontend
    cd client
    npm install
    npm run dev  
Make sure your backend is running on http://localhost:5001 and frontend on http://localhost:5173 (or update accordingly).  

## 🏁 Future Improvements  
🎥 Local video uploads & video player integration  
⭐ Course rating and review system  
📄 Certificate generation after course completion  
🔍 Advanced search, filter, and sort for courses  
📱 PWA support  

## 📚 Learning Outcomes  
Full-stack development using MERN  
REST API design and secure authentication  
Real-world component design with Tailwind and ShadCN  
Scalable code architecture and deployment  
Git collaboration and version control  

## 🧑‍💻 Author
Gummadi Balaram
📧 gummadibu@gmail.com  

## 📄 License  
This project is licensed under the MIT License.


