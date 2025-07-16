# Hostel Management System

A web-based Hostel Management System for educational institutions, featuring separate admin and student panels, room and course management, and booking workflows.

---

## Tech Stack

**Backend:**
- PHP (Recommended: 5.6, 7.4)
- MySQL (Database: `hostelmsphp`)

**Frontend:**
- HTML5, CSS3, JavaScript (jQuery)
- Bootstrap 4 (UI framework)
- SCSS for custom styles

**JavaScript Libraries/Plugins:**
- jQuery
- Bootstrap 4
- Chart.js, Chartist, Chartist Plugin Tooltips (charts)
- Morris.js, Raphael (charts)
- DataTables (with Bootstrap 4 integration)
- FullCalendar (calendar UI)
- Perfect Scrollbar
- Popper.js
- Moment.js

**Build Tools:**
- Gulp (SASS, minification, renaming, etc.)
- BrowserSync (live reloading)

---

## Features

### Admin Panel
- Dashboard with statistics (students, rooms, bookings, courses)
- Register new students
- View student accounts
- Book hostel rooms for students
- Manage students (view, edit, delete)
- Manage rooms (add, edit, delete)
- Manage courses (add, edit, delete)
- View booking and activity logs

### Student Panel
- Dashboard with personal info and stats
- Book hostel room
- View room details
- Log/view personal activities

### Authentication
- Separate login for Admin and Students
- Session management and access control

---

## Database Structure (Main Tables)
- `admin`: Admin user accounts
- `adminlog`: Admin login logs
- `courses`: List of courses
- `registration`: Hostel room bookings and student details
- `rooms`: Hostel room details
- `states`: List of states (for address info)
- `userlog`: Student login logs
- `userregistration`: Student user accounts

---

## Getting Started

### Prerequisites
- PHP 5.6 or 7.4
- MySQL
- Node.js and npm (for frontend build tools)

### Installation

1. **Clone the repository**
2. **Database Setup:**
   - Import `DATABASE FILE/hostelmsphp.sql` into your MySQL server.
   - Update database credentials in `includes/dbconn.php` and `includes/pdoconfig.php` if needed.
3. **Install Node dependencies:**
   ```
   npm install
   ```
4. **Build assets (optional, if you want to recompile SCSS/JS):**
   ```
   gulp
   ```
5. **Run the application:**
   - Place the project in your web server's root directory (e.g., `htdocs` for XAMPP).
   - Access via `http://localhost/Hostelies-main/index.php`

---

## Folder Structure

- `admin/` - Admin panel pages and logic
- `student/` - Student panel pages and logic
- `includes/` - Shared PHP includes (DB connection, navigation, etc.)
- `assets/` - CSS, JS, images, and third-party libraries
- `scss/` - Source SCSS files for custom styles
- `DATABASE FILE/` - SQL dump for database setup

---

- The project uses open-source libraries (see `package.json` and `assets/extra-libs/` for details).

---

## Credits

- Developed by Harshita (https://github.com/manno198 )
