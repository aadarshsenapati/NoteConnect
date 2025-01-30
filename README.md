# Crowdsourced Study Notes Platform
### Introduction 
This is a crowdsourced study notes platform empowering students to share and access high-quality academic resources. It fosters collaboration, enabling peer-to-peer learning and creating a comprehensive repository for diverse subjects. Together, we make studying more effective and accessible for everyone in the university.


### Objective
To design and implement a dynamic crowdsourced platform that empowers university students to share, access, and contribute study notes. This platform aims to foster a culture of peer-to-peer learning and collaboration by providing a centralized repository of diverse, high-quality academic resources. By leveraging the collective knowledge and efforts of students, the platform seeks to enhance learning outcomes, promote inclusivity in education, and create an engaging and supportive academic environment where students can thrive together.

### Scope of Work
The Crowdsourced Study Notes Platform project aims to develop a user-friendly, collaborative web and mobile application that facilitates sharing and accessing academic resources. The scope of work includes the following deliverables:

1) User Management and Authentication:
   a) Develop secure user authentication and authorization features, including: <br>
       i) Registration and login for students.<br>
       ii) Role-based access control (e.g., admin for moderation).<br>

2) Core Features:<br>
   a) Upload and Download Resources:<br>
     i) Enable users to upload study materials, previous year papers, and notes.<br>
     ii) Provide a mechanism for users to download shared resources.<br>
     iii) Security: A person cannot share personal data like photo personal or personal video.<br>
   b) Search and Filter Functionality:<br>
     i) Implement a search bar with filters for subject, course, semester, or year.<br>
   c) Content Organization:<br>
     i) Organize resources by categories such as department, subject, and semester.Organize resources by categories such as department, subject, and semester.<br>
   d) Crowdsourcing Features:<br>
     i) Allow users to upvote, rate, and comment on uploaded materials to improve content quality.<br>
   
3) Administrative Panel<br>
   a) Build an admin dashboard for:<br>
     i) Moderating user-uploaded content to ensure appropriateness.<br>
     ii) Managing categories, subjects, and flagged materials.<br>
   
4) File Management and Storage<br>
   a) Local Development Environment:<br>
      i) Store uploaded files locally.<br>
   b) Cloud store to store files.<br>

5) Backend Development<br>
   a) Django<br>
     i) File upload/download.<br>
     ii) Ratings and comments.<br>
     iii) Search and filtering.<br>
   
7) Database Design and Integration<br>
   a) Design relational schemas for MySQL to store:<br>
     i) User data, file metadata, and ratings.<br>
   b) Integrate with MongoDB for flexible metadata handling if needed.<br>
   
8) Crowdsourcing Enhancements<br>
   a) Enable user interaction with features like:<br>
     i) Ratings to highlight useful materials.<br>
     ii) Comments for feedback and collaboration.<br>
     iii) Submission tracker using activity_visualizer<br>

### User Management<br>
1) Define two primary user roles:<br>
  a) Student: Can upload, download, and rate study materials.<br>
  b) Admin: Responsible for moderating content, managing categories, and addressing flagged uploads.<br>
2) Analytics for Admins:<br>
   a) Active users on the platform.<br>
   b) Number of new registrations.<br>
   c) Popular materials and categories.<br>

### Sample Requisition  
1) user_id: A unique identifier for each user.<br>
2) name: Full name of the user.<br>
3) email: Registered email address for login and communication.<br>
4) password: The hashed password for secure authentication.<br>
5) role: Defines the user's role (e.g., "student" or "admin").<br>
6) profile_picture: URL for the user’s profile image.<br>
7) created_at / updated_at: Timestamps for when the user account was created or last updated.<br>
8) activity: Tracks user actions, including uploads, ratings, and comments.<br>
9) notifications_enabled: A boolean field to manage email or in-app notifications.<br>

### Search Sample
1) Request Fields:<br>
  i) query: The search term entered by the user.<br>
  ii) filters: Specific criteria for narrowing results (e.g., subject, semester, department).<br>
  iii) sort_by and order: Options to organize results (e.g., by rating or upload date).<br>
  iv) page and results_per_page: Pagination settings for navigating large datasets.<br>

2) Response Fields:
  i) total_results: Total number of matching entries.<br>
  ii) current_page: Current page number.<br>
  iii) results_per_page: Number of results displayed on the current page.<br>
  iv) results: A list of matching files with details like:<br>
  v) File metadata (e.g., title, description, subject, semester, department).<br>
  vi) Uploader information and file access link.<br>
  vii) Engagement metrics (e.g., rating and downloads).<br>

### Report Generation & Download Data
1) Report<br>
   a) User Activity Report:<br>
     User details, including uploads, downloads, ratings, and comments.<br>
   b) Content Engagement Report:<br>
     Performance of uploaded resources (e.g., views, downloads, ratings).<br>
   c) Platform Analytics Report:<br>
     Number of active users, total uploads, downloads, and category-specific stats.<br>
   d) Custom Reports:<br>
     Generated based on filters like date range, department, or subject.<br>

2) Data
   a) In app content download
     Allow users to download study materials for offline use within the app while restricting access to raw files on their local storage.

### Technology Used
  1) HTML: HTML5
  2) CSS: CSS3
  3) JavaScript: ECMAScript 2024 (ES15)
  4) Django: Version 5.1.5
  5) Python: Version 3.12
  6) Figma: Web-based application
  7) Flutter: Version 3.10
  8) MySQL: Version 8.1
  9) MongoDB: Version 6.0

### Additional Tools:
  1) Bootstrap: Version 5.3
  2) Git: Version 2.42
  3) Photoshop Online: Web-based application for image editing
