# EST Math | Educational Mathematics Platform

A modern, comprehensive educational platform designed to simplify mathematics for **EST** (Egyptian Scholastic Test) standardized examination students, created and supervised by: **Eyad Mahmoud Mohamed**.

---

## 🌟 Key Platform Features

- **100% Pure Vanilla Technologies**: Built entirely with **HTML5**, **CSS3**, and **Vanilla JavaScript** only. Zero external frameworks or libraries (No React, No Bootstrap, No Tailwind, No jQuery).
- **Fully Responsive Design**: Flawlessly adapts to Desktops, Laptops, Tablets, and Mobile phones with an animated, accessible Hamburger Drawer Navigation.
- **Modern Clean UI/UX & English LTR Layout**: Clear typography, balanced whitespace, smooth micro-interactions, subtle elevations, and focused educational color schemes.
- **Interactive Video Library (YouTube Style)**: Dynamic video cards with thumbnails, category badges, live search bar with real-time keyword matching, and a modal video player mockup with downloadable PDF materials.
- **Course Catalog & Enrollment Flow**: Structured course cards displaying lesson counts, duration, and pricing in EGP. Includes an in-depth Course Details Modal (Objectives & Syllabus) and an interactive Enrollment Modal with live form validation.
- **Direct 1-on-1 Academic Consultation**: Dedicated booking form with validation (Name, Email, Phone, Consultation Category, Details), automated reference ID generation, and immediate feedback.
- **Embedded Scalable Vector Graphics (SVG)**: All logos, course graphics, and lesson thumbnails are rendered as standalone vector SVGs to ensure high sharpness with zero broken images offline.

---

## 📁 Project Directory Structure

```text
est/
│
├── index.html              # Homepage (Hero + What We Offer + Latest Lessons + Founder Feature + CTA)
├── explanations.html       # Video Lessons Library (Live Search + Category Filters + Video Modal)
├── courses.html            # Course Catalog (Course Cards + Details Modal + Booking Modal)
├── consultation.html       # 1-on-1 Academic Consultation Booking (Validation & Feedback)
│
├── css/
│   └── style.css           # Complete Responsive Stylesheet (Pure CSS3 - LTR - CSS Variables)
│
├── js/
│   ├── main.js             # Mobile Hamburger Navigation, Sticky Header, Toasts & Modals
│   ├── explanations.js     # Explanations Data Array & Vanilla Search/Filter Logic
│   └── courses.js          # Courses Data Array & Details/Booking Modal Handlers
│
├── images/
│   ├── logo/
│   │   ├── logo.svg        # Official EST Math Vector Logo
│   │   └── favicon.svg     # Platform Favicon Badge
│   ├── thumbnails/         # 6 Vector Lesson Thumbnails (SVGs)
│   └── courses/            # 3 Vector Course Cover Graphics (SVGs)
│
└── README.md               # Complete Documentation & Developer Guide
```

---

## 🚀 How to Run the Website

1. Navigate to the project folder.
2. Double-click [index.html](index.html) to open it in any modern web browser (Google Chrome, Microsoft Edge, Firefox, Safari).
3. The platform works directly and standalone with zero dependencies or server installations required.

---

## ✏️ Easily Adding New Content

The codebase is built with modular data structures. You can easily add new lessons or courses in seconds by adding new objects into the JavaScript arrays:

### 1. Adding a New Video Lesson:
Open `js/explanations.js` and add a new object to `explanationsData`:

```javascript
{
  id: "exp-7",
  title: "New Lesson Title",
  description: "Short summary of what is taught in this video lesson.",
  thumbnail: "images/thumbnails/thumb-1.svg",
  category: "Past Exams", // Options: Math | Lessons | Practice | Past Exams
  date: "2026-10-05",
  duration: "35:00",
  instructor: "Eyad Mahmoud Mohamed",
  views: "1.2k views",
  videoUrl: "#"
}
```

### 2. Adding a New Training Course:
Open `js/courses.js` and add a new object to `coursesData`:

```javascript
{
  id: "course-4",
  title: "New Course Name",
  shortDescription: "Short preview description shown on the course card.",
  fullDescription: "Detailed breakdown shown inside the course details modal.",
  thumbnail: "images/courses/course-1.svg",
  lessonsCount: 24,
  duration: "48 Hours",
  price: 4000,
  currency: "EGP",
  level: "Advanced",
  tag: "New 🔥",
  objectives: [
    "First learning objective...",
    "Second learning objective..."
  ],
  syllabus: [
    "Module 1: ...",
    "Module 2: ..."
  ]
}
```

---

## 🔮 Future Roadmap (Full-Stack Scaling)

The clean semantic architecture allows for seamless backend integration when ready:
1. **Backend API**: Connect enrollment and consultation forms to a REST API (Node.js/Express or Python/FastAPI/Django).
2. **Database Integration**: Store student submissions, enrollment logs, and appointments in PostgreSQL or MongoDB.
3. **Student Authentication**: Student logins, progress tracking, and interactive quizzes.
4. **Online Payment Gateway**: Integration with Fawry, Vodafone Cash, Visa/MasterCard, or InstaPay.
5. **Instructor Admin Dashboard**: Empowering **Eyad Mahmoud Mohamed** to upload videos, edit courses, and manage student bookings dynamically.

---

## 👨‍🏫 Platform Info

- **Platform Name**: EST Math
- **Founder & Lead Instructor**: Eyad Mahmoud Mohamed
- **Copyright**: © 2026 EST Math - All Rights Reserved.
