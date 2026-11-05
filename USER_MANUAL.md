# VINZONS PILOT ELEMENTARY SCHOOL
## STUDENT INFORMATION AND MANAGEMENT SYSTEM (VPES-SIMS)
### OFFICIAL SYSTEM USER MANUAL & OPERATIONAL GUIDE

---

**Document Identifier:** VPES-SIMS-UM-2026-V1  
**Target System:** Vinzons Pilot Elementary School – Student Information and Management System (VPES-SIMS)  
**Institutional Affiliation:** Department of Education (DepEd) • Region V (Bicol) • Division of Camarines Norte • District of Vinzons  
**School Identification:** DepEd School ID: 112937  
**Academic Year:** S.Y. 2026–2027  
**Publication Date:** November 2026  
**Document Classification:** Official Academic & Institutional User Documentation  

---

## TABLE OF CONTENTS

1. [Chapter 1: Introduction and System Overview](#chapter-1-introduction-and-system-overview)
   - 1.1 Purpose of the User Manual
   - 1.2 System Identification and Institutional Profile
   - 1.3 System Objectives and Tangible Benefits
   - 1.4 Scope and Limitations
   - 1.5 System Architecture, RBAC, and Security Framework
2. [Chapter 2: System Requirements and Getting Started](#chapter-2-system-requirements-and-getting-started)
   - 2.1 Hardware Requirements
   - 2.2 Software and Supported Web Browsers
   - 2.3 Network and Connectivity Standards
   - 2.4 Accessing the Web Portal
3. [Chapter 3: User Accounts, Authentication, and Security](#chapter-3-user-accounts-authentication-and-security)
   - 3.1 User Roles and Access Permission Matrix
   - 3.2 Account Registration and 6-Digit OTP Verification
   - 3.3 User Sign-In (Email/Password and Google OAuth)
   - 3.4 Role-Based Automatic Redirection
   - 3.5 Mandatory First-Login Password Change Procedure
   - 3.6 Password Recovery (Forgot Password via Email/SMS)
   - 3.7 Session Management and Secure Sign-Out
4. [Chapter 4: Public and Guest User Portal](#chapter-4-public-and-guest-user-portal)
   - 4.1 Navigating the Landing Page Interface
   - 4.2 Checking Admission and Enrollment Gating Status
   - 4.3 Reading School Announcements and DepEd Bulletins
   - 4.4 Data Privacy Policy and Terms of Use
5. [Chapter 5: Applicant and Parent/Guardian Portal (Admissions)](#chapter-5-applicant-and-parentguardian-portal-admissions)
   - 5.1 Student Type Selection (New Applicant vs. Existing Student)
   - 5.2 Linking an Existing Student Record via 12-Digit LRN
   - 5.3 Step-by-Step Online Admission Application (DepEd BEEF Compliance)
   - 5.4 Uploading Required Admission Documents
   - 5.5 Reviewing, Certifying Data Privacy, and Submitting the Application
   - 5.6 Understanding the Application Reference Number
   - 5.7 Navigating the Applicant Dashboard and 5-Stage Timeline
   - 5.8 Booking an On-Site Physical Document Submission Appointment Slot
   - 5.9 Downloading and Printing the Official Appointment Slip
   - 5.10 Responding to Document Correction and Re-upload Requests
6. [Chapter 6: Enrolled Student Portal](#chapter-6-enrolled-student-portal)
   - 6.1 Navigating the Enrolled Student Dashboard
   - 6.2 Viewing the Weekly Interactive Class Schedule
   - 6.3 Accessing Quarterly Academic Grades and Performance
   - 6.4 Viewing and Verifying Student Profile Information
   - 6.5 Submitting Continuing Student Re-Enrollment
   - 6.6 Alumni / Graduated Student Interface
7. [Chapter 7: Teacher and Class Adviser Portal](#chapter-7-teacher-and-class-adviser-portal)
   - 7.1 Navigating the Teacher Dashboard
   - 7.2 Managing Advisory Class Student Rosters
   - 7.3 Operating the Teacher Quarterly Grading Sheet
   - 7.4 Using the MAPEH Component Breakdown Modal
   - 7.5 Viewing and Printing the Individual Teaching Schedule
   - 7.6 Generating Official DepEd School Forms (SF1, SF2, SF3, SF5, SF8, SF9)
   - 7.7 Managing Teacher Profile and Password Credentials
8. [Chapter 8: Administrator and Registrar Portal](#chapter-8-administrator-and-registrar-portal)
   - 8.1 Executive Dashboard and Real-Time KPI Metrics
   - 8.2 Managing Admissions and Application Lifecycles
   - 8.3 Managing Re-Enrollment Requests and Bulk Approvals
   - 8.4 Executing Student Year-End Promotion and Grade 6 Graduation
   - 8.5 Operating the Master Document Repository
   - 8.6 Managing On-Site Document Submission Slots and Appointments
   - 8.7 Maintaining the Master Student Information Database
   - 8.8 Generating School-Wide DepEd Academic Reports (Masterlist, SF4, SF6, SF7, SF10, SNEd)
   - 8.9 Managing Class Sections and Advisers
   - 8.10 Managing the DepEd Elementary Subject Curriculum
   - 8.11 Managing Faculty and Teacher Profiles
   - 8.12 Building Class Schedules with Automated Conflict Detection
   - 8.13 Managing User Accounts and Role Promotions
   - 8.14 Publishing School Announcements and Facebook Sync
   - 8.15 Monitoring Security and System Audit Logs
   - 8.16 System Settings, School Year Management, and School CMS
9. [Chapter 9: Official DepEd School Forms Reference Guide](#chapter-9-official-deped-school-forms-reference-guide)
10. [Chapter 10: Troubleshooting, System Messages, and FAQ](#chapter-10-troubleshooting-system-messages-and-faq)
11. [Appendix: Glossary of Terms & Acronyms](#appendix-glossary-of-terms--acronyms)

---

# CHAPTER 1: INTRODUCTION AND SYSTEM OVERVIEW

### 1.1 Purpose of the User Manual
This User Manual provides complete, step-by-step operating instructions for the **Vinzons Pilot Elementary School – Student Information and Management System (VPES-SIMS)**. It is written for all user groups—prospective applicants, parents/guardians, enrolled learners, faculty advisers, subject teachers, school registrars, and system administrators. Furthermore, this document serves as an official technical and operational reference suitable for inclusion within the academic research manuscript.

### 1.2 System Identification and Institutional Profile
* **System Name:** Vinzons Pilot Elementary School – Student Information and Management System (VPES-SIMS)
* **School Name:** Vinzons Pilot Elementary School (VPES) / Special Science Elementary School (SSES)
* **DepEd School ID:** 112937
* **Division:** Camarines Norte
* **Region:** Region V (Bicol Region)
* **District:** Vinzons District
* **Curriculum Programs:** DepEd K-12 Enhanced Basic Education Curriculum / MATATAG Curriculum, Special Science Elementary School (SSES), and Special Needs Education (SNEd) / Inclusive Education.

### 1.3 System Objectives and Tangible Benefits
VPES-SIMS was designed to eliminate the logistical, clerical, and administrative challenges of traditional pen-and-paper school administration. Key benefits include:
1. **Convenient Remote Admissions:** Parents and guardians can submit the complete DepEd Basic Education Enrollment Form (BEEF) and upload digitized credentials 24/7 without waiting in crowded physical lines.
2. **Orderly Document Verification:** An automated appointment slot booking system prevents on-campus crowding by regulating physical document submission visits.
3. **DepEd-Compliant Academic Management:** Standardized quarterly grading (including composite MAPEH sub-grading) with real-time computation of general averages, passing marks, and honors eligibility.
4. **Automated School Forms Generation:** Direct compilation and export of official DepEd School Forms (SF1, SF2, SF3, SF4, SF5, SF6, SF7, SF8, SF9/Form 138, SF10/Form 137, and SNEd Registry) in standardized Excel and PDF formats.
5. **Data Protection & School Year Gating:** Strict role-based access control, encryption, session protection, and school year transition audits that preserve historical academic records while enforcing compliance with Republic Act No. 10173 (Data Privacy Act of 2012).

### 1.4 Scope and Limitations
* **Functional Scope:**
  - Online student registration, transferee admissions, balik-aral applications, and continuing student re-enrollment (Kindergarten to Grade 6).
  - Multi-tier document upload, preview, and administrative verification.
  - On-site appointment slot configuration and booking.
  - Section creation, student allocation, and gender-balanced auto-assignment.
  - Faculty management, teaching workload assignment, and timetable scheduling with real-time conflict checking.
  - Teacher grade encoding, MAPEH component averaging, and advisory class management.
  - Export of 10 official DepEd School Forms in PDF and Excel formats.
  - Multi-channel notification pipeline (Hostinger SMTP email queue, Semaphore SMS OTP alerts, and Facebook Graph API synchronization).
* **System Limitations:**
  - VPES is a public elementary school operating under DepEd free basic education; therefore, the system does not include financial billing or payment gateways.
  - The system operates at the school level (SIMS) and feeds verified data to school registrars for official encoding into the national DepEd Learner Information System (LIS).
  - Active internet access is required for real-time authentication, external API calls, and cloud document storage.

### 1.5 System Architecture, RBAC, and Security Framework
VPES-SIMS employs a multi-tiered architecture:
1. **Presentation Layer:** Responsive web interfaces built with HTML5, vanilla JavaScript ES6+, CSS3 modular variables, and interactive UI modals.
2. **Business Logic Layer:** Object-oriented PHP 8.x REST API endpoints residing in modular directories (`/api/*`).
3. **Data Layer:** MySQL / MariaDB database (`vpes_sims`) utilizing 31 normalized relational tables, strict foreign keys, and transaction integrity.
4. **Security & Authentication Framework:**
   - Dual-tier authentication via Google Firebase Identity Platform and local MySQL role verification.
   - 6-digit cryptographic One-Time Password (OTP) verification for account activations.
   - Dynamic Role-Based Access Control (RBAC) enforcing strict page and API authorization:
     - `admin` (System Administrator / School Registrar)
     - `teacher` (Faculty / Class Adviser / Subject Teacher)
     - `applicant` (Prospective Learner / Parent / Guardian)
     - `student` (Officially Enrolled / Linked Continuing Learner)
   - Immutable audit logging tracking user modifications, logins, approvals, and system configuration updates.

---

# CHAPTER 2: SYSTEM REQUIREMENTS AND GETTING STARTED

### 2.1 Hardware Requirements
* **Client Workstations / Desktop / Laptop:**
  - Processor: Dual-Core 1.8 GHz or faster (Intel Core i3 / AMD Ryzen 3 or higher recommended).
  - Memory (RAM): Minimum 4 GB (8 GB recommended for optimal multi-tab reporting).
  - Display Resolution: Minimum 1024 × 768 pixels (1920 × 1080 recommended for timetable builder and grading sheets).
* **Mobile & Tablet Devices:**
  - Modern iOS (iOS 14+) or Android (Android 9.0+) smartphone or tablet with responsive touchscreen support.

### 2.2 Software and Supported Web Browsers
* **Recommended Web Browsers:**
  - Google Chrome (Version 110 or higher) — *Recommended*
  - Mozilla Firefox (Version 110 or higher)
  - Microsoft Edge (Version 110 or higher)
  - Apple Safari (Version 15 or higher)
* **Required Browser Settings:**
  - JavaScript must be enabled.
  - Cookies and Local Storage / Session Storage must be allowed.
  - Pop-up blockers should be disabled for the VPES domain to permit report printing and appointment slip generation.
* **Document Viewer Software (For Exported Reports):**
  - Adobe Acrobat Reader (or built-in PDF viewer) for PDF reports.
  - Microsoft Excel 2016+, Microsoft 365, or LibreOffice Calc for `.xlsx` DepEd templates.

### 2.3 Network and Connectivity Standards
* **Broadband / Mobile Data:** Stable internet connection with a minimum download speed of 3 Mbps (5 Mbps or higher recommended for document uploads and PDF downloads).

### 2.4 Accessing the Web Portal
1. Open your web browser.
2. Enter the official portal URL in the address bar:
   ```text
   http://localhost/vpes-sims/
   ```
   *(Or the institutional production domain: `https://vpes.edu.ph/`)*
3. Press **Enter** on your keyboard to navigate to the Landing Page.

```text
[Insert Figure 1: System Landing Page Interface and Institutional Branding Here]
```

---

# CHAPTER 3: USER ACCOUNTS, AUTHENTICATION, AND SECURITY

### 3.1 User Roles and Access Permission Matrix

| Feature / Module | Public / Guest | Applicant / Parent | Enrolled Student | Teacher / Adviser | Administrator / Registrar |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Landing Page & Announcements** | Read-Only | Read-Only | Read-Only | Read-Only | Full Management |
| **Online BEEF Admission Form** | Blocked | Create / Edit | Read-Only | Blocked | Full Management |
| **Document Upload & Verification** | Blocked | Upload / Replace | Read-Only | Read-Only | Verify / Reject |
| **Physical Slot Booking** | Blocked | Book / Reschedule | Read-Only | Blocked | Full Management |
| **Student Timetable / Schedule** | Blocked | Blocked | View Assigned | View Assigned | Build / Conflict Check |
| **Quarterly Grades & MAPEH** | Blocked | Blocked | View Own Grades | Encode & Export | Full Audit Access |
| **School Forms Generation** | Blocked | Blocked | Blocked | SF1–SF9 Advisory | All SF1–SF10 & Masterlist |
| **Section & Subject Management** | Blocked | Blocked | Blocked | Blocked | Full Management |
| **User & Role Administration** | Blocked | Blocked | Blocked | Blocked | Full Management |
| **School Year Gating & Settings** | Blocked | Blocked | Blocked | Blocked | Full Management |
| **Audit Logs & System History** | Blocked | Blocked | Blocked | Blocked | Full Access |

---

### 3.2 Account Registration and 6-Digit OTP Verification
* **Purpose:** To create a secure account for applicants and parents to access the admission and student portal.
* **Access Path:** Navigate to `login.html` and click **"Create Account"** or select **"Sign Up"**.
* **Prerequisites:** Valid personal email address and active mobile number.

```text
[Insert Figure 4: New User Account Registration Interface Here]
```

#### Step-by-Step Procedure:
1. In the Sign-Up panel, enter your **Full Name** (e.g., *Maria Santos*).
2. Enter a valid **Email Address** (e.g., *mariasantos@gmail.com*).
3. Enter your **Mobile Phone Number** (11-digit Philippine mobile format: `09XXXXXXXXX`).
4. Enter your chosen **Password** (minimum 8 characters; must contain uppercase, lowercase, and numeric characters).
5. Confirm your password in the **Confirm Password** field.
6. Check the Google **reCAPTCHA** box ("I'm not a robot").
7. Click the **"Register Account"** button.
8. The system will dispatch a **6-Digit One-Time Password (OTP)** to your registered email/phone.
9. On the OTP verification screen, type the 6 digits into the sequential input boxes.
10. Click **"Verify Code"**.

```text
[Insert Figure 5: 6-Digit One-Time Password (OTP) Verification Interface Here]
```

* **Expected Result:** The system validates the OTP token, creates your user profile in the database with the default role `applicant`, and redirects you to the Student Type Selection screen.
* **Important Notes:** The OTP code expires after 10 minutes. If you do not receive the code within 60 seconds, click **"Resend verification code"**.

---

### 3.3 User Sign-In (Email/Password and Google OAuth)
* **Purpose:** To authenticate registered users and route them to their authorized role workspace.
* **Access Path:** Open `login.html`.
* **Prerequisites:** Active user account.

```text
[Insert Figure 3: System Authentication Interface (Login Form & Google Sign-In) Here]
```

#### Step-by-Step Procedure (Standard Sign-In):
1. In the Login form, enter your registered **Email Address**.
2. Enter your **Password**.
3. Click the **"Sign In"** button.
4. The system validates your credentials against Firebase and the local database.

#### Step-by-Step Procedure (Google OAuth Sign-In):
1. Click the **"Sign in with Google"** button (`btn-google`).
2. A secure Google Identity popup window will appear.
3. Select your authorized Google Account.
4. Grant standard profile and email permissions.

* **Expected Result:** The system retrieves your account role and routes your browser to the designated role portal.
* **Important Notes:** If an account is suspended by the school administrator, the system will prevent sign-in and display: *"Your account has been suspended. Please contact support."*

---

### 3.4 Role-Based Automatic Redirection
Upon successful authentication, the system evaluates the user's verified role and automatically redirects:
* **`admin`:** Redirects immediately to `adminDashboard.html`.
* **`teacher`:** Redirects immediately to `teacherDashboard.html`.
* **`applicant` / `student`:** Redirects to `studentDashboard.html` (or `index.html`).

---

### 3.5 Mandatory First-Login Password Change Procedure
* **Purpose:** To secure staff and faculty accounts created with administrative temporary passwords.
* **Access Path:** Triggered automatically upon initial login if `must_change_password = 1`.
* **Prerequisites:** Login using an administrator-issued temporary password.

#### Step-by-Step Procedure:
1. Upon logging in with your temporary password, a modal prompts: *"Temporary Password Detected. You must change your password before proceeding."*
2. Enter your temporary password in the **Current Password** field.
3. Enter your chosen personal password in the **New Password** field.
4. Retype the new password in the **Confirm New Password** field.
5. Click **"Update Password & Continue"**.

* **Expected Result:** The password hash is updated in both Firebase and MySQL, the `must_change_password` flag is reset to `0`, and you are granted full access to your portal.
* **Important Notes:** You cannot navigate away from this screen until a new password complying with security complexity is saved.

---

### 3.6 Password Recovery (Forgot Password via Email/SMS)
* **Purpose:** To regain access to an account when credentials are forgotten.
* **Access Path:** Click **"Forgot Password?"** on `login.html`.

#### Step-by-Step Procedure:
1. Click the **"Forgot Password?"** link on the login card.
2. In the recovery form, enter your registered **Email Address** or **Phone Number**.
3. Click **"Send Reset Link / Code"**.
4. Check your email inbox for an automated password reset link from VPES Portal.
5. Click the link to open the password reset interface, enter your new password twice, and click **"Save Password"**.

* **Expected Result:** Your password is reset, and you can immediately log in with your new credentials.

---

### 3.7 Session Management and Secure Sign-Out
* **Purpose:** To terminate authenticated sessions and prevent unauthorized access on shared devices.
* **Access Path:** Click the **User Avatar / Profile Menu** in the header or sidebar, and select **"Sign Out"** (or **"Log Out"**).

#### Step-by-Step Procedure:
1. Click the **"Sign Out"** button on the interface.
2. A confirmation modal will appear: *"Are you sure you want to log out?"*
3. Click **"Yes, Log Out"**.

* **Expected Result:** Session tokens and cached identity credentials in `sessionStorage` and `localStorage` are cleared, Firebase Auth sign-out is triggered, and your browser redirects to `login.html`.

---

# CHAPTER 4: PUBLIC AND GUEST USER PORTAL

### 4.1 Navigating the Landing Page Interface
* **Purpose:** To provide the community with school information, institutional announcements, and access to enrollment.
* **Access Path:** Access `index.html`.
* **Prerequisites:** None (publicly accessible).

#### Interface Elements:
* **Top Navigation Bar:** Contains the VPES Logo, School Name, navigation links (**Home**, **About**, **Admissions**, **Announcements**, **Contact**), and the **Login / Dashboard** button.
* **Hero Section:** Features the school motto, admission status banner, and primary call-to-action button (**"Enroll Now"** or **"View Admission"**).
* **Core Values Section:** Displays DepEd core values: *Maka-Diyos, Makatao, Makakalikasan, Makabansa*.
* **Institutional Details:** Presents the school history, SSES science program highlights, faculty statistics, and contact information.
* **Footer:** Displays address, official DepEd School ID (112937), email, links to the Privacy Policy and Terms and Conditions.

---

### 4.2 Checking Admission and Enrollment Gating Status
* **Purpose:** To inform parents whether the school is actively accepting new applications or re-enrollments.
* **Access Path:** Visible directly on the Hero section of `index.html`.

#### Status Indicators:
1. **Early Registration Open:** Indicates incoming Kindergarten and Grade 1 learners can submit pre-registration data.
2. **Regular Enrollment Open:** Full admission is active for all grade levels (Kindergarten to Grade 6).
3. **Re-Enrollment Active:** Continuing students can confirm their enrollment for the next academic year.
4. **Admissions Closed:** Displays an advisory informing parents that enrollment is closed and provides school office contact numbers.

---

### 4.3 Reading School Announcements and DepEd Bulletins
* **Purpose:** To view school news, academic schedules, and weather-related suspension advisories.
* **Access Path:** Scroll to the **Announcements** section of `index.html` or click **"Announcements"** in the top navigation bar.

```text
[Insert Figure 2: Public School Announcements Feed and Modal View Here]
```

#### Step-by-Step Procedure:
1. On the Landing Page, locate the **Announcements** feed.
2. Filter announcements by category if desired: **All**, **Academic**, **Admissions**, or **Emergency**.
3. Click on any announcement card to open the **Announcement Modal**.
4. Read the complete announcement text and view attached images or memos.
5. If the announcement originated from the official VPES Facebook Page, an official badge is displayed.
6. Click the **"X"** button or click outside the card to close the modal.

---

### 4.4 Data Privacy Policy and Terms of Use
* **Purpose:** To inform users how their personal identifiable information (PII) is collected, stored, and protected in compliance with the Data Privacy Act of 2012 (RA 10173).
* **Access Path:** Click **"Privacy Policy"** (`privacy-policy.html`) or **"Terms and Conditions"** (`terms-and-conditions.html`) in the footer.
* **Key Provisions:**
  - Compliance with DepEd Order No. 54, s. 2016 and RA 10173.
  - Strict utilization of student data solely for educational profiling, LIS recording, and academic grading.
  - Encryption of uploaded identity documents and strict administrative role access controls.


---

# CHAPTER 5: APPLICANT AND PARENT/GUARDIAN PORTAL (ADMISSIONS)

### 5.1 Student Type Selection (New Applicant vs. Existing Student)
* **Purpose:** To determine whether the logged-in user is applying as a new learner or linking an existing enrolled learner's permanent academic record.
* **Access Path:** Triggered automatically upon initial login of an account with the `applicant` role.
* **Prerequisites:** Authenticated applicant account.

```text
[Insert Figure 6: Student Type Selection Modal (New Applicant vs. Existing Student) Here]
```

#### Step-by-Step Procedure:
1. Upon logging in, the **"Welcome to VPES Portal!"** modal appears.
2. Review the two available applicant categories:
   - **New Student / Applicant:** Select this option if you are enrolling in Kindergarten for the first time, transferring from another school, or returning to school (*Balik-Aral*).
   - **Existing Student:** Select this option if the student has already been enrolled in VPES during a prior school year and possesses an existing DepEd 12-digit Learner Reference Number (LRN).
3. Click the card corresponding to your status.

* **Expected Result:**
  - Selecting **"New Student / Applicant"** redirects to the Online Admission Application Form (`applicationform.html`).
  - Selecting **"Existing Student"** opens the LRN Verification & Account Linking Dialog (`lrnVerificationModal.js`).

---

### 5.2 Linking an Existing Student Record via 12-Digit LRN
* **Purpose:** To associate an existing enrolled student's permanent records, grades, and schedule with a newly created parent or student user account.
* **Access Path:** Click **"Existing Student"** on the Student Type Modal or click **"Link Existing Student Record"** on the applicant dashboard.
* **Prerequisites:** Official 12-digit DepEd LRN and registered student Birthdate.

```text
[Insert Figure 7: LRN Verification and Account Linking Modal Here]
```

#### Step-by-Step Procedure:
1. In the **Link Your Student Record** dialog, enter the student's **12-Digit Learner Reference Number (LRN)** in the input field.
2. Select the student's exact **Birthdate** (Month, Day, Year) matching their official DepEd registration records.
3. Click **"Verify LRN"**.
4. The system validates the credentials against the master student database:
   - If a match is verified, the system displays the student's **Full Name**, **Grade Level**, and **Last Enrolled Section** for identity confirmation.
   - A confirmation prompt appears: *"Is this your student record?"*
5. Click **"Confirm & Link Account"**.

* **Expected Result:** The user's account role is upgraded to `student`. The dashboard reconfigures to display active academic grades, weekly timetables, and continuing re-enrollment features.
* **Important Notes:** An LRN can only be linked to authorized parent/student accounts. If your LRN is rejected or flagged as already linked, contact the VPES Registrar with a copy of the student's PSA Birth Certificate.

---

### 5.3 Step-by-Step Online Admission Application (DepEd BEEF Compliance)
* **Purpose:** To complete the official Department of Education Basic Education Enrollment Form (BEEF) online.
* **Access Path:** Select **"New Student / Applicant"** or click **"New Admission Application"** on `studentDashboard.html`.
* **Prerequisites:** Completed student demographic data, parent/guardian information, and residential address details.

---

#### 5.3.1 Step 1: School Information and Grade Level Selection
* **Target Interface:** Form Card 1 (`applicationform.html`)

```text
[Insert Figure 8: Online Admission Form – Step 1: School Information & Grade Level Here]
```

1. **School Year:** Automatically loaded and displayed as read-only based on the active school year configured by the administrator (e.g., *2026–2027*).
2. **Grade Level to Enroll:** Click the dropdown menu and select the target grade level:
   - *Kindergarten*
   - *Grade 1*
   - *Grade 2*
   - *Grade 3*
   - *Grade 4*
   - *Grade 5*
   - *Grade 6*
3. **Learner Status / Type:** Select whether the applicant is:
   - *No LRN (Incoming Kindergarten / New Enrollee)*
   - *With LRN (Continuing / Grade 1 to 6)*
   - *Transferee (Transferring in from another school)*
   - *Balik-Aral / Returning Learner (Resuming schooling after a dropout period)*

---

#### 5.3.2 Step 2: Learner Demographic and LIS Information
* **Target Interface:** Form Card 2 (`applicationform.html`)

```text
[Insert Figure 9: Online Admission Form – Step 2: Student Demographic & BEEF Information Here]
```

1. **Learner Reference Number (LRN):** Enter the 12-digit number (required for Grades 1–6; optional for Kindergarten).
2. **PSA Birth Certificate Number:** Enter the official Certificate of Live Birth registry number issued by the Philippine Statistics Authority (PSA) / NSO.
3. **Learner Legal Name:**
   - **Last Name:** Enter the student's legal surname.
   - **First Name:** Enter the student's legal given name.
   - **Middle Name:** Enter the middle name (leave blank or check "No Middle Name" if not applicable).
   - **Extension Name:** Select name extension from the dropdown if applicable (*Jr., Sr., II, III, IV*).
4. **Date of Birth:** Select date from the date picker.
5. **Age:** Automatically calculated and displayed by the system based on the birthdate.
6. **Sex:** Select **Male** or **Female**.
7. **Mother Tongue:** Select or enter the learner's native first language (e.g., *Tagalog*, *Bikol*, *English*).
8. **Belonging to Indigenous Peoples (IP) Community?:** Select **Yes** or **No**. If Yes, specify the specific IP/ICC community.
9. **4Ps Beneficiary?:** Select **Yes** or **No**. If Yes, enter the official 4Ps Household ID Number.

---

#### 5.3.3 Step 3: Geographic Residential Address (PSGC Lookup)
* **Target Interface:** Form Card 3 (`applicationform.html`)

```text
[Insert Figure 10: Online Admission Form – Step 3: PSGC Geographic Residential Address Here]
```

The system incorporates the Philippine Standard Geographic Code (PSGC) database for cascading address selection:
1. **Region:** Select the administrative region (Default: *Region V - Bicol*).
2. **Province:** Select the province (Default: *Camarines Norte*).
3. **Municipality / City:** Select the municipality (Default: *Vinzons*).
4. **Barangay:** Click the dropdown to select the specific barangay (e.g., *Barangay I (Poblacion)*, *Barangay II*, *Calangcawan Norte*, *Mangcayo*, etc.).
5. **House No. / Street / Sitio / Purok:** Type the exact house number, street address, or purok identifier.
6. **Zip Code:** Automatically filled based on municipality selection (*4603* for Vinzons).

---

#### 5.3.4 Step 4: Parent and Legal Guardian Profiling
* **Target Interface:** Form Card 4 (`applicationform.html`)

```text
[Insert Figure 11: Online Admission Form – Step 4: Parent & Guardian Details Here]
```

> [!IMPORTANT]
> DepEd regulations require full contact details for at least one parent or legal guardian.

1. **Father's Profile:**
   - Last Name, First Name, Middle Name
   - Contact Telephone / Mobile Number
   - Highest Educational Attainment
   - Employment / Occupation
2. **Mother's Maiden Profile:**
   - Maiden Last Name (surname before marriage), First Name, Middle Name
   - Contact Telephone / Mobile Number
   - Highest Educational Attainment
   - Employment / Occupation
3. **Legal Guardian Profile:** (Required if the learner does not live with parents)
   - Full Name, Relationship to Learner (*Grandparent, Aunt/Uncle, Sibling, Foster Guardian*)
   - Contact Mobile Number
4. **Emergency Contact Person:** Provide the primary contact person's full name, relationship, and active phone number for emergency notifications.

---

#### 5.3.5 Step 5: Special Needs Education (SNEd) and PWD Information
* **Target Interface:** Form Card 5 (`applicationform.html`)

```text
[Insert Figure 12: Online Admission Form – Step 5: Special Needs Education (SNEd) & Modality Here]
```

1. **Under SNEd / Special Education Program?:** Select **Yes** or **No**.
2. If **Yes**:
   - **Has PWD ID?:** Select **Yes** or **No**. If Yes, enter the official PWD ID number.
   - **Medical Diagnosis:** Check applicable diagnosed conditions (*Visual Impairment, Hearing Impairment, Learning Disability, Intellectual Disability, Autism Spectrum Disorder, Emotional-Behavioral Disorder, Orthopedic/Physical Handicap, Speech/Language Disorder, Health Impairment*).
   - **Manifestations & Assistive Requirements:** Specify if the learner requires specialized assistive technologies, braille, sign language, or accessibility ramps.

---

#### 5.3.6 Step 6: Returning Learner (Balik-Aral) and Transferee History
* **Target Interface:** Form Card 6 (`applicationform.html`)
*(This section is displayed conditionally for Transferees and Balik-Aral applicants)*
1. **Last Grade Level Completed:** Select the previous grade finished.
2. **Last School Year Completed:** Enter the previous academic year (e.g., *2025–2026*).
3. **Last School Attended:** Enter the full official name of the previous elementary school.
4. **Previous School ID:** Enter the 6-digit DepEd School ID of the previous institution.

---

#### 5.3.7 Step 7: Learning Modality Preferences
* **Target Interface:** Form Card 7 (`applicationform.html`)
1. Select the family's preferred learning modality:
   - *Face-to-Face (In-Person Classroom Instruction)* — Standard
   - *Blended Learning (Combined in-person and digital learning)*
   - *Modular (Printed Self-Learning Modules)*
   - *Modular (Digital / Offline Tablet Modules)*
2. After completing all form cards, click the **"Proceed to Documents"** button (`btn-primary`).

---

### 5.4 Uploading Required Admission Documents
* **Purpose:** To submit digitized copies of required academic and identification credentials.
* **Access Path:** Step 2 of the admission sequence (`uploadDocument.html`).
* **Prerequisites:** Scanned documents or clear camera photos in PDF, JPG, or PNG format (Maximum file size: 5 MB per document).

```text
[Insert Figure 13: Document Upload Interface with Grade-Specific Requirement Slots Here]
```

#### Required Document Slots by Grade Level:
* **All Applicants (Kindergarten to Grade 6):**
  - **PSA Birth Certificate:** Clear, readable copy of the PSA/NSO Certificate of Live Birth.
* **Grade 1 Applicants:**
  - **Kindergarten Certificate of Completion (ECCDC Checklist):** Proof of kindergarten completion.
* **Transferees and Returning Learners (Grades 1 to 6):**
  - **School Form 9 (SF9 / Form 138):** Official Learner Progress Report Card from the previous school year indicating promotional status.
  - **School Form 10 (SF10 / Form 137):** Permanent Academic Record (or request letter / temporary record).
  - **Certificate of Good Moral Character:** Issued by previous school head.

#### Step-by-Step Procedure:
1. For each document slot, click the **"Choose File"** (or **"Browse"**) button.
2. Select the digitized file from your computer or mobile storage.
3. Once selected, the system displays the file name, size, and a preview thumbnail.
4. Click the **"View"** button (`ri-eye-line`) to inspect the document and confirm legibility.
5. If the wrong file was selected, click the **"Remove"** button (`ri-delete-bin-line`) and re-select.
6. Once all mandatory document slots display an uploaded status, click **"Proceed to Review"**.

---

### 5.5 Reviewing, Certifying Data Privacy, and Submitting the Application
* **Purpose:** To verify all submitted information, agree to statutory privacy declarations, and finalize submission.
* **Access Path:** Step 3 of the admission sequence (`review.html`).

```text
[Insert Figure 14: Application Review, Data Privacy Agreement, and Submission Here]
```

#### Step-by-Step Procedure:
1. Carefully inspect the summary cards for **School Information**, **Student Demographics**, **Residential Address**, **Parent/Guardian Contacts**, **SNEd Details**, and **Uploaded Documents**.
2. If any field requires correction, click the **"Edit"** button on that specific card to return to the appropriate form section.
3. Scroll down to the **Declaration & Legal Consent** card.
4. Read the official DepEd and RA 10173 statutory statement:
   > *"I hereby certify that the above information given are true and correct to the best of my knowledge and I allow the Department of Education to use my child's details to create and/or update his/her learner profile in the Learner Information System. The information herein shall be treated as confidential in compliance with the Data Privacy Act of 2012."*
5. Check the mandatory declaration checkbox: **"I have reviewed all information and agree to the terms and conditions."**
6. The **"Submit Application"** button will activate. Click **"Submit Application"**.

---

### 5.6 Understanding the Application Reference Tracking Code
* **Target Interface:** Submission Confirmation Dialog (`review.html`)

```text
[Insert Figure 15: Application Submission Success Dialog and Tracking Number Generation Here]
```

Upon submission, the system performs the following actions:
1. Generates a unique, standardized Application Reference Number in the format:
   ```text
   VPES-YYYY-XXXXX
   ```
   *(Example: `VPES-2026-00142`)*
2. Creates an immutable application log entry timestamping the submission.
3. Queues an automated confirmation email to the applicant's registered address.
4. Click the **"Copy"** button to copy the reference tracking code to your clipboard.
5. Click **"Go to Dashboard"** to transition to your live applicant tracking portal.

---

### 5.7 Navigating the Applicant Dashboard and 5-Stage Timeline
* **Purpose:** To monitor admission progress and interact with admissions personnel.
* **Access Path:** Open `studentDashboard.html` (Applicant Mode).

```text
[Insert Figure 16: Applicant Dashboard with 5-Stage Admission Progress Tracker Here]
```

#### The 5-Stage Admissions Progress Timeline:
1. **Stage 1: Application Submitted:** Application successfully received by the VPES admissions server.
2. **Stage 2: Document Review:** Admissions staff are reviewing digital uploads for clarity, completeness, and validity.
3. **Stage 3: Evaluation & Verification:** Registrar verifies demographic data and checks for duplicate LRN records.
4. **Stage 4: Admission Approval:** The application is officially approved. **This milestone unlocks the appointment slot booking feature.**
5. **Stage 5: On-Site Submission Schedule:** The applicant visits the campus on their booked date with original documents. Once verified, the student is transitioned to **Officially Enrolled**.

#### Dashboard Navigation Tabs:
* **Home / Overview (`dashboardSection`):** Real-time timeline, status banner, and actionable guidance alerts.
* **Application Details (`applicationSection`):** Full read/edit view of submitted BEEF information.
* **Document Requirements (`documentsSection`):** Status per document slot (*Pending*, *Verified*, or *Needs Re-upload*).
* **Book Schedule (`bookApptSection`):** Physical appointment booking calendar (enabled upon Stage 4 approval).
* **Status Tracker (`statusSection`):** Chronological log of administrative actions and notes.

---

### 5.8 Booking an On-Site Physical Document Submission Appointment Slot
* **Purpose:** To select an official date and time window to present original physical documents at the VPES Registrar's Office.
* **Access Path:** Click **"Book Schedule"** on the applicant dashboard guidance card or click the **"Book Appointment"** sidebar tab.
* **Prerequisites:** Application must be approved by the administrator (**Stage 4: Admission Approval**).

```text
[Insert Figure 17: On-Site Document Submission Appointment Slot Booking Interface Here]
```

#### Step-by-Step Procedure:
1. Navigate to the **Book Appointment** section.
2. An interactive monthly calendar will appear displaying available verification dates.
   - **Green Dates:** Dates with available open slots.
   - **Red / Gray Dates:** Dates that are fully booked, weekends, or non-working holidays.
3. Click on your desired available appointment date.
4. In the side panel, choose your preferred **Time Window**:
   - **Morning Session (AM):** 8:00 AM – 11:30 AM
   - **Afternoon Session (PM):** 1:00 PM – 4:30 PM
5. The interface indicates remaining capacity for each session.
6. Click **"Confirm Appointment Booking"**.

* **Expected Result:** The appointment slot is reserved in the database (`slot_bookings` table), decreasing available capacity. The system generates an official Appointment Slip.

---

### 5.9 Downloading and Printing the Official Appointment Slip
* **Purpose:** To provide physical proof of scheduled on-site document verification.
* **Access Path:** Click **"Download Appointment Slip"** or **"Print Slip"** on the appointment confirmation dialog.

#### Step-by-Step Procedure:
1. Click the **"Print / Download Slip"** button.
2. A print-ready document preview opens containing:
   - Official School Header and DepEd Seal
   - Student Full Name and Application Reference Number (`VPES-YYYY-XXXXX`)
   - Grade Level Applied For
   - Confirmed Appointment Date and Time Window (AM/PM)
   - Checklist of Original Documents Required for Verification
   - Unique Verification QR Code
3. Click **"Print"** to send to your local printer, or select **"Save as PDF"** to store on your device.
4. Bring this slip along with your original documents on your scheduled visit date.

---

### 5.10 Responding to Document Correction and Re-upload Requests
* **Purpose:** To replace a rejected document (e.g., due to blurriness or incorrect document type) without restarting the application.
* **Access Path:** Navigate to the **Document Requirements** section on `studentDashboard.html`.
* **Prerequisites:** Document rejected by registrar with specific feedback.

#### Step-by-Step Procedure:
1. When a document is rejected, the applicant receives an automated email/SMS alert detailing the rejection reason (e.g., *"PSA Birth Certificate is blurred and registry number is illegible"*).
2. Log in to the applicant dashboard and click **"Documents"**.
3. The rejected document slot displays a red status badge: **"Needs Re-upload"** along with the reviewer's feedback note.
4. Click **"Upload Replacement File"**.
5. Select a clear, properly scanned document.
6. Click **"Submit Updated Document"**.

* **Expected Result:** The document status resets to **"Pending Verification"**, and an alert is delivered to the administrator to re-evaluate the file.


---

# CHAPTER 6: ENROLLED STUDENT PORTAL

### 6.1 Navigating the Enrolled Student Dashboard
* **Purpose:** To provide officially enrolled learners and their parents with a centralized view of active academic enrollment, section details, and school updates.
* **Access Path:** Automatically displayed upon logging into an account linked to an officially enrolled learner (`studentDashboard.html` - Enrolled Mode).
* **Prerequisites:** Student must be transitioned to `ENROLLED` status by the school registrar.

```text
[Insert Figure 18: Enrolled Student Dashboard Overview and Section Details Here]
```

#### Interface Elements:
* **Student Academic Card:** Displays the learner's official **Full Name**, permanent **12-Digit LRN**, **Grade Level**, enrolled **Section Name** (with its official color badge), **Classroom / Room Number**, and **Class Adviser Name**.
* **Academic School Year Badge:** Confirms the currently active DepEd school year (e.g., *S.Y. 2026–2027*).
* **Sidebar Navigation:**
  - **Home (`enrolledHomeSection`):** Enrolled status, adviser details, quick announcements.
  - **Class Schedule (`scheduleSection`):** Full weekly subject timetable.
  - **My Grades (`gradesSection`):** Current quarterly academic grades and historical archives.
  - **Documents (`documentsSection`):** Archive of verified submitted credentials.
  - **Profile (`profileSection`):** Learner demographic, parent, and emergency contact records.
  - **Re-Enrollment (`reEnrollmentSection`):** Visible when the re-enrollment window is activated by the school administration.

---

### 6.2 Viewing the Weekly Interactive Class Schedule
* **Purpose:** To inspect daily class hours, subjects, assigned teachers, and room numbers.
* **Access Path:** Click **"Class Schedule"** on the student dashboard sidebar.

```text
[Insert Figure 19: Enrolled Student Weekly Interactive Class Schedule Here]
```

#### Step-by-Step Procedure:
1. In the student sidebar, click the **"Class Schedule"** tab (`scheduleSection`).
2. The interactive weekly timetable renders Monday through Friday in chronological time blocks.
3. Each schedule card displays:
   - **Time Range:** Start time and end time (e.g., *07:30 AM – 08:20 AM*).
   - **Subject Title:** DepEd subject name (e.g., *Mathematics*, *English*, *Araling Panlipunan*).
   - **Assigned Teacher:** Full name and title of the subject teacher (e.g., *Mr. Jonathan Dela Cruz*).
   - **Room / Location:** Classroom assignment (e.g., *Room 102 - Mabini Hall*).
   - **Subject Color Code:** Color-coded border matching official curriculum settings.
4. Click on any class block to view a detailed popup modal of the session.
5. Click **"Print Schedule"** to print or save a clean copy of your weekly timetable.

---

### 6.3 Accessing Quarterly Academic Grades and Performance
* **Purpose:** To monitor quarterly learning progress, subject grades, general average, and promotional standing.
* **Access Path:** Click **"My Grades"** on the student dashboard sidebar.

```text
[Insert Figure 20: Enrolled Student Quarterly Grades Display and MAPEH Breakdown Here]
```

---

#### 6.3.1 Interpreting DepEd Quarterly Grades and Passing Status
The grading system adheres strictly to DepEd Order No. 8, s. 2015 (Policy Guidelines on Classroom Assessment for the K to 12 Basic Education Program):
* **Quarterly Columns:** Displays numerical grades for **1st Quarter (Q1)**, **2nd Quarter (Q2)**, **3rd Quarter (Q3)**, and **4th Quarter (Q4)**.
* **Final Rating:** The unweighted arithmetic average of the four quarters, computed automatically:
  $$\text{Final Rating} = \frac{Q_1 + Q_2 + Q_3 + Q_4}{4}$$
* **Passing Standard:**
  - Grades $\ge 75$: Marked with a green badge: **"Passed"**.
  - Grades $< 75$: Marked with a red badge: **"Failed"**.
* **General Average:** Displayed in the summary card at the bottom of the table along with the learner's overall promotional standing (*Promoted to Next Grade Level* or *Retained*).

---

#### 6.3.2 Viewing Detailed MAPEH Component Sub-Grades
In accordance with DepEd elementary curriculum standards, the **MAPEH** subject (Music, Arts, Physical Education, and Health) displays an expandable drawer or sub-table:
1. In the grades table, locate the **MAPEH** subject row.
2. Click the **"View Components"** button (`ri-arrow-down-s-line`) next to the MAPEH composite grade.
3. The table expands to reveal the two integrated component marks:
   - **Music & Arts:** Quarterly grade
   - **Physical Education & Health (PE & Health):** Quarterly grade
4. The system confirms that the overall MAPEH quarterly grade is the exact mathematical average of the components:
   $$\text{MAPEH Composite} = \frac{\text{Music \& Arts} + \text{PE \& Health}}{2}$$

---

#### 6.3.3 Browsing Historical School Year Grade Archives
* **Step-by-Step Procedure:**
  1. At the top of the **My Grades** section, locate the **School Year Selector** dropdown.
  2. Select any previous completed academic year (e.g., *S.Y. 2025–2026*).
  3. The table instantly reloads to display the archived grades, section adviser, and final promotional status for that historical term.
  4. Select **"Current S.Y. (2026–2027)"** to return to active school year evaluations.

---

### 6.4 Viewing and Verifying Student Profile Information
* **Purpose:** To verify that the learner's official DepEd master records are complete and accurate.
* **Access Path:** Click **"Profile"** on the student dashboard sidebar.

#### Elements Displayed:
* **Learner Identification:** Full Legal Name, LRN, PSA Birth Certificate Number, Birthdate, Gender, Age.
* **Residential Address:** Standardized PSGC address, Barangay, Municipality, Province, Zip.
* **Family & Guardian Information:** Father's name and contact, Mother's maiden name and contact, Guardian details.
* **Social Protection Indicators:** 4Ps Household ID, Indigenous Peoples (IP) affiliation, SNEd / PWD categorization.
* **Reporting Discrepancies:** If any information contains a typographical error, click **"Request Information Correction"** to submit a correction notice to the school registrar.

---

### 6.5 Submitting Continuing Student Re-Enrollment
* **Purpose:** To confirm enrollment for the upcoming school year without re-submitting the full application form.
* **Access Path:** Click **"Re-Enrollment"** (`reEnrollmentSection`) on the student dashboard sidebar.
* **Prerequisites:** Administrator must open the Re-Enrollment period in System Settings.

#### Step-by-Step Procedure:
1. When the re-enrollment period opens, an advisory alert appears on the student dashboard: *"Re-Enrollment for S.Y. 2027–2028 is now Open."*
2. Click **"Confirm Re-Enrollment Now"** or click the **Re-Enrollment** sidebar tab.
3. Verify the target promotional grade level displayed (e.g., *Advancing to Grade 5*).
4. Review your emergency contact number and residential address:
   - If unchanged, leave as is.
   - If changed, type your updated contact details in the fields provided.
5. Click **"Submit Re-Enrollment Intent"**.
6. A confirmation modal appears: *"Your re-enrollment request has been submitted to the registrar for placement."*

* **Expected Result:** The submission is recorded in `re_enrollment_confirmations` and appears in the administrator's re-enrollment queue for section assignment.

---

### 6.6 Alumni / Graduated Student Interface
* **Purpose:** To provide Grade 6 graduates with lifelong access to their elementary scholastic achievements.
* **Access Path:** Automatically configured when a student account holds the `GRADUATED` lifecycle status.
* **Features:**
  - Displays a commemorative graduation banner celebrating completion of elementary education at VPES.
  - Permanent access to complete academic transcripts, honors, and year-by-year grade archives across all six elementary grades.
  - Provides official request links for school-to-school transfer of the Learner Permanent Academic Record (DepEd SF10-ES) to the recipient Junior High School.

---

# CHAPTER 7: TEACHER AND CLASS ADVISER PORTAL

### 7.1 Navigating the Teacher Dashboard
* **Purpose:** To give teachers an operational overview of their advisory section, teaching loads, and daily schedule.
* **Access Path:** Log in using a teacher account (`teacherDashboard.html`).
* **Prerequisites:** Active user account with the `teacher` role.

```text
[Insert Figure 21: Teacher Dashboard Overview and Assigned Advisory Class Summary Here]
```

#### Interface Elements:
* **Welcome Header:** Displays the teacher's official name, employee ID, active school year, and current quarter.
* **Advisory Class Summary Card:**
  - Assigned Section Name (e.g., *Grade 4 - Mabini*)
  - Grade Level and Assigned Room Number
  - Total Enrolled Learners (with Male vs. Female demographic breakdown)
* **Teaching Load Metrics:** Displays the total number of subject classes handled and total weekly teaching minutes.
* **Today's Teaching Schedule:** Chronological widget showing today's upcoming classes with countdown indicators.
* **Sidebar Navigation:**
  - **Dashboard (`teacherDashboard.html`):** Overview and announcements.
  - **My Students (`teacherStudents.html`):** Advisory class learner roster.
  - **Grading Sheet (`teacherGrades.html`):** Quarterly grade encoding grid.
  - **School Forms (`teacherSchoolForms.html`):** DepEd SF1 to SF9 generator.
  - **Schedule (`teacherSchedule.html`):** Personal weekly timetable.
  - **Settings (`teacherSettings.html`):** Teacher profile and security.

---

### 7.2 Managing Advisory Class Student Rosters
* **Purpose:** To view, search, and manage learner records within the assigned advisory section.
* **Access Path:** Click **"My Students"** on the teacher sidebar (`teacherStudents.html`).

```text
[Insert Figure 22: Teacher Advisory Student Roster Directory Here]
```

#### Step-by-Step Procedure:
1. Navigate to `teacherStudents.html`.
2. The page automatically loads all officially enrolled learners in your advisory section.
3. Use the search bar to locate students by **LRN** or **Last Name**.
4. Filter by **Gender** (**Male** / **Female**) or **Enrollment Status**.
5. The roster displays:
   - Student Full Legal Name
   - 12-Digit LRN
   - Age and Birthdate
   - 4Ps Beneficiary Status
   - Parent / Guardian Full Name and Emergency Mobile Number
6. Click **"View Full Profile"** on any student row to inspect the learner's complete BEEF demographic profile and emergency contacts.
7. Click **"Export Roster (Excel)"** or **"Print Roster"** to generate a quick physical reference list.

---

### 7.3 Operating the Teacher Quarterly Grading Sheet
* **Purpose:** To encode, compute, validate, and submit quarterly academic grades in compliance with DepEd assessment standards.
* **Access Path:** Click **"Grading Sheet"** on the teacher sidebar (`teacherGrades.html`).
* **Prerequisites:** Assigned subject or advisory class for the active academic year.

```text
[Insert Figure 23: Teacher Quarterly Grading Sheet Grid Here]
```

---

#### 7.3.1 Selecting Section, Subject, and Grading Quarter
1. At the top of `teacherGrades.html`, use the three selectors:
   - **Select Section:** Choose from your assigned sections (e.g., *Grade 4 - Mabini*).
   - **Select Subject:** Choose the subject you teach for that section (e.g., *Mathematics*, *Science*, *MAPEH*).
   - **Select Quarter:** Choose the grading period:
     - *1st Quarter*
     - *2nd Quarter*
     - *3rd Quarter*
     - *4th Quarter*
2. The system dynamically loads the official student roster for that section into the spreadsheet grid.

---

#### 7.3.2 Encoding Quarterly Numerical Grades (0–100 Scale)
1. In the grading grid, locate the input cell under the active quarter for a student.
2. Type the learner's quarterly numerical grade (e.g., *88*).
3. **Automated Input Validation:**
   - The cell accepts numerical values between `0` and `100`.
   - Entering values outside `0–100` triggers an immediate error outline preventing saving.
   - Grades $\ge 75$ are styled with positive green text; grades $< 75$ are highlighted in amber/red.
4. Press the **Down Arrow** or **Enter** key on your keyboard to navigate to the next student row quickly.

---

#### 7.3.3 Using the MAPEH Component Breakdown Modal
When grading **MAPEH**, individual sub-component marks must be recorded to determine the composite quarterly grade.

```text
[Insert Figure 24: Teacher MAPEH Component Breakdown and Sub-Grading Modal Here]
```

1. Select **MAPEH** in the Subject dropdown.
2. In the grading table, the quarter cells for MAPEH display a special **Calculator Icon** (`ri-calculator-line`).
3. Click on the input cell or click the **"Breakdown"** button on any student row.
4. The **MAPEH Component Breakdown Modal** opens, displaying:
   - Student Full Name and LRN
   - Active Grading Quarter
5. Enter the numerical grade for:
   - **Music & Arts:** (e.g., `86.00`)
   - **Physical Education & Health (PE & Health):** (e.g., `90.00`)
6. As you type, the modal's calculation engine computes the composite in real time:
   $$\text{Computed Composite} = \frac{86.00 + 90.00}{2} = 88.00$$
7. The modal displays the computed rating and passing remarks (*Passed*).
8. Click **"Apply & Update MAPEH"**.
9. The calculated composite (`88.00`) is automatically inserted into the master grading table and recorded in the `mapeh_subgrades` database table.

---

#### 7.3.4 Reviewing General Averages, Automatic Remarks, and Saving Grades
1. As quarterly grades are entered, the system updates the **Final Rating** and **Remarks** columns in real time:
   - Grades $\ge 75$: Remarks = **PASSED**
   - Grades $< 75$: Remarks = **FAILED**
2. After completing grade entry for the class, click the **"Save All Changes"** button (`btn-primary`).
3. A confirmation modal verifies: *"Are you sure you want to save all grade changes to the database?"*
4. Click **"Confirm & Save"**.
5. The system saves the records to the `grades` table and logs the modification in the audit trail. A green toast notification confirms: *"Grades successfully updated!"*

---

#### 7.3.5 Exporting the Official Class Record Summary
1. Click the **"Export Grades"** button on the grading toolbar.
2. Choose your preferred output:
   - **Download Class Record (Excel):** Generates the official DepEd electronic class record (`.xlsx`).
   - **Print Summary of Grades (PDF):** Generates a print-ready PDF class list complete with quarterly grades, final ratings, and teacher signature lines.

---

### 7.4 Viewing and Printing the Individual Teaching Schedule
* **Purpose:** To view personal weekly teaching hours and print an individual teaching timetable.
* **Access Path:** Click **"Schedule"** on the teacher sidebar (`teacherSchedule.html`).

```text
[Insert Figure 25: Teacher Individual Weekly Timetable View and Print Preview Here]
```

#### Step-by-Step Procedure:
1. Open `teacherSchedule.html`.
2. The timetable displays your weekly schedule grid from Monday to Friday.
3. Inspect each block for:
   - Time duration
   - Subject taught
   - Section name
   - Assigned classroom / room number
4. The summary bar at the top displays your **Total Teaching Load** (e.g., *30 hours / week*).
5. Click the **"Print Timetable"** button. A formatted, high-resolution schedule opens in a print preview window ready for physical posting in your classroom.

---

### 7.5 Generating DepEd School Forms in the Teacher Hub
* **Purpose:** To automatically compile and generate official Department of Education School Forms for the teacher's advisory class.
* **Access Path:** Click **"School Forms"** on the teacher sidebar (`teacherSchoolForms.html`).
* **Prerequisites:** Must be assigned as the official Class Adviser of a section.

```text
[Insert Figure 26: Teacher DepEd School Forms Hub (SF1 to SF8 Generation Cards) Here]
```

---

#### 7.5.1 Generating SF1: School Register (Excel and PDF)
* **Description:** Official masterlist of learners containing comprehensive demographic, family, and socio-economic data.
* **Step-by-Step Procedure:**
  1. In the School Forms catalog, locate the **SF 1: School Register** card.
  2. Click **"View & Generate SF1"**.
  3. Select your output format: **Official Excel Template (.xlsx)** or **Print-Ready PDF**.
  4. Click **"Download / Generate"**.
  5. The system reads student records from `students`, `student_addresses`, and `student_guardians`, populates the official DepEd SF1 template, and delivers the file to your browser downloads.

---

#### 7.5.2 Generating SF2: Daily Attendance Report (Monthly Selector)
* **Description:** Monthly attendance summary recording daily learner presence, absences, tardiness, and dropouts.
* **Step-by-Step Procedure:**
  1. Locate the **SF 2: Daily Attendance Report** card.
  2. Click **"Generate SF2"**.
  3. In the modal dialog, select the **Target Month and Year** (e.g., *October 2026*).
  4. Select **Format Scope** (Excel or PDF).
  5. Click **"Generate SF2"**. The system compiles attendance data and exports the official report.

---

#### 7.5.3 Generating SF3: Books Issued and Returned
* **Description:** Official textbook inventory tracking textbooks assigned to and retrieved from each learner.
* **Step-by-Step Procedure:**
  1. Locate the **SF 3: Books Issued & Returned** card.
  2. Click **"Generate SF3"**.
  3. Review the textbook title checklist.
  4. Click **"Download Excel"** to generate the inventory tracking sheet.

---

#### 7.5.4 Generating SF5: Report on Promotion and Level of Proficiency
* **Description:** End-of-school-year report listing all promoted, retained, and conditionally promoted learners with final general averages.
* **Step-by-Step Procedure:**
  1. Locate the **SF 5: Report on Promotion** card.
  2. Click **"Generate SF5"**.
  3. The system checks that all four quarters of grades have been encoded.
  4. Select **Excel** or **PDF**.
  5. Click **"Download SF5"**. The file contains complete general averages, proficiency distribution statistics, and promotional summaries.

---

#### 7.5.5 Generating SF8: Learner Basic Health and Nutrition Report
* **Description:** Annual health assessment recording learner height, weight, Body Mass Index (BMI), and nutritional status.
* **Step-by-Step Procedure:**
  1. Locate the **SF 8: Health & Nutrition Report** card.
  2. Click **"Generate SF8"**.
  3. Select **Download Official Excel Template**.

---

#### 7.5.6 Generating SF9 / Form 138: Progress Report Card (Individual & Batch ZIP)
* **Description:** The official elementary learner report card issued to parents showing quarterly academic ratings, core values ratings, and attendance.

```text
[Insert Figure 27: Teacher SF9 (Progress Report Card) Generator & Batch ZIP Download Interface Here]
```

* **Procedure for Individual Student SF9:**
  1. Locate the **SF 9: Progress Report Card (Form 138)** card and click **"Open SF9 Workspace"**.
  2. The table lists all enrolled learners in your advisory section.
  3. Use the search input to filter by student name or LRN.
  4. On any student row, choose from the three action buttons:
     - **Excel:** Downloads that single learner's official SF9 card as an `.xlsx` workbook.
     - **PDF:** Opens a high-resolution, print-ready PDF of the front and back of the report card.
     - **Print / Preview:** Opens the direct browser print dialog.

* **Procedure for Batch Export of ALL Student SF9 Cards (.ZIP):**
  1. In the SF9 Workspace, locate the top action toolbar.
  2. Click the green button: **"Export All SF9 (.ZIP of Excel)"** (`ri-folder-zip-line`).
  3. The backend system loops through every enrolled student in the section, populates the DepEd SF9 template with their quarterly grades, generates individual Excel files, and packages them into a single compressed `.ZIP` file.
  4. The file `SF9_Section_[SectionName]_[SY].zip` automatically downloads to your workstation.

---

### 7.6 Managing Teacher Profile and Password Credentials
* **Purpose:** To update contact information and change account security passwords.
* **Access Path:** Click **"Settings"** on the teacher sidebar (`teacherSettings.html`).

#### Step-by-Step Procedure:
1. Open `teacherSettings.html`.
2. Review your personal profile details (Name, Employee ID, Email, Assigned Faculty Cluster).
3. To update your password:
   - Enter your **Current Password**.
   - Enter your **New Password**.
   - Confirm your **New Password**.
   - Click **"Update Password"**.
4. The system validates and saves the new credentials.


---

# CHAPTER 8: ADMINISTRATOR AND REGISTRAR PORTAL

### 8.1 Executive Dashboard and Real-Time KPI Metrics
* **Purpose:** To provide school leadership and the registrar with real-time operational awareness over admissions, enrollment counts, faculty, and academic compliance.
* **Access Path:** Automatically displayed upon logging into an account with the `admin` role (`adminDashboard.html`).
* **Prerequisites:** Authenticated administrator account.

```text
[Insert Figure 28: Administrator Executive Dashboard with KPI Metrics and Real-Time Alerts Here]
```

#### Key Dashboard Metrics & Widgets:
1. **Key Performance Indicator (KPI) Cards:**
   - **Total Applications:** All applications received for the active school year.
   - **Approved Applications:** Applications evaluated and ready for physical document submission.
   - **Officially Enrolled Learners:** Total count of learners confirmed and active in sections.
   - **Pending Verification:** Documents requiring administrative review.
   - **Active Faculty Count:** Number of active teaching staff.
   - **Configured Sections:** Total class sections created across Kindergarten to Grade 6.
2. **Actionable Alerts Panel:** Displays urgent operational notices, such as:
   - On-site document verification appointments scheduled for today.
   - Unassigned enrollees requiring section placement.
   - Grade encoding deadlines and pending teacher grading submissions.
3. **Enrollment Trend & Demographic Charts:** Graphical breakdown of enrollees by grade level and gender distribution (Male vs. Female).
4. **Quick Navigation Tiles:** Direct shortcuts to **Applications**, **Document Slots**, **Students Database**, **Sections**, **Timetable Builder**, and **Settings**.

---

### 8.2 Managing Admissions and Application Lifecycles
* **Purpose:** To evaluate, approve, reject, and transition admission applications into permanent student enrollments.
* **Access Path:** Click **"Applications"** on the administrator sidebar (`applications.html`).

```text
[Insert Figure 29: Administrator Applications Management Hub (New Applications Table) Here]
```

---

#### 8.2.1 Processing New Applications (Evaluating, Approving, Rejecting, Enrolling)
1. On `applications.html`, select the **"New Applications"** tab (`newApplications`).
2. Filter the table using the top control bar:
   - **Status Filter:** *All Statuses*, *Submitted*, *Under Review*, *Approved*, *Enrolled*, *Rejected*.
   - **Grade Level Filter:** *Kindergarten* through *Grade 6*.
   - **Search Box:** Type an Application Reference Number (`VPES-2026-XXXXX`), Learner Name, or LRN.
3. Review the table summary columns: Reference No., Applicant Name, Grade Level, Application Date, Document Upload Status, and Current Status Badge.
4. **Action Menu on Each Row:**
   - Click the **"Action"** dropdown on any applicant row.
   - **View Details:** Opens the complete application dossier modal.
   - **Approve Application:** Validates the application, transitions status to `APPROVED`, sends an automated approval email/SMS, and unlocks on-site appointment booking for the applicant.
   - **Reject Application:** Opens a prompt requiring a specific rejection remark. Sends a notification to the applicant.
   - **Mark as Enrolled:** Once original physical documents have been validated in person, click **"Enroll"**.

---

#### 8.2.2 Inspecting Comprehensive Application Dossiers
* **Target Interface:** Application Details Modal / Page (`applicationDetails.html`)

```text
[Insert Figure 30: Administrator Detailed Application Evaluation and Approval Modal Here]
```

1. Click **"View Details"** on any application record.
2. The complete dossier opens, organized into structured inspection tabs:
   - **Learner Demographics:** Full legal name, LRN, PSA birth cert number, birthdate, sex, age, mother tongue, IP status, 4Ps ID.
   - **Address:** Complete standardized Philippine PSGC residential address.
   - **Family & Guardians:** Father, mother maiden, legal guardian details, and emergency contacts.
   - **SNEd Information:** Special needs diagnosis, manifestations, PWD ID.
   - **Uploaded Documents Viewer:** View embedded high-resolution previews of the uploaded birth certificate, report cards, and certificates.
   - **Application Audit Log:** Chronological history of all state changes and staff remarks.
3. Direct action buttons at the bottom of the modal allow immediate approval, rejection, or enrollment.

---

#### 8.2.3 Managing Re-Enrollment Requests and Bulk Approvals
* **Purpose:** To process continuing student re-enrollment requests for the upcoming school year.
* **Access Path:** Select the **"Re-Enrollment"** tab (`reEnrollmentTab`) on `applications.html`.

```text
[Insert Figure 31: Administrator Continuing Student Re-Enrollment and Promotion Interface Here]
```

1. Click the **"Re-Enrollment"** tab.
2. The table displays all continuing students who submitted re-enrollment confirmations.
3. Review student names, current grade, advancing promotional grade, and submission timestamps.
4. **Individual Processing:**
   - Click **"Approve"** on any row to confirm re-enrollment.
   - Click **"Assign Section"** to place the continuing learner into an active section.
5. **Bulk Approval Feature:**
   - Check the select-all checkbox at the top-left of the table (or select specific learners).
   - Click the green button: **"Bulk Approve Selected"** (`ri-check-double-line`).
   - Confirm the batch action. The system updates all selected records to `APPROVED` simultaneously and dispatches notification emails.

---

#### 8.2.4 Executing Student Year-End Promotion and Grade 6 Graduation
* **Purpose:** To advance eligible students to the next grade level based on academic performance and process Grade 6 graduates.
* **Access Path:** Select the **"Student Promotion"** tab (`studentPromotionTab`) on `applications.html`.

1. **Sub-Tab 1: Promote Learners (`promoSubTabPromote`):**
   - Select the target **Grade Level** (e.g., *Grade 1 to Grade 5*).
   - Click **"Check Promotion Eligibility"**.
   - The system inspects all enrolled students' final general averages from the `grades` table:
     - Students with General Average $\ge 75$: Tagged as **"Eligible for Promotion"**.
     - Students with General Average $< 75$ or incomplete quarterly marks: Tagged with warnings.
   - Select eligible learners and click **"Execute Batch Promotion"**.
   - Promoted students advance to the next higher grade level in the upcoming school year.
2. **Sub-Tab 2: Grade 6 Graduation (`promoSubTabGraduating`):**
   - Click the **"Graduating Students"** sub-tab.
   - The table lists all Grade 6 candidates.
   - Click **"Process Graduation"**.
   - The system updates their lifecycle status to `GRADUATED`, archives their permanent records for SF10 generation, and transitions their accounts to the alumni portal view.

---

### 8.3 Operating the Master Document Repository
* **Purpose:** To manage, inspect, verify, and archive all student credentials across the entire institution.
* **Access Path:** Click **"Documents"** on the administrator sidebar (`documents.html`).

```text
[Insert Figure 32: Administrator Master Document Repository and Verification Modal Here]
```

#### Step-by-Step Procedure:
1. Navigate to `documents.html`.
2. Choose your preferred viewing mode:
   - **Table View (`btnTableView`):** Detailed tabular list of every uploaded file with student name, file type, upload date, and verification status.
   - **Student Dossier View (`btnDossierView`):** Student-centric folder view grouping all credentials under each student's name.
3. Filter by **School Year**, **Grade Level**, **Document Type** (*PSA Birth Certificate*, *SF9*, *SF10*, *Kinder Cert*), or **Verification Status** (*Pending*, *Verified*, *Rejected*).
4. **Verifying a Document:**
   - Click **"Preview"** on any document row to launch the **Enhanced Document Verification Modal**.
   - Inspect the high-resolution image or PDF using the zoom, rotate, and full-screen tools.
   - If valid, click **"Verify / Approve Document"** (`ri-checkbox-circle-line`). The badge turns green (`VERIFIED`).
   - If invalid, click **"Reject Document"** (`ri-close-circle-line`).
   - A dialog prompts: *"Select or enter rejection reason."* Choose from standard presets (*Blurry/Illegible*, *Incorrect Document*, *Missing Pages*, *Uncertified Copy*) or type custom remarks.
   - Click **"Confirm Rejection"**. The system flags the document as rejected and automatically sends an alert to the applicant instructing them to re-upload.

---

### 8.4 Managing On-Site Document Submission Slots and Appointments
* **Purpose:** To configure available appointment schedules for physical document verification and manage attendee check-ins.
* **Access Path:** Click **"Document Slots"** on the administrator sidebar (`documentSlots.html`).

```text
[Insert Figure 33: Administrator Appointment Slot Management and Attendance Roster Here]
```

---

#### 8.4.1 Managing Booked Appointments, Daily Rosters, and Check-ins
1. On `documentSlots.html`, select the **"Bookings"** tab (`tabBtn-bookings`).
2. Use the date picker to select a specific date, or click **"Today"** to load today's scheduled visitors.
3. Filter by **Period** (**All**, **Morning AM**, **Afternoon PM**) or **Status** (**Booked**, **Attended**, **No Show**, **Cancelled**).
4. When a parent arrives at the registrar's window:
   - Locate their entry in the table by scanning the QR code on their Appointment Slip or searching their name.
   - Verify their original physical documents.
   - Click **"Mark Attended"** (`ri-check-line`).
5. Click **"Print Daily Appointment Masterlist"** to generate a printed physical log sheet for security desk check-ins.

---

#### 8.4.2 Adding Individual Slots and Executing the Bulk Slot Generator
1. Switch to the **"Slots Management"** tab (`tabBtn-slots`).
2. **Adding an Individual Slot:**
   - Click **"Add New Slot"** (`btn-primary`).
   - Select the **Slot Date**.
   - Choose the **Time Period** (*Morning 8:00 AM – 11:30 AM* or *Afternoon 1:00 PM – 4:30 PM*).
   - Set the **Maximum Capacity** (e.g., *25 applicants*).
   - Click **"Save Slot"**.
3. **Using the Bulk Slot Generator:**
   - Click the green button: **"Bulk Create Slots"** (`btn-success`).
   - In the modal dialog, select the **Start Date** and **End Date** (e.g., a two-week enrollment period).
   - Select operating days (check *Monday through Friday*; uncheck weekends).
   - Check **Create Morning Slots** and enter morning capacity (e.g., *25*).
   - Check **Create Afternoon Slots** and enter afternoon capacity (e.g., *25*).
   - Click **"Generate Slots"**. The system generates all appointment slots across the calendar in a single batch operation.

---

### 8.5 Maintaining the Master Student Information Database
* **Purpose:** To oversee all active, enrolled, graduated, and transferred students in the institution.
* **Access Path:** Click **"Students"** on the administrator sidebar (`students.html`).

```text
[Insert Figure 34: Administrator Master Student Database and Section Assignment Controls Here]
```

---

#### 8.5.1 Searching, Filtering, and Inspecting Student Profiles
1. On `students.html`, filter the directory using:
   - **Grade Level:** *All Grades*, *Kindergarten* to *Grade 6*.
   - **Section:** Filter by specific section name.
   - **Status:** *All*, *Active Enrolled*, *Unassigned*, *Graduated*, *Transferred Out*, *Archived*.
   - **Search:** Search by 12-digit LRN, Surname, or Given Name.
2. Click on any student row or click **"View Profile"** to open the comprehensive Student Profile Modal containing full personal, academic, and family data.

---

#### 8.5.2 Manual Section Assignment, Section Transfers, and Unassigning
1. To assign an unassigned student to a section:
   - In the student row, click the **"Section"** dropdown.
   - Select the target section. The system displays current section capacity and gender count.
   - Confirm assignment. The student is linked to that section in the `enrollments` table.
2. To transfer a student to another section:
   - Click **"Transfer Section"**.
   - Select the new section and click **"Confirm Transfer"**.
3. To unassign a student:
   - Click **"Unassign"**. The student is moved to the unassigned queue.

---

#### 8.5.3 Running the Automated Gender-Balanced Section Assignment Tool
* **Purpose:** To automatically distribute enrolled students across sections while ensuring equal class sizes and balanced male-to-female ratios.
* **Access Path:** Navigate to `sections.html` and click the **"Assign Students"** tab (`tabBtnAssignStudents`).

#### Step-by-Step Procedure:
1. Select the target **Grade Level** (e.g., *Grade 1*).
2. The interface displays the count of unassigned students and the available sections for that grade with their capacity limits.
3. Click the blue button: **"Auto-Assign Students"** (`btn-primary`).
4. A confirmation modal explains the algorithm:
   - Ranks sections by available capacity.
   - Alternates male and female learners to maintain a 1:1 gender balance.
   - Avoids exceeding classroom capacity thresholds.
5. Click **"Execute Auto-Assignment"**.
6. The system executes the assignment algorithm and presents a summary of allocated students per section.

---

#### 8.5.4 Managing LRN Updates and Account Linking/Unlinking
1. **Updating an LRN:** If an incoming kindergarten learner is officially assigned an LRN by DepEd, locate the student on `students.html`, click **"Update LRN"**, enter the 12-digit number, and save.
2. **Unlinking Accounts:** If a student account was bound to an unauthorized user, click **"Unlink Account"**. The parent user account is detached, allowing the student record to be linked to the proper guardian.

---

### 8.6 Generating School-Wide DepEd Academic Reports
* **Purpose:** To generate institution-wide DepEd statistical reports, permanent academic records, and registries.
* **Access Path:** Click **"Academic Records"** on the administrator sidebar (`academicRecords.html`).

```text
[Insert Figure 35: Administrator Academic Records & School-Wide DepEd Forms Hub Here]
```

#### Step-by-Step Procedures for School-Wide Forms:
1. **Section Masterlist:**
   - Locate the **Section Masterlist** card.
   - Select the target **Grade Level** and **Section**.
   - Click **"Download Masterlist (Excel)"** or **"Print Masterlist"**.
2. **SF4: Monthly Report on Learner Movement & Attendance:**
   - Click **"View & Download SF4"**.
   - Select the reporting **Month and Year**.
   - The system aggregates attendance, registered learners, dropouts, and transfers across all sections into the official school-wide statistical matrix.
   - Download as **Excel** or **PDF**.
3. **SF6: Summarized Report on Promotion & Level of Proficiency:**
   - Click **"View & Download SF6"**.
   - Generates the consolidated school-wide summary of promoted and retained learners across Grades 1–6 (official replacement for DepEd Form 20).
4. **SF7: School Personnel Assignment List & Basic Profile:**
   - Click **"View & Download SF7"**.
   - Automatically compiles faculty plantilla profiles, educational degrees, teaching designations, and daily teaching minutes.
5. **SF10-ES: Learner Permanent Academic Record (Form 137):**
   - Click **"Open SF10 Workspace"**.
   - Search for the specific student by LRN or Name.
   - Click **"Generate SF10-ES"**.
   - The system reads complete historical grades from `grades` and `grades_history`, formats them into the official DepEd SF10-ES layout, and delivers the permanent scholastic record in PDF or Excel.
6. **SPED / SNEd & PWD Registry:**
   - Click **"Generate SNEd Registry"**.
   - Exports the specialized institutional registry of all learners with disabilities, including medical diagnoses, manifestations, and 4Ps coverage.

---

### 8.7 Managing Class Sections and Advisers
* **Purpose:** To configure class sections, assign classroom spaces, designate faculty advisers, and set enrollment capacity caps.
* **Access Path:** Click **"Sections"** on the administrator sidebar (`sections.html`).

```text
[Insert Figure 36: Administrator Section Management and Class Adviser Assignment Interface Here]
```

#### Step-by-Step Procedure:
1. Navigate to `sections.html` (**"Manage Sections"** tab).
2. Click **"Create New Section"** (`btn-primary`).
3. In the section modal, configure:
   - **Section Name:** Enter the official section name (e.g., *Mabini*, *Rizal*, *Bonifacio*).
   - **Grade Level:** Select grade level (*Kindergarten* to *Grade 6*).
   - **Classroom / Room Number:** (e.g., *Room 102*).
   - **Maximum Student Capacity:** (Default: *35* to *40*).
   - **Assigned Class Adviser:** Select a faculty member from the teacher dropdown list.
   - **Section Color Theme:** Choose an accent color for visual differentiation across timetables.
4. Click **"Save Section"**.
5. **Publishing a Section:** Use the **Publish Toggle Switch** on any section card. Only published sections are visible to students and parents during enrollment.

---

### 8.8 Managing the DepEd Elementary Subject Curriculum
* **Purpose:** To manage standard DepEd subjects, curriculum minutes, color codings, and report card display ordering.
* **Access Path:** Click **"Subject Management"** on the administrator sidebar (`subjectManagement.html`).

#### Step-by-Step Procedure:
1. Open `subjectManagement.html`.
2. Filter subjects by **Grade Level** (e.g., *Grade 1*, *Grade 4*).
3. **Adding a Subject:**
   - Click **"Add Subject"**.
   - Enter **Subject Code** (e.g., *MATH-G4*) and **Subject Title** (e.g., *Mathematics*).
   - Set **Weekly Minutes** (e.g., *250 minutes* = 50 min/day).
   - Set **Display Order:** Numeric value determining row order on official SF9 report cards.
   - Select **Subject Color Code** for the timetable builder.
   - Click **"Save Subject"**.
4. **Archiving / Reordering:** Drag subject cards to reorder, or click **"Archive"** to deactivate subjects without deleting historical grade records.

---

### 8.9 Managing Faculty and Teacher Profiles
* **Purpose:** To maintain the official directory of teaching personnel, faculty cluster classifications, and employment records.
* **Access Path:** Click **"Teacher Management"** on the administrator sidebar (`teacherManagement.html`).

#### Step-by-Step Procedure:
1. Navigate to `teacherManagement.html`.
2. Filter by faculty cluster:
   - **All Faculty**
   - **Kindergarten Cluster**
   - **Primary Cluster (Grades 1 to 3)**
   - **Intermediate Cluster (Grades 4 to 6)**
3. Click **"Add New Teacher"** to create a faculty profile:
   - Enter Full Name, DepEd Employee ID, Email, Mobile Number, and Specialization.
4. **View Teacher Weekly Schedule:** Click the **"Timetable"** button on any teacher card to view and print their full weekly teaching load across all sections.

---

### 8.10 Building Class Schedules with Automated Conflict Detection
* **Purpose:** To build conflict-free weekly timetables for all sections and teachers.
* **Access Path:** Click **"Schedule Management"** on the administrator sidebar (`scheduleManagement.html`).

```text
[Insert Figure 37: Administrator Timetable Builder with Automated Conflict Checking Engine Here]
```

---

#### 8.10.1 Navigating the Master Sections Timetable Grid
1. In `scheduleManagement.html`, the default tab is the **Master Sections Calendar** (`tabBtnMasterSectionsCalendar`).
2. Displays all section timetables side by side.
3. Filter by Grade Level to inspect specific cohorts.

---

#### 8.10.2 Creating Schedule Blocks and Automated Conflict Checking
1. Switch to the **"Schedule Editor"** tab (`tabBtnScheduleEditor`).
2. Select the target **Section** (e.g., *Grade 4 - Mabini*).
3. In the **Create Session** side panel, configure:
   - **Subject:** Select subject from curriculum dropdown.
   - **Assigned Teacher:** Select faculty member.
   - **Day(s) of Week:** Check *Monday*, *Tuesday*, *Wednesday*, *Thursday*, *Friday*.
   - **Start Time & End Time:** (e.g., *08:00 AM – 08:50 AM*).
   - **Room:** Enter or confirm classroom number.
4. Click **"Add Session"**.
5. **Real-Time Automated Conflict Detection:**
   - The conflict engine verifies whether:
     - The assigned **Teacher** is already scheduled in another section at the same time.
     - The assigned **Room** is already occupied by another class.
     - The **Section** already has an overlapping subject during that time window.
   - **If a conflict is detected:** The system blocks session creation, flashes a red conflict warning banner, and specifies the exact overlapping section and teacher name.
   - **If no conflict exists:** The block is added to the weekly timetable grid.
6. Click **"Save Schedule"** to commit all changes to the `class_schedules` table.

---

#### 8.10.3 Utilizing Auto-Assign Teacher and Auto-Fill Missing Schedules
* **Auto-Fill Missing Schedules:** Automatically fills open timetable gaps based on DepEd curriculum time allocations.
* **Auto-Assign Teacher:** Automatically assigns qualified teachers based on faculty cluster specializations.

---

#### 8.10.4 Publishing Schedules and Exporting to High-Resolution PNG or JSON
1. Click the **"Publish Schedule"** switch. Once published, the schedule becomes visible on student and teacher dashboards.
2. Click **"Export PNG"** to download a high-resolution image of the complete section timetable for classroom posting.
3. Click **"Export JSON"** for administrative backup.

---

### 8.11 Managing User Accounts and Role Permissions
* **Purpose:** To administer user credentials, assign system roles, and enforce security policies.
* **Access Path:** Click **"User Management"** on the administrator sidebar (`users.html`).

```text
[Insert Figure 38: Administrator User Account Management and Role Modification Dialog Here]
```

---

#### 8.11.1 Creating Staff/Teacher Accounts with Temporary Passwords
1. On `users.html`, click **"Add New User"** (`btn-primary`).
2. In the modal dialog, configure:
   - **Role:** Select `teacher` or `admin`.
   - **Honorific / Title:** *Mr.*, *Ms.*, *Mrs.*, *Dr.*
   - **Full Legal Name**
   - **Email Address**
   - **Contact Number**
   - Click **"Generate Temporary Password"** to produce a secure randomized password.
   - Ensure the checkbox **"Require password change on first login"** is checked (`must_change_password = 1`).
3. Click **"Create Account"**. The system creates the user in Firebase Auth and MySQL and queues a welcome notification.

---

#### 8.11.2 Promoting Teachers to Administrators (Safety Rule Enforcement)
1. In the user list, locate a user with the `teacher` role.
2. Click the **"Edit Role"** button (`ri-shield-user-line`).
3. Select `admin` in the new role dropdown.
4. Click **"Update Role"**.
5. **System Safety Guard:** The system strictly prohibits changing applicant roles and prevents demoting the last remaining active administrator to prevent accidental administrative lockout.

---

#### 8.11.3 Password Resets, Account Suspensions, and Account Deletions
1. **Password Reset:** Click **"Reset Password"** on any user row. An automated password reset link is dispatched to their email.
2. **Account Suspension:** Click **"Suspend Account"** to immediately revoke access for compromised accounts.
3. **Delete User:** Permanently removes unverified or duplicate accounts with full audit logging.

---

### 8.12 Publishing School Announcements and Facebook Sync
* **Purpose:** To broadcast school news, advisories, and emergency suspensions to the portal and sync with the official Facebook Page.
* **Access Path:** Click **"Announcements"** on the administrator sidebar (`announcements.html`).

```text
[Insert Figure 39: Administrator Announcements Management and Facebook Sync Approval Modal Here]
```

---

#### 8.12.1 Creating School Bulletins, Category Tagging, and Priority Pinning
1. On `announcements.html`, click **"Create Announcement"** (`btn-primary`).
2. In the modal editor, configure:
   - **Announcement Title**
   - **Category:** *General*, *Academic*, *Admissions*, *Events*, *Emergency / Suspension*.
   - **Target Audience:** *All Users*, *Teachers Only*, *Parents & Students*.
   - **Content:** Type the bulletin body using rich formatting.
   - **Attachment / Banner Image:** Upload optional announcement flyer.
   - **Priority Pin:** Check **"Pin to Top"** for critical announcements.
   - **Auto-Post to Facebook:** Toggle to automatically publish to the official school Facebook Page via Graph API.
3. Click **"Publish Announcement"**.

---

#### 8.12.2 Reviewing and Approving Synced Facebook Page Posts
1. When official posts are published directly on the VPES Facebook page, the system webhook captures them and places them into the **"Pending Review"** tab (`tabPending`).
2. Click the **"Pending Review"** tab.
3. Click **"Review Post"** on any synced item.
4. A two-column modal displays the Facebook content alongside portal preview formatting.
5. Select the appropriate **Portal Category** and adjust visibility.
6. Click **"Approve & Publish to Portal"**. The announcement immediately appears on the landing page feed.

---

### 8.13 Monitoring Security and System Audit Logs
* **Purpose:** To review an immutable chronological trail of all user actions, logins, status modifications, and data updates.
* **Access Path:** Click **"Audit Logs"** on the administrator sidebar (`auditLogs.html`).

#### Step-by-Step Procedure:
1. Open `auditLogs.html`.
2. Filter the log trail by:
   - **Category Pills:** *All*, *Re-Enrollment*, *Applications*, *Documents*, *Users*, *Sections*, *Settings*.
   - **Date Range:** Filter by specific dates.
3. The table displays: Timestamp, Action Performed, Performed By (User Name & ID), and Description.
4. Click **"View Detail"** on any log row to open the **Audit Detail Modal**, displaying complete before-and-after metadata diffs and system diagnostics.

---

### 8.14 System Settings, School Year Management, and School CMS
* **Purpose:** To configure institutional school identifiers, manage academic calendars, toggle admission gating, and edit public portal content.
* **Access Path:** Click **"Settings"** on the administrator sidebar (`settings.html`).

```text
[Insert Figure 40: Administrator System Settings, Enrollment Gating Switches, and SY Readiness Audit Here]
```

---

#### 8.14.1 Managing Academic School Years and the Activation Readiness Audit
1. In `settings.html`, select the **"School Year"** tab (`schoolYearTab`).
2. **Creating a New School Year:** Click **"Add School Year"** (e.g., *2027–2028*), set official term start and end dates, and save.
3. **The Activation Readiness Audit:**
   - Before activating a new academic school year, click **"Check Activation Readiness"**.
   - The automated readiness engine performs a comprehensive system audit:
     - Verifies that all students in active sections have complete 4th-quarter grades.
     - Confirms that student promotions and Grade 6 graduations have been finalized.
     - Validates that new sections and subject curricula are configured for the target year.
   - If warnings or missing grades exist, the system presents an itemized resolution list.
   - Once all criteria pass, the **"Activate School Year"** button enables, transitioning the institution to the new academic term.

---

#### 8.14.2 Independent Gating for Early Registration, Enrollment, and Re-enrollment
The system features three independent gating switches:
1. **Early Registration Toggle:** Toggle **ON** to accept incoming Kindergarten and Grade 1 pre-registrations. Set start and end calendar dates.
2. **Official Enrollment Toggle:** Toggle **ON** to accept general admissions across all grade levels.
3. **Re-Enrollment Toggle:** Toggle **ON** to open the re-enrollment tab on continuing student dashboards.
*Toggling any switch to OFF immediately locks that form on the public portal and displays official closed advisories.*

---

#### 8.14.3 Updating School Institutional Profile and DepEd Identifiers
1. Click the **"School Profile"** tab (`schoolProfileTab`).
2. Update official DepEd data:
   - **Official School Name:** *Vinzons Pilot Elementary School*
   - **DepEd School ID:** *112937*
   - **Region:** *Region V - Bicol*
   - **Division:** *Camarines Norte*
   - **District:** *Vinzons*
   - **School Head / Principal Full Name**
   - **Upload Official School Logo**
   - **Official School Email Address, Contact Number, and Physical Address**
3. Click **"Save Institutional Profile"**. All generated DepEd forms instantly adopt the updated identifiers.

---

#### 8.14.4 Landing Page Content Management System (Hero, Cards, Media)
1. Click the **"System / CMS"** tab (`systemTab`).
2. Update public landing page content:
   - **Hero Banner:** Edit headline text, sub-headline, and upload hero background photography.
   - **Feature Cards:** Edit the title and descriptions of portal capability cards.
   - **Live Preview:** Inspect changes in real time on the embedded preview panel.
3. Click **"Save Landing Page Content"**.

---

#### 8.14.5 Configuring Mailer, SMS Gateway, and External API Credentials
1. In the integration settings card, configure:
   - **Hostinger SMTP / Mailer Settings:** Host, port, username, password, encryption type (`TLS`/`SSL`).
   - **Semaphore SMS API Key:** Enter active API token for mobile OTP dispatch.
   - **Facebook Graph API:** Enter Page Access Token, App ID, App Secret, and Webhook verification token.
2. Click **"Test Connection"** to verify service connectivity before saving.


---

# CHAPTER 9: OFFICIAL DEPED SCHOOL FORMS (SF) REFERENCE GUIDE

### 9.1 Legal and Regulatory Framework
The automated reporting modules in VPES-SIMS comply strictly with the policies, layouts, and data reporting standards established by the Department of Education:
* **DepEd Order No. 4, s. 2014:** *Adoption of the Modified School Forms (SFs) for Public Elementary and Secondary Schools.*
* **DepEd Order No. 58, s. 2017:** *Adoption of New School Forms for Kindergarten, Senior High School, Alternative Learning System, Health and Nutrition, and Permanent Records.*
* **DepEd Order No. 8, s. 2015:** *Policy Guidelines on Classroom Assessment for the K to 12 Basic Education Program.*
* **Republic Act No. 10173:** *Data Privacy Act of 2012.*

---

### 9.2 Complete School Forms Matrix and Specification Guide

| Form Code | Official DepEd Form Title | Generating Role | Output Formats | Primary Data Sources | Legal & Regulatory Purpose |
| :--- | :--- | :---: | :---: | :--- | :--- |
| **SF 1** | **School Register** | Teacher / Adviser | Excel (.xlsx), PDF | `students`, `student_addresses`, `student_guardians` | Replaces Form 1. Master directory of enrolled learners containing demographic, socio-economic, and parent data. |
| **SF 2** | **Daily Attendance Report** | Teacher / Adviser | Excel (.xlsx), PDF | `enrollments`, daily attendance logs | Replaces Form 2. Monthly record of daily attendance, absences, tardiness, and dropouts per section. |
| **SF 3** | **Books Issued and Returned** | Teacher / Adviser | Excel (.xlsx) | `enrollments`, textbook inventories | Replaces Form 3. Textbook accountability record tracking learning materials distributed and retrieved. |
| **SF 4** | **Monthly Report on Learner Movement & Attendance** | Admin / Registrar | Excel (.xlsx), PDF | Aggregated from all section SF2 records | Replaces Form 3. Consolidated school-level monthly summary of registered learners, attendance rates, and dropouts. |
| **SF 5** | **Report on Promotion & Level of Proficiency** | Teacher / Adviser | Excel (.xlsx), PDF | `grades`, `enrollments`, `students` | Replaces Form 18-E1. End-of-school-year report listing promoted and retained learners with final general averages. |
| **SF 6** | **Summarized Report on Promotion & Level of Proficiency** | Admin / Registrar | Excel (.xlsx), PDF | Aggregated from all section SF5 records | Replaces Form 20. Consolidated school-wide statistical distribution of learner promotion and proficiency levels. |
| **SF 7** | **School Personnel Assignment List & Basic Profile** | Admin / Registrar | Excel (.xlsx), PDF | `teachers`, `class_schedules`, `sections` | Replaces Forms 12, 19, 29, 31. Faculty plantilla profile, educational background, and daily teaching minute loads. |
| **SF 8** | **Learner Basic Health & Nutrition Report** | Teacher / Adviser | Excel (.xlsx) | Health assessment logs, `students` | Baseline and end-of-year nutritional status assessment based on height, weight, and Body Mass Index (BMI). |
| **SF 9** | **Learner Progress Report Card (Form 138)** | Teacher / Adviser | Excel (.xlsx), PDF, Batch ZIP | `grades`, `mapeh_subgrades`, `enrollments` | Replaces Form 138. The official individual progress report card issued to parents showing quarterly academic grades and core values. |
| **SF 10-ES** | **Learner Permanent Academic Record (Form 137)** | Admin / Registrar | Excel (.xlsx), PDF | `students`, `grades_history`, `enrollments` | Replaces Form 137. The permanent scholastic transcript recording complete multi-year elementary grades for transfer or graduation. |
| **SNEd** | **SPED / SNEd & PWD Institutional Registry** | Admin / Registrar | Excel (.xlsx) | `applications`, `application_personal_info` | Institutional directory of learners under the Special Needs Education program, medical diagnoses, and PWD numbers. |

---

# CHAPTER 10: TROUBLESHOOTING, SYSTEM MESSAGES, AND FREQUENTLY ASKED QUESTIONS (FAQ)

### 10.1 Common User Errors and Step-by-Step Resolutions

#### Issue 1: "I did not receive the 6-Digit OTP verification code."
* **Cause:** Email deliverability delays, incorrect mobile number format, or spam folder filtering.
* **Resolution:**
  1. Check your email **Spam** or **Junk** folder for messages from `vpes.portal@gmail.com`.
  2. Ensure your mobile number was entered in the valid 11-digit Philippine format (`09XXXXXXXXX`).
  3. Wait 60 seconds until the countdown timer expires, then click **"Resend verification code"**.
  4. If delays persist, choose email verification instead of SMS.

#### Issue 2: "My LRN is rejected during account linking."
* **Cause:** LRN typographical error, incorrect birthdate, or the LRN is already linked to another registered email.
* **Resolution:**
  1. Verify the 12-digit number against your child's official DepEd SF9 report card.
  2. Confirm that the birthdate entered exactly matches the official DepEd registration records.
  3. If another family member previously linked the student, contact the school registrar to request an account unlinking.

#### Issue 3: "The Appointment Booking section is locked / inaccessible."
* **Cause:** The admission application has not yet been approved by the school administrator.
* **Resolution:**
  1. Appointment slot booking unlocks automatically once the application reaches **Stage 4: Admission Approval**.
  2. Allow 1 to 2 business days for the admissions committee to verify your submitted BEEF data and digital documents.
  3. Check your registered email for status updates or requests for document clarification.

#### Issue 4: "Database conflict error on local system startup (Port 3306)."
* **Cause:** Another MySQL service (such as `MySQL84`) is running on the workstation, blocking XAMPP's MySQL/MariaDB from binding to port `3306`.
* **Resolution:**
  1. Press `Win + R`, type `services.msc`, and press **Enter**.
  2. Locate `MySQL84` (or any other standalone MySQL service), right-click it, and select **Stop**.
  3. Open the **XAMPP Control Panel** and click **Start** next to MySQL.
  4. Verify that MySQL starts successfully and binds to port `3306`.

---

### 10.2 Document Upload and Format Error Handling
* **Error: "File exceeds maximum size limit (5 MB)."**
  - *Solution:* Compress the image or PDF using an online compressor before uploading, or capture the document at standard smartphone resolution rather than ultra-high resolution.
* **Error: "Unsupported file format."**
  - *Solution:* The system strictly accepts `.pdf`, `.jpg`, `.jpeg`, and `.png` files. Convert word processor files (`.docx`) or proprietary formats to PDF before uploading.
* **Status: "Needs Re-upload" with reviewer comment.**
  - *Solution:* Read the specific feedback note (e.g., *"PSA Birth Certificate is blurred; cannot read birth certificate number"*). Take a clearer, well-lit photograph or flatbed scan and upload it through the **Document Requirements** section.

---

### 10.3 Schedule Conflict Warning Troubleshooting
* **Warning: "Teacher Schedule Conflict Detected!"**
  - *Cause:* The administrator is attempting to assign a faculty member to a section during a time period when that teacher is already scheduled in another section.
  - *Resolution:* Inspect the conflict banner to identify the overlapping section, adjust the proposed time range, or assign an alternate available teacher.
* **Warning: "Classroom / Room Conflict Detected!"**
  - *Cause:* Two different sections are assigned to the same physical room number at the same time.
  - *Resolution:* Assign a different available room number in the session editor.

---

### 10.4 School Year Activation Readiness Error Resolution
* **Error: "Cannot Activate School Year: Missing Student Grades Detected."**
  - *Cause:* One or more teachers have not submitted final 4th-quarter grades for active sections in the current school year.
  - *Resolution:* Click **"View Itemized Report"** on the Activation Readiness modal to identify the specific sections and teachers with missing grades. Notify the concerned faculty to finalize grade encoding before re-attempting school year activation.
* **Error: "Cannot Activate School Year: Student Promotions Incomplete."**
  - *Cause:* Eligible students have not been formally promoted or graduated.
  - *Resolution:* Navigate to `applications.html` > **Student Promotion**, execute batch promotions for eligible learners, and process Grade 6 graduations.

---

### 10.5 Technical Support and Helpdesk Directory
For institutional assistance, data correction requests, or technical support, please contact the school administration:
* **Registrar's Office:** Vinzons Pilot Elementary School, Vinzons, Camarines Norte
* **Office Hours:** Monday to Friday, 8:00 AM – 5:00 PM (excluding public holidays)
* **Official Institutional Email:** `vpes.portal@gmail.com`
* **DepEd School Identifier:** School ID 112937

---

# APPENDIX: GLOSSARY OF TERMS & ACRONYMS

* **BEEF:** Basic Education Enrollment Form — The standard official enrollment form mandated by the Department of Education for public and private elementary and secondary schools.
* **CMS:** Content Management System — Built-in administrative tools allowing school leaders to update public landing page text, banners, and media.
* **DepEd:** Department of Education — The executive department of the Philippine government responsible for governing and overseeing the Philippine basic education system.
* **FPDF / FPDI:** Free PDF / FPDI PDF Parser — Software libraries used by the system to dynamically generate and manipulate high-resolution PDF documents.
* **K-12 / MATATAG Curriculum:** The national basic education curriculum enacted under Republic Act 10533 and updated by the DepEd MATATAG agenda.
* **LIS:** Learner Information System — The Department of Education's centralized national web-based registry of learners.
* **LRN:** Learner Reference Number — A unique 12-digit permanent identification number issued by DepEd to every learner in the Philippine basic education system.
* **MAPEH:** Music, Arts, Physical Education, and Health — An integrated core subject in the Philippine elementary curriculum whose quarterly rating is derived from sub-component averages.
* **mPDF:** A PHP library which generates PDF files from UTF-8 encoded HTML.
* **OTP:** One-Time Password — A 6-digit cryptographic security code dispatched via SMS or email to verify user identity during registration and account recovery.
* **PhpSpreadsheet:** A pure PHP library for reading and writing spreadsheet files, utilized by VPES-SIMS to compile and populate official DepEd `.xlsx` templates.
* **PSGC:** Philippine Standard Geographic Code — A systematic classification and coding of geographic areas in the Philippines (Regions, Provinces, Municipalities, Barangays).
* **RA 10173:** Republic Act No. 10173, known as the *Data Privacy Act of 2012*, governing the collection, storage, and processing of personal identifiable information.
* **RBAC:** Role-Based Access Control — A security access governance mechanism restricting system capabilities according to verified user roles (`admin`, `teacher`, `applicant`, `student`).
* **SF:** School Form — Standardized administrative and academic reporting templates mandated by DepEd Orders (SF1 through SF10).
* **SNEd:** Special Needs Education — Specialized educational programs and accommodations designed for learners with disabilities, giftedness, or other special needs.
* **SSES:** Special Science Elementary School — A specialized elementary education program focusing on advanced science, mathematics, and research curricula.
* **SY:** School Year — The official annual academic operational period (e.g., *S.Y. 2026–2027*).
* **VPES:** Vinzons Pilot Elementary School — The public elementary educational institution in Camarines Norte for which this system was developed.
* **VPES-SIMS:** Vinzons Pilot Elementary School – Student Information and Management System.

---

### DOCUMENT CONTROL & VERIFICATION SIGN-OFF

* **Document Version:** 1.0.0 (Production Release)
* **Author / System Architect:** VPES-SIMS Development Team
* **Reviewed & Verified Against Codebase:** November 2026
* **Academic Submission Status:** Approved for inclusion in Project Research Manuscript / Thesis Appendices
* **Target Audience:** Public Users, Applicants, Students, Teachers, Registrars, Administrators, Academic Evaluation Panels
