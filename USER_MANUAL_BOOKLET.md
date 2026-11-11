# APPENDIX: SYSTEM USER MANUAL
## Vinzons Pilot Elementary School – Student Information and Management System (VPES-SIMS)
*DepEd School ID: 112937 | Division of Camarines Norte | Region V – Bicol*

---

# [COVER PAGE]

```text
================================================================================
                                USER MANUAL
                   VINZONS PILOT ELEMENTARY SCHOOL (VPES)
              STUDENT INFORMATION AND MANAGEMENT SYSTEM (SIMS)
================================================================================

             [INSERT PHOTO / SYSTEM GRAPHIC PLACEHOLDER HERE]
    Recommended Image: High-resolution collage or mockup showing the 
       VPES-SIMS Landing Page, Admin Dashboard, and Mobile Responsive View.

--------------------------------------------------------------------------------
                     Camarines Norte State College (CNSC)
               College of Information and Communications Technology
                          Department of Computer Studies
--------------------------------------------------------------------------------
```

---

# [SYSTEM OVERVIEW & INTRODUCTION]

### SYSTEM OVERVIEW
The **Vinzons Pilot Elementary School – Student Information and Management System (VPES-SIMS)** is a centralized, cloud-hosted web application engineered to modernize and digitize the institutional processes of Vinzons Pilot Elementary School (School ID: 112937) in Vinzons, Camarines Norte. 

The system transitions traditional manual operations—such as paper-based admissions, walk-in appointment queuing, physical index card records, manual section balancing, and handwritten DepEd school forms (SF4, SF6, SF7, SF9, and SF10-ES)—into a responsive, secure, and automated digital ecosystem. Hosted online with SSL/TLS encryption, VPES-SIMS delivers role-specific portals tailored for School Administrators, Subject Teachers, Class Advisers, Enrolling Applicants, and Continuing Students/Guardians.

### SYSTEM SPECIFICATIONS & REQUIREMENTS
* **Deployment Model:** Cloud-Hosted Online Server (Hostinger Cloud Infrastructure / HTTPS / Custom Domain)
* **Client-Side Requirements:**
  * Modern Web Browser (Google Chrome 110+, Microsoft Edge 110+, Mozilla Firefox 110+, or Safari 16+)
  * Minimum Display Resolution: 1366 × 768 pixels (Desktop/Laptop) or 375 × 667 pixels (Mobile/Tablet)
  * Internet Connection: Active broadband or mobile data connection (minimum 2 Mbps recommended)
  * PDF Viewer: Built-in browser PDF engine or Adobe Acrobat Reader for official DepEd document exports

---

# TABLE OF CONTENTS

* **PART 1: PUBLIC PORTAL & APPLICANT REGISTRATION**
  * 1.1 Public Landing Page & Portal Navigation (`index.html`)
  * 1.2 User Authentication & Integrated Login Modal (`#authModal`)
  * 1.3 New Applicant Account Registration (`registration.html`)
  * 1.4 Online Learner Admission Form (SF1 Data Capture)
  * 1.5 Document Submission Scheduling & Appointment Booking (`#apptModal`)
  * 1.6 Online Application Tracker & Status Verification (`track.html`)
* **PART 2: ADMINISTRATOR PORTAL OPERATIONS**
  * 2.1 Administrator Master Dashboard & Analytics (`adminDashboard.html`)
  * 2.2 Online Applications Evaluation & Intake Verification (`applications.html`)
  * 2.3 Applicant Submitted Document Verification (`documents.html`)
  * 2.4 Document Verification Appointment Slots Management (`documentSlots.html`)
  * 2.5 Learner Master Directory & Profiles (`students.html`)
  * 2.6 Official DepEd 12-Digit LRN Update Modal (`#updateLrnModal`)
  * 2.7 Guardian/Parent Account Detachment & Unlinking (`#unlinkModal`)
  * 2.8 Section Directory & Class Capacity Management (`sections.html`)
  * 2.9 Drag-and-Drop Section Assignment Workspace (`sections.html`)
  * 2.10 DepEd Curriculum & Elementary Subject Management (`subjectManagement.html`)
  * 2.11 Faculty Directory & Teacher Profile Management (`teacherManagement.html`)
  * 2.12 Teacher Weekly Schedule & Timetable Modal (`#largeTeacherTimetableModal`)
  * 2.13 Master Section Schedules Grid (`scheduleManagement.html`)
  * 2.14 Class Timetable Builder & Conflict Detection Engine (`scheduleManagement.html`)
  * 2.15 User Account Administration & Role Permissions (`users.html`)
  * 2.16 System Security & Activity Audit Trail Logs (`auditLogs.html`)
  * 2.17 School Year Setup & Activation Readiness Audit (`settings.html`)
  * 2.18 Independent Admission & Enrollment Gating Controls (`settings.html`)
  * 2.19 Institutional DepEd Profile & Public CMS (`settings.html`)
  * 2.20 School Forms & Official Reports Center (`academicRecords.html`)
  * 2.21 DepEd SF4: Monthly Learner Movement & Attendance (`generate_sf4_pdf.php`)
  * 2.22 DepEd SF6: Summarized Report on Promotion & Proficiency (`generate_sf6_pdf.php`)
  * 2.23 DepEd SF7: School Personnel Assignment List & Profile (`generate_sf7_pdf.php`)
  * 2.24 DepEd SF10-ES: Learner Permanent Academic Record Workspace (`#workspace-sf10`)
  * 2.25 School Bulletins & Announcement Publishing (`announcements.html`)
  * 2.26 Synced Facebook Post Review & Lightbox Approval (`#reviewModal`)
* **PART 3: TEACHER & FACULTY PORTAL OPERATIONS**
  * 3.1 Faculty Dashboard & Advisory Overview (`teacherDashboard.html`)
  * 3.2 Advisory Class Learner Directory (`teacherDashboard.html`)
  * 3.3 Quarterly Grade Encoding Matrix (DepEd SF9) (`teacherDashboard.html`)
  * 3.4 Learner Promotion & Final Academic Status Evaluation (`teacherDashboard.html`)
  * 3.5 Teacher Teaching Program & Weekly Timetable View (`teacherDashboard.html`)
* **PART 4: STUDENT & PARENT PORTAL OPERATIONS**
  * 4.1 Student Portal Dashboard & Announcements (`studentDashboard.html`)
  * 4.2 Electronic Report Card (SF9) Quarterly Grade Viewer (`studentDashboard.html`)
  * 4.3 Continuing Learner Re-Enrollment Submission (`studentDashboard.html`)
  * 4.4 Student Profile & Emergency Contact Verification (`studentDashboard.html`)

---

# PART 1: PUBLIC PORTAL & APPLICANT REGISTRATION

---

### 1.1 Public Landing Page & Portal Navigation
**Header:** PUBLIC PORTAL  
**Figure 1. VPES-SIMS Public Landing Page Interface**  
> **Figure Description:** Capture the full desktop view of `index.html` displaying the Vinzons Pilot Elementary School hero banner, DepEd logo, primary navigation bar, latest announcement cards, admission announcement banner, and quick portal action buttons.

**Interface Controls & Elements:**
1. **School Brand & Navigation Bar** – Displays official VPES logo, DepEd School ID (112937), and fast navigation links to About, Announcements, Admissions, and Contact.
2. **Hero Call-to-Action (CTA) Buttons** – "Enroll Now" redirects new students to the registration portal; "Portal Login" triggers the integrated authentication modal.
3. **Admission Status Ribbon** – Real-time banner indicating whether Early Registration, Official Enrollment, or Re-enrollment is currently OPEN or CLOSED.
4. **School Bulletins & News Carousel** – Highlights official announcements and advisories broadcasted by the administration and synced with Facebook.
5. **Quick Application Tracker Bar** – Allows applicants to input their unique Reference Number to check application status without logging in.

---

### 1.2 User Authentication & Integrated Login Modal
**Header:** AUTHENTICATION  
**Figure 2. Integrated Portal Authentication Modal Dialog**  
> **Figure Description:** Capture `index.html` with the `#authModal` active on screen. The modal should show the email input field, password field with show/hide toggle, role-based login processor, forgot password link, and register redirect button.

**Interface Controls & Elements:**
1. **Email Address Field** – Input registered email address (e.g., student, parent, teacher, or administrator email).
2. **Password Field** – Input the secure account password.
3. **Show / Hide Password Icon** – Toggles password visibility to prevent typing errors.
4. **Log In Button** – Authenticates user credentials with Firebase Authentication and routes to the appropriate portal (Admin, Teacher, or Student).
5. **Forgot Password Link** – Dispatches an automated DepEd password reset verification link to the user's verified email.
6. **New Student Registration Link** – Redirects incoming parents and applicants to the account registration workflow.

---

### 1.3 New Applicant Account Registration
**Header:** REGISTRATION  
**Figure 3. Applicant Account Registration Interface**  
> **Figure Description:** Capture `registration.html` showing the account creation card with fields for Guardian Name, Email Address, Mobile Number, Password, Password Confirmation, and Terms of Agreement checkbox.

**Interface Controls & Elements:**
1. **Guardian / Applicant Full Name** – Full legal name of parent or guardian creating the portal account.
2. **Email Address Input** – Valid email address used for enrollment progress notifications, appointment confirmations, and password recovery.
3. **Mobile Contact Number** – 11-digit Philippine mobile number (`09XXXXXXXXX`) for urgent SMS advisories.
4. **Password & Confirmation Fields** – Minimum 8-character password with security requirements.
5. **Data Privacy Consent Checkbox** – Confirms user consent in compliance with the Philippine Republic Act 10173 (Data Privacy Act of 2012).
6. **Create Account Button** – Validates input, provisions the Firebase user account, and launches the online enrollment application form.

---

### 1.4 Online Learner Admission Form (SF1 Data Capture)
**Header:** ADMISSIONS  
**Figure 4. Online Student Application & SF1 Learner Information Form**  
> **Figure Description:** Capture the multi-section enrollment application interface showing Grade Level applied for, Learner Personal Information (Name, PSA Birth Certificate Number, Birth Date, Sex), Address details, and Parent/Guardian information.

**Interface Controls & Elements:**
1. **Grade Level & Enrollment Type Selector** – Choose incoming grade level (Kindergarten to Grade 6) and student status (New Learner, Transferee, or Balik-Aral).
2. **Learner Reference Number (LRN) Input** – 12-digit DepEd LRN (optional for incoming Kindergarten, mandatory for Grades 1–6 transferees).
3. **Learner Personal Details Form** – Fields for Last Name, First Name, Middle Name, Name Extension (Jr./III), Sex, and Birth Date.
4. **PSA Birth Certificate Registry Number** – Official birth registration number for DepEd identity verification.
5. **Residential Address & Contact Information** – House No., Street, Barangay, Municipality (Vinzons), and Province (Camarines Norte).
6. **Special Needs & Disability Checklist (BEEF Section 5)** – Diagnostic checkboxes for learners requiring Special Needs Education (SNEd) accommodations.
7. **Submit Application Button** – Encrypts and transmits the admission record to the administrative verification queue and generates a unique Application Reference Number (e.g., `APP-2026-XXXX`).

---

### 1.5 Document Submission Scheduling & Appointment Booking
**Header:** APPOINTMENTS  
**Figure 5. On-Site Physical Document Submission Appointment Scheduler**  
> **Figure Description:** Capture the appointment booking view on the applicant portal displaying the verified admission notification, the date selector dropdown with remaining slots, time window radio buttons, and the booking confirmation button.

**Interface Controls & Elements:**
1. **Verified Application Alert Banner** – Informs applicant that preliminary online application has been approved and physical verification is required.
2. **Appointment Date Selector Dropdown** – Dropdown list displaying approved submission dates with live available capacity (e.g., `Monday, November 9, 2026 — 30 slots left`).
3. **Session Window Selector** – Radio button selection for **Morning Session (8:00 AM – 12:00 PM)** or **Afternoon Session (1:00 PM – 5:00 PM)**.
4. **Document Checklist Indicator** – List of mandatory physical documents required upon visit (PSA Birth Certificate, Form 138/SF9 Report Card, 1x1 ID Photos).
5. **Book Appointment Button** – Submits selection and launches the Appointment Confirmation Slip Modal (`#apptModal`).
6. **Print Confirmation Slip Button** – Generates a printable PDF appointment slip displaying scheduled date, time window, applicant reference code, and QR verification stamp.

---

### 1.6 Online Application Tracker & Status Verification
**Header:** APPLICANT TRACKER  
**Figure 6. Universal Application Tracker & Progress Pipeline**  
> **Figure Description:** Capture `track.html` (or the tracking card on the applicant dashboard) showing the search input with a loaded application displaying the 4-step progress pipeline (Submitted, Under Review, Appointment Booked, Officially Enrolled).

**Interface Controls & Elements:**
1. **Application Reference Search Input** – Input field for the applicant's unique tracking code (e.g., `APP-2026-112937`).
2. **Track Status Button** – Queries the database and retrieves live enrollment status.
3. **Application Stage Pipeline Visualizer** – Step-by-step progress indicator:
   - *Step 1: Application Submitted* (Online form completed)
   - *Step 2: Under Administrative Review* (Registrar evaluating documents)
   - *Step 3: Document Verification Scheduled* (On-site appointment set)
   - *Step 4: Officially Enrolled* (LRN confirmed and section assigned)
4. **Remarks & Administrative Feedback Box** – Displays notes from the school registrar (e.g., "PSA Birth Certificate is blurred; please present original copy on appointment date").

---

# PART 2: ADMINISTRATOR PORTAL OPERATIONS

---

### 2.1 Administrator Master Dashboard & Analytics
**Header:** ADMIN DASHBOARD  
**Figure 7. Administrator Master KPI Analytics & Overview Hub**  
> **Figure Description:** Capture `adminDashboard.html` showing the top KPI summary metric cards (Total Enrolled, Pending Applications, Active Teachers, Class Sections), the enrollment trends graph, and quick action shortcuts.

**Interface Controls & Elements:**
1. **Top KPI Statistics Cards** – High-level summary metrics showing Total Enrolled Students, Pending Applications, Total Faculty Personnel, and Active Sections.
2. **Enrollment Distribution Chart** – Interactive visual graph showing learner headcount distribution per Grade Level (Kindergarten to Grade 6).
3. **Gender Ratio Metric Bar** – Visual distribution of Male vs. Female enrolled learners across the institution.
4. **Recent Activity Feed** – Live chronological preview of recent audit events, student applications, and grade submissions.
5. **Quick Navigation Shortcuts** – Direct access buttons to evaluate applications, create announcements, or generate DepEd school forms.

---

### 2.2 Online Applications Evaluation & Intake Verification
**Header:** APPLICATIONS  
**Figure 8. Administrator Applications Management & Evaluation Interface**  
> **Figure Description:** Capture `applications.html` displaying the application status filter tabs (All, Pending, Approved, Rejected), search bar, data table with applicant rows, and the Application Review Modal active.

**Interface Controls & Elements:**
1. **Status Filter Tabs** – Quick-filtering tabs: *Pending Review*, *Approved for Verification*, *Officially Enrolled*, and *Rejected / Incomplete*.
2. **Grade Level Dropdown Filter** – Filters applicants by incoming grade level (Kindergarten to Grade 6).
3. **Application Search Box** – Instant search by applicant name, reference number, or LRN.
4. **Applicant Review Button (`btn-review`)** – Opens the comprehensive Application Review Drawer/Modal displaying complete applicant profile and uploaded attachments.
5. **Approve Application Action** – Advances status to *Approved for Document Verification* and triggers an automated notification to the applicant.
6. **Reject / Return for Revision Action** – Prompts a feedback modal to specify deficiencies (e.g., incorrect grade level or missing signatures).

---

### 2.3 Applicant Submitted Document Verification
**Header:** DOCUMENTS  
**Figure 9. Submitted Document Verification Hub & PDF Viewer**  
> **Figure Description:** Capture `documents.html` showing the document status pills (Pending, Verified, Flagged), the document records table, and the inline image/PDF document preview drawer.

**Interface Controls & Elements:**
1. **Document Category Filter** – Filter records by document type: *PSA Birth Certificate*, *Form 138 / SF9*, *Good Moral Certificate*, or *Special Needs Medical Certification*.
2. **Document Record Table** – Lists applicant name, document type, date uploaded, and current verification status.
3. **Document Preview Button** – Launches the high-resolution lightbox viewer supporting JPG, PNG, and multi-page PDF documents.
4. **Mark as Verified Button** – Updates document state to *Verified*, recording the administrator ID and timestamp in the audit log.
5. **Reject / Request Re-upload Button** – Flags document as invalid or unreadable and opens an advisory prompt for applicant re-submission.

---

### 2.4 Document Verification Appointment Slots Management
**Header:** APPOINTMENT SLOTS  
**Figure 10. Administrator Appointment Capacity & Daily Slot Manager**  
> **Figure Description:** Capture `documentSlots.html` showing the school year selector, monthly date calendar/list, slot capacity configuration panel, and table of scheduled applicant appointments.

**Interface Controls & Elements:**
1. **School Year & Month Selectors** – Sets the active academic term and calendar month for physical document intake.
2. **Daily Capacity Configuration Inputs** – Fields to set maximum allowed appointments per day for Morning (AM) and Afternoon (PM) sessions.
3. **Date Lock / Blackout Toggle** – Locks specific dates (holidays, weekends, faculty training days) to prevent applicant bookings.
4. **Scheduled Appointments Table** – Displays confirmed appointments per day with applicant names, reference codes, and assigned time slots.
5. **Print Daily Appointment Schedule** – Exports the official daily visitor gate pass roster for school security personnel.

---

### 2.5 Learner Master Directory & Profiles
**Header:** STUDENTS  
**Figure 11. Student Master Directory and Demographic Data Table**  
> **Figure Description:** Capture `students.html` displaying the grade level filter pills, universal search input, the enrolled students table, and the action dropdown on a student row.

**Interface Controls & Elements:**
1. **Grade Level Filter Pills** – Instant filter buttons for Kindergarten, Grade 1, Grade 2, Grade 3, Grade 4, Grade 5, Grade 6, or All Learners.
2. **Universal Search Bar** – Fast lookup by 12-digit LRN, Student Full Name, or Assigned Section.
3. **Student Directory Table** – Columns displaying Student Name, 12-digit LRN, Sex, Grade Level, Current Section, and Enrollment Status.
4. **View Complete Profile Button** – Opens the full academic and demographic folder of the student.
5. **Update LRN Button** – Launches the DepEd LRN Assignment Modal (`#updateLrnModal`).
6. **Unlink Account Button** – Triggers the safety-gated guardian account detachment modal (`#unlinkModal`).

---

### 2.6 Official DepEd 12-Digit LRN Update Modal
**Header:** STUDENTS  
**Figure 12. DepEd 12-Digit LRN Update & Validation Modal**  
> **Figure Description:** Capture the `#updateLrnModal` on `students.html` showing the student's name, current LRN status (Temporary / Unassigned), the 12-digit numeric input field, validation badge, and Save button.

**Interface Controls & Elements:**
1. **Learner Demographic Summary** – Displays the selected student's full name, birth date, and current grade level.
2. **Official 12-Digit LRN Input** – Numeric input strictly restricted to exactly 12 digits, validated against standard DepEd LRN formatting rules.
3. **Format Validation Indicator** – Real-time badge that turns green upon entering exactly 12 digits and flags invalid characters or incorrect length.
4. **Save LRN Button** – Commits the official DepEd LRN to the `students` table, permanently upgrading the learner's temporary admission record.
5. **Cancel / Dismiss Button** – Closes the modal without saving modifications.

---

### 2.7 Guardian/Parent Account Detachment & Unlinking
**Header:** STUDENTS  
**Figure 13. Guardian Account Unlink Modal with Safety Countdown Timer**  
> **Figure Description:** Capture `#unlinkModal` on `students.html` showing the warning notification, details of the currently linked parent user account, the 5-second countdown lock on the confirm button, and the cancel button.

**Interface Controls & Elements:**
1. **Security Warning Alert** – Explains that unlinking detaches the student record from the parent's portal credentials, revoking their grade access until re-linked.
2. **Linked Guardian Information Card** – Displays current guardian name, verified email, and date of original account binding.
3. **5-Second Safety Lock Timer** – Disables the confirmation button for 5 seconds to prevent accidental or unauthorized clicks.
4. **Confirm Unlink Button** – Enables after the countdown finishes; clicking detaches the user ID from the student record and logs the event in audit logs.
5. **Cancel Button** – Closes the dialog immediately with zero alterations to the database.

---

### 2.8 Section Directory & Class Capacity Management
**Header:** SECTIONS  
**Figure 14. Class Section Directory & Classroom Capacity Interface**  
> **Figure Description:** Capture `sections.html` showing the Grade Level filter, section summary cards (Grade & Section Name, Room Number, Section Capacity bar, Class Adviser name), and the "Create New Section" modal.

**Interface Controls & Elements:**
1. **Grade Level Tab Bar** – Filters active sections by Kindergarten, Primary (Grades 1–3), and Intermediate (Grades 4–6).
2. **Create Section Button** – Opens modal to create a new section with Section Name, Grade Level, Room Number, and Maximum Capacity.
3. **Section Information Cards** – Visual cards displaying Section Name (e.g., *Grade 4 - Mabini*), Assigned Class Adviser, Room Location, and Total Students.
4. **Capacity Utilization Progress Bar** – Color-coded capacity meter (Green: Open slots; Amber: Approaching limit; Red: Full section at 45 pupils).
5. **Assign Students Tab (`tabBtnAssignStudents`)** – Switches to the interactive dual-panel drag-and-drop student sectioning workspace.

---

### 2.9 Drag-and-Drop Section Assignment Workspace
**Header:** SECTIONS  
**Figure 15. Dual-Panel Drag-and-Drop Section Assignment Workspace**  
> **Figure Description:** Capture the Assign Students tab on `sections.html` showing the left panel (Unassigned Students with Male/Female columns), the right panel (Target Section Roster), bulk checkboxes, and the publication status banner.

**Interface Controls & Elements:**
1. **Target Section Selector Dropdown** – Selects the class section receiving student assignments (e.g., *Grade 1 - Rizal*).
2. **Publication Status Ribbon** – Indicates whether current section assignments are in **DRAFT MODE** (internal view) or **PUBLISHED** (visible on student/teacher portals).
3. **Unassigned Pupils Panel (Left)** – Displays unassigned students filtered by grade level, neatly separated into **Male (Blue)** and **Female (Pink)** columns for gender balancing.
4. **Assigned Section Roster Panel (Right)** – Displays currently enrolled pupils in the selected section with live gender counts and total headcount.
5. **Drag-and-Drop & Bulk Checkboxes** – Drag individual student cards across panels, or check multiple pupils and click "Bulk Assign".
6. **Unassign Button (`×`)** – One-click button on assigned student cards to safely return a learner to the unassigned queue.
7. **Publish Section Roster Button** – Finalizes assignments and officially registers students into the DepEd master class enrollment database.

---

### 2.10 DepEd Curriculum & Elementary Subject Management
**Header:** SUBJECTS  
**Figure 16. DepEd Curriculum Subject Management Interface**  
> **Figure Description:** Capture `subjectManagement.html` displaying the Active Curriculum vs. Archived Subjects tabs, grade level filter, subject cards with Subject Code and Units, and the Add/Edit Subject Modal (`#subjectModal`).

**Interface Controls & Elements:**
1. **Curriculum View Tabs** – Toggle between **Active Curriculum Subjects** and **Archived Subjects**.
2. **Grade Level Filter Bar** – Filters elementary learning areas by Grade Level (Kindergarten, Grades 1 to 6).
3. **Add New Subject Button** – Opens `#subjectModal` to register a standard DepEd elementary subject.
4. **Add/Edit Subject Modal (`#subjectModal`) Form Fields:**
   - *Subject Name* (e.g., *Mathematics*, *Araling Panlipunan*)
   - *Subject Code* (e.g., *MATH4*, *AP4*)
   - *Grade Level* (Assigned elementary grade)
   - *Units / Weight* (Standard curriculum credit units)
   - *Description* (Official DepEd learning competency overview)
5. **Archive Subject Button** – Safely deactivates subjects without deleting historical learner grade records.
6. **Restore Subject Button** – Restores previously archived subjects back to active curriculum status.

---

### 2.11 Faculty Directory & Teacher Profile Management
**Header:** TEACHERS  
**Figure 17. Faculty Directory & Grade Cluster Profile Management**  
> **Figure Description:** Capture `teacherManagement.html` showing the faculty cluster filter pills (All, Kindergarten, Primary, Intermediate), the teacher profile cards, and the Add Teacher Modal (`#addTeacherModal`).

**Interface Controls & Elements:**
1. **Faculty Cluster Filter Pills** – Quick filter by teaching assignment: *All Faculty*, *Kindergarten Cluster*, *Primary Cluster (Grades 1–3)*, or *Intermediate Cluster (Grades 4–6)*.
2. **Add Teacher Button** – Launches `#addTeacherModal` to register an existing user account into the official faculty directory.
3. **Teacher Account Selector Dropdown** – Selects an authenticated user from the system dropdown (`#teacherAccount`), auto-populating read-only name fields.
4. **Handled Grade Cluster & Specialization** – Sets teaching cluster and subject specialization (e.g., *English & Reading Specialist*).
5. **Teacher Profile Cards** – Displays teacher photo/avatar, DepEd Employee ID, Specialization, Assigned Advisory Section, and Status.
6. **View Timetable Button** – Launches the Large Teacher Timetable Modal (`#largeTeacherTimetableModal`) displaying the teacher's full weekly schedule.

---

### 2.12 Teacher Weekly Schedule & Timetable Modal
**Header:** TEACHERS  
**Figure 18. Large Teacher Timetable Modal with Weekly Class Schedule**  
> **Figure Description:** Capture `#largeTeacherTimetableModal` on `teacherManagement.html` showing the teacher's weekly 5-day schedule grid (Monday to Friday, 7:00 AM – 5:00 PM), subject blocks with section labels, and the Print Timetable button.

**Interface Controls & Elements:**
1. **Teacher Identification Header** – Displays teacher full name, employee number, specialization, and total assigned teaching minutes per week.
2. **Weekly Timetable Grid** – 5-column calendar grid (Monday to Friday) with time intervals from 7:00 AM to 5:00 PM.
3. **Scheduled Class Blocks** – Color-coded subject blocks displaying Subject Title, Grade & Section, and Assigned Classroom.
4. **Advisory Section Indicator** – Highlights periods where the teacher acts as official homeroom class adviser.
5. **Print Schedule Button** – Formats the weekly timetable into official DepEd SF7 individual program format for printing and division submission.
6. **Close Modal Button** – Dismisses the timetable modal viewer.

---

### 2.13 Master Section Schedules Grid
**Header:** SCHEDULES  
**Figure 19. Master Section Schedules Grid & Class Timetable Hub**  
> **Figure Description:** Capture Tab 1 on `scheduleManagement.html` showing the grade level filter pills, the Master Section Timetable cards grid, search bar, and schedule publication status badge.

**Interface Controls & Elements:**
1. **Master Schedules Tab (Tab 1)** – Default view displaying complete weekly timetables across all active sections in the institution.
2. **Grade Level & Search Filter** – Filters schedule cards by specific grade levels or section names.
3. **Section Schedule Cards** – Visual cards summarizing weekly subject load, total instructional minutes, and publication status per section.
4. **Publication Status Toggle** – Allows administrator to publish section schedules school-wide or keep them in draft mode during planning.
5. **Switch to Schedule Builder (Tab 2)** – Button to transition into the interactive schedule session creator and conflict checking engine.

---

### 2.14 Class Timetable Builder & Conflict Detection Engine
**Header:** SCHEDULES  
**Figure 20. Interactive Class Timetable Builder with Automated Conflict Detection**  
> **Figure Description:** Capture Tab 2 on `scheduleManagement.html` showing the left panel (Session Creator form with Start Time, Duration, Days checkboxes, Teacher dropdown), the right panel (5-Day Weekly Timetable Grid), and the Conflict Warning Modal.

**Interface Controls & Elements:**
1. **Target Section Selector** – Choose the target section being scheduled (e.g., *Grade 5 - Bonifacio*).
2. **Create Session Form (Left Panel):**
   - *Subject Dropdown* (Curriculum subjects for that grade level)
   - *Assigned Teacher Dropdown* (Qualified faculty personnel)
   - *Start Time Picker* (e.g., `08:00 AM`)
   - *Duration in Minutes* (e.g., `50` minutes)
   - *Day of Week Checkboxes* (Select Monday, Tuesday, Wednesday, Thursday, Friday)
3. **Real-Time Automated Conflict Detection Engine** – Instantly validates whether:
   - The selected Teacher is already scheduled in another section at the same time.
   - The Section already has an overlapping subject during that time window.
4. **Collision Warning Alert Modal** – Flashes a red warning banner if an overlap occurs, blocking the entry and specifying the conflicting teacher and section.
5. **Weekly Schedule Grid (Right Panel)** – Interactive visual grid displaying time blocks; allows clicking existing blocks to edit or delete.
6. **Auto-Generate Missing Subjects Button** – Automatically populates timetable gaps based on DepEd curriculum minimum time allocations.
7. **Auto-Assign Teachers Button** – Intelligently assigns qualified teachers based on cluster specializations.
8. **Save Draft / Finalize Schedule Buttons** – Commits the weekly timetable to the database.

---

### 2.15 User Account Administration & Role Permissions
**Header:** USERS  
**Figure 21. System User Accounts Management & Security Roles Directory**  
> **Figure Description:** Capture `users.html` showing the user role filter pills (All, Administrator, Teacher, Student/Parent), user search box, user accounts table with status toggles, and the Add New User modal.

**Interface Controls & Elements:**
1. **Role Filter Pills** – Categorizes user accounts by system role: *All Users*, *System Administrator*, *Teacher / Faculty*, and *Student / Parent*.
2. **User Search Bar** – Instant search by user display name, registered email, or user ID.
3. **User Accounts Data Table** – Displays Avatar, Full Name, Email Address, Assigned System Role, Account Creation Date, and Status (Active/Suspended).
4. **Add New User Button** – Launches modal to provision a new administrative or faculty account with assigned permissions.
5. **Edit Role / Permissions Action** – Modifies role designations and administrative access rights.
6. **Account Status Toggle** – Instant toggle switch to activate or suspend user login credentials.
7. **Reset Password Dispatcher** – Triggers an official password reset email to the user.

---

### 2.16 System Security & Activity Audit Trail Logs
**Header:** AUDIT LOGS  
**Figure 22. System Security Audit & Activity Logs Interface**  
> **Figure Description:** Capture `auditLogs.html` showing the 5 KPI summary cards at the top, the category filter pills, search input, date range filter, the audit trail data table, and the Audit Event Detail modal (`#auditDetailModal`).

**Interface Controls & Elements:**
1. **Top KPI Summary Cards** – Real-time counts for *Total Logged Events*, *Actions Today*, *Re-Enrollment Events*, *Admissions Events*, and *Security & Settings Events*.
2. **Universal Audit Search Bar (`#auditSearchInput`)** – Filters logs by student name, 12-digit LRN, administrator name, or event description.
3. **Category Quick-Filter Pills** – Filter stream by *All Logs*, *Re-Enrollment*, *Admissions*, *Documents*, *Users & Security*, *Sections & Schedules*, or *System Settings*.
4. **Date Range Filter Dropdown (`#auditDateFilter`)** – Preset date filtering (*All Time*, *Today*, *Yesterday*, *Last 7 Days*, *Last 30 Days*, or *Custom Date Range*).
5. **Audit Trail Data Table** – Columns for **Date & Time** (with relative time badge), **Event Action** (with category badge), **Description & Details** (with smart entity highlighting), and **Performed By** (with user role and avatar).
6. **Audit Event Detail Modal (`#auditDetailModal`)** – Clicking any row opens this modal to inspect programmatic action codes, performer email, full description, and linked Application ID references.
7. **Live Refresh Button (`#btnRefreshLogs`)** – Polls and loads newly logged events without reloading the page.

---

### 2.17 School Year Setup & Activation Readiness Audit
**Header:** SETTINGS  
**Figure 23. School Year Management & Activation Readiness Audit Interface**  
> **Figure Description:** Capture Tab 1 on `settings.html` showing the Active School Year banner, historical school years table, "Add School Year" modal, and the automated "Activation Readiness Audit" dialog with verification checklist.

**Interface Controls & Elements:**
1. **Active School Year Display Banner** – Identifies current active DepEd academic term (e.g., *S.Y. 2026–2027*).
2. **Add School Year Button** – Launches dialog to define a new academic year with official Term Start Date and Term End Date.
3. **Historical School Years Table** – Catalogs past academic years, enrollment totals, and archiving status.
4. **Check Activation Readiness Button** – Runs an automated institutional readiness engine before activating a new school year:
   - Verifies all students in active sections have finalized 4th-quarter grades.
   - Confirms Grade 6 student graduations and general promotions are complete.
   - Validates that new grade sections and curriculum subjects exist for the new year.
5. **Readiness Checklist & Resolution Prompt** – Displays itemized checklist; enables "Activate School Year" button only when all critical criteria pass.

---

### 2.18 Independent Admission & Enrollment Gating Controls
**Header:** SETTINGS  
**Figure 24. Independent Admission & Enrollment Gating Switches**  
> **Figure Description:** Capture the three independent gating cards on `settings.html` showing the toggle switches (ON/OFF), calendar start/end date selectors, and public advisory message boxes.

**Interface Controls & Elements:**
1. **Early Registration Gating Switch** – Toggles pre-registration **ON/OFF** for incoming Kindergarten and Grade 1 applicants.
2. **Official General Enrollment Switch** – Toggles general enrollment **ON/OFF** for all grade levels across the public portal.
3. **Student Re-Enrollment Gating Switch** – Controls whether the **"Re-Enrollment"** tab is active and accepting submissions on continuing student dashboards.
4. **Start & End Calendar Date Pickers** – Automates scheduled portal opening and closing based on DepEd official calendar dates.
5. **Portal Advisory Notice Customizer** – Text input to customize the public advisory message displayed to parents when enrollment is closed.

---

### 2.19 Institutional DepEd Profile & Public CMS
**Header:** SETTINGS  
**Figure 25. School Profile & Institutional DepEd Identifiers Interface**  
> **Figure Description:** Capture Tab 2 on `settings.html` showing the official DepEd Institutional Profile form (School Name, School ID 112937, Principal Name, Division, Region, Address, and Logo uploader).

**Interface Controls & Elements:**
1. **DepEd School ID Input** – Read-only / configured institutional identifier (`112937`).
2. **Official School Name** – *Vinzons Pilot Elementary School*.
3. **Administrative Identifiers** – Fields for School Principal Name, DepEd Division (*Camarines Norte*), and Region (*Region V - Bicol*).
4. **Official School Seal & Logo Uploader** – Uploads high-resolution school seal rendered on report cards and official certificates.
5. **Contact & Social Media Links** – Sets public contact email, office telephone, and official Facebook Page URL.
6. **Save Profile Button** – Commits institutional details across all portal footers and DepEd official report headers.

---

### 2.20 School Forms & Official Reports Center
**Header:** ACADEMIC REPORTS  
**Figure 26. School Forms & Official Reports Center Catalog Hub**  
> **Figure Description:** Capture `academicRecords.html` showing the header with Refresh button and the catalog of the 4 active DepEd School Forms cards (SF4, SF6, SF7, and SF10-ES).

**Interface Controls & Elements:**
1. **Page Title & Header Toolbar** – Displays "School Forms & Official Reports Center" with a live Refresh button.
2. **SF4: Monthly Learner Movement Card** – Displays description, badges (*Monthly Aggregate*, *School-Wide*), and the **"View & Download SF4"** action button.
3. **SF6: Promotion & Proficiency Summary Card** – Displays description, badges (*End of School Year*, *Consolidated*), and the **"View & Download SF6"** action button.
4. **SF7: School Personnel Assignment List Card** – Displays description, badges (*Class Schedule*, *Faculty Profile*), and the **"View & Download SF7"** action button.
5. **SF10-ES: Learner Permanent Academic Record Card** – Displays description, badges (*Multi-Year Cumulative*, *Active & Alumni*), and the **"Open SF10 Generator"** action button.

---

### 2.21 DepEd SF4: Monthly Learner Movement & Attendance
**Header:** ACADEMIC REPORTS  
**Figure 27. DepEd SF4 Monthly Movement & Attendance PDF Viewer Modal**  
> **Figure Description:** Capture the `#sf10ModalOverlay` active after clicking "View & Download SF4" on `academicRecords.html`, showing the embedded PDF viewer displaying the official SF4 matrix, month/year metadata, and the PDF/Excel download buttons in the modal footer.

**Interface Controls & Elements:**
1. **Modal Header & Metadata** – Displays "Monthly Report on Learner Movement & Attendance (SF4)", reporting month, and active school year.
2. **Close Modal Button (`ri-close-line`)** – Top-right close button to dismiss the viewer.
3. **Embedded Official PDF Viewer Iframe** – Live interactive PDF preview displaying consolidated registered learners, daily attendance averages, dropouts, and transfers across all sections.
4. **Download PDF Button** – Downloads the official legal-sized DepEd SF4 PDF directly to the local computer.
5. **Download Excel (.xlsx) Button** – Exports the raw consolidated data into an editable official DepEd Excel spreadsheet.

---

### 2.22 DepEd SF6: Summarized Report on Promotion & Proficiency
**Header:** ACADEMIC REPORTS  
**Figure 28. DepEd SF6 Summarized Promotion & Level of Proficiency Modal**  
> **Figure Description:** Capture `#sf10ModalOverlay` displaying the SF6 official matrix, showing student promotion totals, retention counts, and learning progress distributions (Did Not Meet Expectations to Outstanding) across Grades 1 to 6.

**Interface Controls & Elements:**
1. **Modal Title Bar** – Displays "Summarized Report on Promotion & Level of Proficiency (SF6) | Consolidated School Matrix (Grades 1–6)".
2. **Consolidated Statistical Matrix Preview** – Live PDF preview of the official replacement for DepEd Form 20, itemized by grade level and gender.
3. **Proficiency Distribution Table** – Renders counts for:
   - *Did Not Meet Expectations (Below 75)*
   - *Fairly Satisfactory (75–79)*
   - *Satisfactory (80–84)*
   - *Very Satisfactory (85–89)*
   - *Outstanding (90–100)*
4. **Download PDF Button** – Downloads the finalized SF6 report in standard DepEd print-ready PDF format.
5. **Download Excel (.xlsx) Button** – Exports the statistical matrix into an official DepEd `.xlsx` spreadsheet.

---

### 2.23 DepEd SF7: School Personnel Assignment List & Profile
**Header:** ACADEMIC REPORTS  
**Figure 29. DepEd SF7 School Personnel Assignment List & Basic Profile Modal**  
> **Figure Description:** Capture `#sf10ModalOverlay` displaying the official DepEd SF7 form, showing faculty names, plantilla items, educational attainment, teaching designations, and weekly instructional minute loads.

**Interface Controls & Elements:**
1. **Modal Header & School Year Indicator** – Displays "School Personnel Assignment List and Basic Profile (SF7) | S.Y. 2026–2027".
2. **Personnel Roster & Plantilla Table** – Renders teacher names, employee IDs, Civil Service eligibility, and highest educational degree completed.
3. **Daily Instructional Class Program** – Details daily teaching schedules, subjects handled per section, and total teaching minutes per week.
4. **School Head Certification Block** – Official signature line for the School Principal / Head Teacher.
5. **Download PDF & Download Excel Buttons** – Export buttons for printing or division electronic submission.

---

### 2.24 DepEd SF10-ES: Learner Permanent Academic Record Workspace
**Header:** ACADEMIC REPORTS  
**Figure 30. DepEd SF10-ES Permanent Academic Records Workspace & Roster**  
> **Figure Description:** Capture the `#workspace-sf10` view on `academicRecords.html` showing the 3 roster scope cards (Currently Enrolled, Graduated / Alumni, Master Archive), grade level pills, universal search, learner table, and "View SF10" button.

**Interface Controls & Elements:**
1. **Back to Reports Catalog Button** – Returns user to the main School Forms catalog hub.
2. **Roster Scope Cards & Switcher:**
   - *Currently Enrolled* (Active learners in current school year)
   - *Graduated / Alumni* (Learners who finished Grade 6)
   - *Master Learner Archive* (All historical registered learners)
3. **Universal Learner Search Box** – Fast search by student name, 12-digit LRN, or section name.
4. **Grade Level Quick-Filter Pills** – Filter roster by All Grades, Kindergarten, or Grades 1 to 6.
5. **Learner Scholastic Registry Table** – Columns for Learner Info, 12-digit LRN, Grade & Section, and Grade Coverage.
6. **View SF10 Action Button** – Launches the live SF10-ES PDF preview modal displaying multi-year scholastic marks from Kindergarten to Grade 6 (formerly Form 137).
7. **Export Options** – Download official permanent records in print-ready legal PDF or Excel spreadsheet formats.

---

### 2.25 School Bulletins & Announcement Publishing
**Header:** ANNOUNCEMENTS  
**Figure 31. Administrator Announcements Management & Creation Modal**  
> **Figure Description:** Capture `announcements.html` showing the active announcements list, priority pinned bulletins, and the Create Announcement modal active with Title, Category, Content editor, and Auto-Post to Facebook toggle.

**Interface Controls & Elements:**
1. **Create Announcement Button** – Opens modal to author a new school bulletin.
2. **Title & Category Selectors** – Enter announcement headline and select category: *General Advisory*, *Academic News*, *Emergency Suspension*, or *DepEd Memorandum*.
3. **Target Audience Radios** – Target announcement to *Public*, *All Students & Parents*, or *Faculty Only*.
4. **Content Rich-Text Editor** – Formats announcement message body and bullet points.
5. **Priority Pinning Toggle** – Pins urgent bulletins to the top of the portal feed and marks them with a high-priority red badge.
6. **Auto-Post to Facebook Toggle** – Synchronizes and publishes the announcement simultaneously to the official Vinzons Pilot Elementary School Facebook page.
7. **Publish Announcement Button** – Immediately broadcasts the advisory across selected channels.

---

### 2.26 Synced Facebook Post Review & Lightbox Approval
**Header:** ANNOUNCEMENTS  
**Figure 32. Facebook Synced Post Review & Approval Lightbox**  
> **Figure Description:** Capture the `#reviewModal` on `announcements.html` displaying the two-column review interface: Facebook post preview on the left, and portal publishing configuration controls on the right.

**Interface Controls & Elements:**
1. **Pending Review Tab (`tabPending`)** – Displays incoming Facebook Page posts captured via webhook awaiting administrative approval.
2. **Facebook Post Source Panel (Left)** – Displays raw Facebook post text, original publishing timestamp, and attached graphics.
3. **Portal Formatting Panel (Right)** – Allows administrator to adjust announcement title, select school portal category, and edit description text.
4. **Approve & Publish to Portal Button** – Immediately approves the post, displaying it on the public landing page feed.
5. **Dismiss / Reject Post Button** – Removes the synced post from the queue without showing it on the portal.

---

# PART 3: TEACHER & FACULTY PORTAL OPERATIONS

---

### 3.1 Faculty Dashboard & Advisory Overview
**Header:** TEACHER PORTAL  
**Figure 33. Faculty Portal Dashboard & Teaching Assignment Overview**  
> **Figure Description:** Capture `teacherDashboard.html` showing the teacher welcome card, DepEd employee info, advisory section badge, summary statistics of handled pupils, and quick links to grade encoding.

**Interface Controls & Elements:**
1. **Teacher Profile Header Card** – Displays teacher photo, full name, DepEd employee ID, and cluster designation.
2. **Advisory Section Summary Card** – Displays assigned homeroom section (e.g., *Grade 4 - Mabini*), room number, and total pupil count.
3. **Teaching Load Quick-Metrics** – Total subjects handled, weekly teaching minutes, and grade encoding completion percentage.
4. **Class Advisory Roster Shortcut** – One-click button navigating directly to the homeroom student list.
5. **Grade Encoding Quick-Launch** – Direct shortcut to the quarterly grade matrix for assigned subjects.

---

### 3.2 Advisory Class Learner Directory
**Header:** TEACHER PORTAL  
**Figure 34. Class Advisory Pupil Directory & Contact Roster**  
> **Figure Description:** Capture the Advisory Class tab on `teacherDashboard.html` showing the pupil roster table separated by Male and Female learners, showing 12-digit LRNs, birth dates, guardian names, and contact numbers.

**Interface Controls & Elements:**
1. **Section Metadata Header** – Displays Grade Level, Section Name, and total registered learners.
2. **Gender Breakdown Indicators** – Displays count of Male learners and Female learners.
3. **Pupil Directory Table** – Lists pupil names alphabetically (Males first, then Females in DepEd format) with 12-digit LRN, Age, and Address.
4. **Parent / Guardian Contact Info** – Direct phone numbers and email addresses for emergency contact.
5. **Learner Academic Profile Button** – Opens individual student performance summaries and attendance cards.

---

### 3.3 Quarterly Grade Encoding Matrix (DepEd SF9)
**Header:** GRADING  
**Figure 35. DepEd SF9 Quarterly Grade Encoding Matrix Interface**  
> **Figure Description:** Capture the grading interface on `teacherDashboard.html` showing the Subject and Section selectors, Quarter filter (Q1, Q2, Q3, Q4), student grade input grid with auto-calculation of General Average and Remarks (Passed/Failed), and the Save Grades button.

**Interface Controls & Elements:**
1. **Section & Subject Selectors** – Choose the class section and learning area being graded (e.g., *Grade 4 - Mabini | Mathematics*).
2. **Quarter Selector Tabs** – Toggle between **1st Quarter**, **2nd Quarter**, **3rd Quarter**, and **4th Quarter**.
3. **Grade Input Fields** – Numeric input cells restricted to valid Philippine elementary grading scale (60 to 100).
4. **Real-Time Final Rating Calculator** – Automatically computes final rating across all 4 quarters:
   $$\text{Final Rating} = \frac{Q1 + Q2 + Q3 + Q4}{4}$$
5. **Automated Remarks Generator** – Displays **"Passed"** for grades $\ge 75$ or **"Failed"** for grades $< 75$.
6. **Save Draft Grades Button** – Saves current encoded grades to database without locking.
7. **Submit & Finalize Grades Button** – Locks the quarterly grading sheet and submits marks to the registrar for report card generation.

---

### 3.4 Learner Promotion & Final Academic Status Evaluation
**Header:** GRADING  
**Figure 36. End-of-School-Year Learner Promotion & Proficiency Evaluation**  
> **Figure Description:** Capture the end-of-year promotion tab on `teacherDashboard.html` showing the consolidated general averages, DepEd proficiency descriptors, and promotion status dropdown (Promoted, Retained, Conditional).

**Interface Controls & Elements:**
1. **Learner General Average Summary** – Displays overall general average across all DepEd curriculum subjects.
2. **DepEd Proficiency Level Descriptors:**
   - *Outstanding (90–100)*
   - *Very Satisfactory (85–89)*
   - *Satisfactory (80–84)*
   - *Fairly Satisfactory (75–79)*
   - *Did Not Meet Expectations (Below 75)*
3. **Promotion Status Selector** – Dropdown options: **Promoted** (passed all subjects), **Conditional** (lacking 1–2 learning areas), or **Retained** (failed 3 or more subjects).
4. **Adviser Endorsement Remarks** – Input field for homeroom adviser's end-of-year character narrative.
5. **Submit Final Promotion Roster Button** – Submits official section promotion data into the school-wide SF6 compilation engine.

---

### 3.5 Teacher Teaching Program & Weekly Timetable View
**Header:** TEACHER PORTAL  
**Figure 37. Faculty Personal Weekly Teaching Timetable Schedule**  
> **Figure Description:** Capture the My Schedule tab on `teacherDashboard.html` showing the teacher's weekly subject distribution grid across all handled sections, classroom numbers, and daily instructional time.

**Interface Controls & Elements:**
1. **Weekly Program Calendar View** – Monday to Friday schedule grid with colored class blocks.
2. **Class Block Details** – Displays subject name, section, room number, and exact time window (e.g., *08:00 AM – 08:50 AM | Science 4 | Section Diamond*).
3. **Advisory Homeroom Time Block** – Highlights designated homeroom guidance and flag ceremony periods.
4. **Weekly Instructional Load Meter** – Displays total rendered teaching minutes vs. official DepEd standard teaching load.
5. **Print Schedule Action** – Generates a clean PDF copy for classroom posting.

---

# PART 4: STUDENT & PARENT PORTAL OPERATIONS

---

### 4.1 Student Portal Dashboard & Announcements
**Header:** STUDENT PORTAL  
**Figure 38. Student & Parent Portal Home Dashboard**  
> **Figure Description:** Capture `studentDashboard.html` showing the learner's welcome banner, 12-digit LRN badge, currently enrolled grade and section, class adviser details, school announcements feed, and quick links.

**Interface Controls & Elements:**
1. **Learner Header Card** – Displays student full name, 12-digit LRN, student ID, and enrolled academic year.
2. **Current Section & Adviser Card** – Displays enrolled Grade Level, Section Name, Classroom location, and Class Adviser name with contact link.
3. **School Bulletins & News Feed** – Live stream of official VPES announcements, event notices, and emergency suspension alerts.
4. **Attendance Overview Meter** – Monthly days present, days absent, and attendance percentage.
5. **Portal Navigation Tabs** – Fast navigation to **My Grades (SF9)**, **Re-Enrollment**, and **My Profile**.

---

### 4.2 Electronic Report Card (SF9) Quarterly Grade Viewer
**Header:** STUDENT PORTAL  
**Figure 39. Electronic Progress Report Card (DepEd SF9) Viewer**  
> **Figure Description:** Capture the Grades tab on `studentDashboard.html` displaying the official DepEd SF9 electronic report card matrix with learning areas, Q1–Q4 ratings, Final Rating, Remarks, and the Print/Download SF9 button.

**Interface Controls & Elements:**
1. **Official DepEd SF9 Header** – Displays Region V, Division of Camarines Norte, Vinzons Pilot Elementary School (School ID: 112937).
2. **Curriculum Learning Areas Column** – Lists all DepEd subjects: *Mother Tongue*, *Filipino*, *English*, *Mathematics*, *Science*, *Araling Panlipunan (AP)*, *Edukasyon sa Pagpapakatao (EsP)*, and *MAPEH (Music, Arts, PE, Health)*.
3. **Quarterly Grades (Q1 to Q4)** – Displays released numeric grades per quarter once finalized by teachers.
4. **Final Rating & Remarks Column** – Reflects weighted final grade and official DepEd status (*Passed* / *Failed*).
5. **Learner General Average Box** – Highlights overall general academic average for the school year.
6. **Download / Print Report Card Button** – Exports the official SF9 report card into a clean, printable PDF format.

---

### 4.3 Continuing Learner Re-Enrollment Submission
**Header:** RE-ENROLLMENT  
**Figure 40. Continuing Learner Online Re-Enrollment Submission Interface**  
> **Figure Description:** Capture the Re-Enrollment tab on `studentDashboard.html` showing the incoming school year notification, pre-populated learner details, target grade level, emergency contact update inputs, and the "Submit Re-Enrollment" button.

**Interface Controls & Elements:**
1. **Re-Enrollment Eligibility Status Banner** – Indicates whether student is cleared for re-enrollment based on promotion status and active school year gating.
2. **Pre-Populated Learner Information** – Automatically loads student 12-digit LRN, legal name, and completed grade level.
3. **Target Incoming Grade Level** – Automatically identifies next grade level (e.g., promoted from Grade 3 to Grade 4).
4. **Contact & Address Update Fields** – Allows parents to update current residential address and active emergency phone numbers.
5. **Special Needs & Health Update Checkbox** – Allows reporting newly diagnosed medical or learning conditions.
6. **Submit Re-Enrollment Application Button** – Transmits continuation intent directly to the registrar's intake queue with zero paper forms required.

---

### 4.4 Student Profile & Emergency Contact Verification
**Header:** STUDENT PROFILE  
**Figure 41. Student Profile & Emergency Contact Verification Interface**  
> **Figure Description:** Capture the Profile tab on `studentDashboard.html` showing the learner's demographic details, PSA registry number, parent/guardian information, and account security settings.

**Interface Controls & Elements:**
1. **Learner Demographic Details Card** – Read-only display of official legal name, sex, birth date, and verified PSA birth certificate number.
2. **Permanent Address Card** – Registered residential address in Vinzons, Camarines Norte.
3. **Parent / Guardian Details** – Father's Name, Mother's Maiden Name, Guardian Name, and registered phone numbers.
4. **Account Security & Password Management** – Interface allowing user to update their portal account password.
5. **Sign Out Action Button** – Safely ends the portal session, clearing cached authentication tokens.

---
*(End of User Manual Appendix – Document verified for Vinzons Pilot Elementary School – SIMS)*

