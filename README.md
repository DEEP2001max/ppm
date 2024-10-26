<!DOCTYPE html>
<html lang="en">

<body>

<h1>Placement Management Portal</h1>

<p><strong>Author</strong>: CultSoft<br>
<strong>Technologies Used</strong>: HTML, CSS, JavaScript, PHP, MySQL<br>
<strong>Database Name</strong>: <code>miniproject</code></p>

<h2>Project Description</h2>

<p>The Placement Management Portal is a web-based application designed to streamline and manage the placement process for colleges and universities. The portal allows administrators to manage student profiles, job listings, and placement records, providing an organized, user-friendly interface for efficient placement activities.</p>

<h2>Features</h2>

<ul>
    <li><strong>Student Registration and Profile Management</strong>: Students can register, update their profiles, and view placement opportunities.</li>
    <li><strong>Job Listing Management</strong>: Admins can post, update, and delete job listings available to students.</li>
    <li><strong>Placement Tracking</strong>: Track placement statuses and allow students to view their placement status.</li>
    <li><strong>User Authentication</strong>: Basic user login and registration for students and administrators.</li>
    <li><strong>Responsive Design</strong>: Optimized for both desktop and mobile devices.</li>
</ul>

<h2>Project Structure</h2>

<pre>
    ├── css/                     # Contains all CSS files for styling
    ├── js/                      # Contains JavaScript files for frontend logic
    ├── db/                      # Contains the SQL database file
    ├── index.html               # Main landing page
    ├── register.html            # Registration page for students
    ├── login.html               # Login page for all users
    ├── dashboard.php            # Dashboard for both students and admins
    ├── job_listings.php         # Page displaying available job listings
    ├── placement_records.php    # Page showing placement records for admins
    ├── README.html              # Project documentation
    └── db/miniproject.sql       # Database setup file
</pre>

<h2>Database Setup</h2>

<ol>
    <li><strong>Create the Database</strong>: Open your MySQL client (e.g., phpMyAdmin, MySQL Workbench, or command line) and create a database named <code>miniproject</code>.
        <pre><code>CREATE DATABASE miniproject;</code></pre>
    </li>
    <li><strong>Import the Database Schema</strong>: Inside the <code>db/</code> directory, there is a file named <code>miniproject.sql</code>. This file contains all the necessary table structures and initial data for the application.
        <ul>
            <li>Import the SQL file by running the following command in your MySQL command line:
                <pre><code>mysql -u your_username -p miniproject < db/miniproject.sql</code></pre>
            </li>
            <li>Alternatively, you can import the SQL file via phpMyAdmin by selecting the <code>miniproject</code> database, clicking on the "Import" tab, and uploading the <code>miniproject.sql</code> file.</li>
        </ul>
    </li>
    <li><strong>Configure Database Connection in PHP</strong>: In the project files, locate the PHP configuration file where database credentials are defined (e.g., <code>config.php</code> or at the top of each PHP script if configured locally). Ensure your MySQL credentials are correctly set.
        <pre><code>
$servername = "localhost";
$username = "your_username";
$password = "your_password";
$dbname = "miniproject";
        </code></pre>
    </li>
</ol>

<h2>Getting Started</h2>

<h3>Requirements</h3>

<ul>
    <li>PHP (version 7.0 or higher recommended)</li>
    <li>MySQL (or MariaDB)</li>
    <li>Web Server (Apache, XAMPP, or similar)</li>
</ul>

<h3>Running the Project Locally</h3>

<ol>
    <li>Clone the repository to your local machine.
        <pre><code>git clone https://github.com/DEEP2001max/ppm.git</code></pre>
    </li>
    <li>Move the project files to your web server’s root directory (e.g., <code>htdocs</code> in XAMPP).</li>
    <li>Open a web browser and navigate to the portal’s main page:
        <pre><code>http://localhost/placement-management-portal/index.html</code></pre>
    </li>
    <li>Register as a new student or log in as an admin to start using the system.</li>
</ol>

<h2>File Explanations</h2>

<ul>
    <li><strong><code>index.html</code></strong>: The main page for the Placement Management Portal.</li>
    <li><strong><code>register.html</code></strong>: Registration form for students to create a new account.</li>
    <li><strong><code>login.html</code></strong>: Login page for both students and administrators.</li>
    <li><strong><code>dashboard.php</code></strong>: Displays personalized dashboard for users.</li>
    <li><strong><code>job_listings.php</code></strong>: Displays the list of available job listings for students.</li>
    <li><strong><code>placement_records.php</code></strong>: Admin-only access page showing placement records.</li>
</ul>

<h2>Future Enhancements</h2>

<ul>
    <li><strong>Improved Role-based Access</strong>: Enhance user roles for better access control between students, admins, and recruiters.</li>
    <li><strong>Enhanced Security</strong>: Implement password hashing, two-factor authentication, and data sanitization.</li>
    <li><strong>Email Notifications</strong>: Automatic notifications for placement events and updates.</li>
</ul>

<h2>License</h2>

<p>This project is licensed under the MIT License.</p>

</body>
</html>
