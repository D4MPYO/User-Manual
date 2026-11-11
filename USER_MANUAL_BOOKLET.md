# APPENDIX: SYSTEM USER MANUAL
## Vinzons Pilot Elementary School – Student Information and Management System (VPES-SIMS)
*DepEd School ID: 112937 | District of Vinzons | Division of Camarines Norte | Region V – Bicol*

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

# [SYSTEM OVERVIEW & TECHNICAL SPECIFICATIONS]

### SYSTEM IDENTIFICATION & OVERVIEW
The **Vinzons Pilot Elementary School – Student Information and Management System (VPES-SIMS)** is an enterprise web-based school administration platform engineered for Vinzons Pilot Elementary School (DepEd School ID: 112937) in Vinzons, Camarines Norte. 

Developed as a capstone research project under the **Department of Computer Studies, Camarines Norte State College (CNSC)**, the system replaces paper-based workflows with a secure, centralized, and cloud-hosted solution. The platform digitizes remote student enrollment (DepEd BEEF compliance), on-site document verification appointment scheduling, section management with dual-panel drag-and-drop gender balancing, quarterly academic grading, automated report card generation (SF9), and direct compilation of official DepEd School Forms (SF1, SF2, SF3, SF4, SF5, SF6, SF7, SF8, SF10-ES, and SNEd Registry).

### TECHNICAL ARCHITECTURE & DEPLOYMENT
* **Deployment Model:** Production Cloud Server hosted on **Hostinger Cloud Infrastructure** with SSL/TLS encryption.
* **Authentication & Security:** Firebase Authentication with Role-Based Access Control (Admin, Teacher, Student/Parent), password hashing, automated session timeouts, and 5-second countdown safety locks for high-risk actions.
* **Client-Side Requirements:**
  - Modern Web Browser (Google Chrome, Microsoft Edge, Mozilla Firefox, or Safari).
  - Screen Display: Desktop/Laptop (1366 × 768 or higher) and Mobile/Tablet responsive interfaces.
  - Active Internet Connection (minimum 2 Mbps recommended).
  - Built-in PDF reader for previewing and downloading official DepEd reports.

---

# TABLE OF CONTENTS

* **SECTION 1: SYSTEM OVERVIEW & ARCHITECTURE**
* **SECTION 2: USER AUTHENTICATION & ACCESS CONTROL (Figures 1–7)**
* **SECTION 3: PUBLIC LANDING PAGE & GUEST PORTAL (Figures 8–14)**
* **SECTION 4: ONLINE ADMISSIONS & DEPED BEEF APPLICANT PORTAL (Figures 15–27)**
* **SECTION 5: DOCUMENT VERIFICATION & APPOINTMENT SCHEDULER (Figures 28–35)**
* **SECTION 6: ENROLLED STUDENT & PARENT PORTAL (Figures 36–43)**
* **SECTION 7: TEACHER & CLASS ADVISER PORTAL (Figures 44–54)**
* **SECTION 8: ADMINISTRATOR & REGISTRAR OPERATIONS (Figures 55–87)**
  * 8.1 Executive Dashboard & KPI Analytics (Figures 55–58)
  * 8.2 Application Lifecycle & Intake Evaluation (Figures 59–62)
  * 8.3 Document Repository & Verification (Figures 63–64)
  * 8.4 Appointment Slots & Intake Capacity (Figures 65–66)
  * 8.5 Student Master Database & LRN Updates (Figures 67–69)
  * 8.6 Section Management & Timetable Scheduling (Figures 70–75)
  * 8.7 User Administration & Security Audit Logs (Figures 76–80)
  * 8.8 School Year Management & System CMS (Figures 81–84)
  * 8.9 School Forms & Official Reports Center (Figure 85)
  * 8.10 Administrative Utilities & Certificate Templates (Figures 86–87)
* **SECTION 9: OFFICIAL DEPED SCHOOL FORMS (SF) MATRIX**
* **SECTION 10: TROUBLESHOOTING & FREQUENTLY ASKED QUESTIONS (FAQ)**

---

---

### SYSTEM LANDING PAGE INTERFACE AND INSTITUTIONAL BRANDING
**Header:** SYSTEM ACCESS & BRANDING  
**Figure 1. System Landing Page Interface and Institutional Branding**  
> **Figure Description:** Capture index.html displaying the top navigation bar, institutional logo, VPES hero headline, admission status banner, and the primary "Enroll Now" and "Login" buttons

**Interface Controls & Elements:**

1. **School Logo & Header** – Displays official VPES and DepEd seals, school name, and School ID: 112937.
2. **Navigation Bar** – Provides quick access to Home, About Us, Academic Programs, Announcements, and Contact.
3. **Admission Status Ribbon** – Real-time dynamic indicator displaying whether Early Registration or Enrollment is active.
4. **Enroll Now CTA Button** – Directs incoming kindergarten learners and transferees to the admission application workflow.
5. **Login Header Button** – Launches the integrated authentication modal (#authModal) for all user roles.
6. **Announcements Feed** – Highlights the latest school bulletins, advisories, and Facebook-synced posts.

---

### INTEGRATED AUTHENTICATION MODAL – USER SIGN-IN INTERFACE
**Header:** USER AUTHENTICATION & SECURITY  
**Figure 2. Integrated Authentication Modal – User Sign-In Interface**  
> **Figure Description:** Capture #authModal on index.html displaying the "Welcome Back!" header, Email or Phone Number field, Password input with eye unmask toggle, "Sign In to VPES" button, and "Forgot Password?" link

**Interface Controls & Elements:**

1. **Email or Mobile Input** – Enter registered email address or 11-digit Philippine mobile phone number.
2. **Password Input Field** – Enter account password with secure masked characters.
3. **Password Visibility Toggle** – Click eye icon to show or hide entered password characters.
4. **Sign In to VPES Button** – Submits credentials to Firebase Authentication and routes to role dashboard.
5. **Forgot Password Link** – Opens password recovery interface to request an email reset link.
6. **Register Switch Link** – Switches modal from sign-in view to new user registration view.

---

### INTEGRATED AUTHENTICATION MODAL – ACCOUNT REGISTRATION VIEW
**Header:** USER AUTHENTICATION & SECURITY  
**Figure 3. Integrated Authentication Modal – Account Registration View**  
> **Figure Description:** Capture #authModal switched to registration mode showing inputs for First Name, Middle Name, Last Name, Email, Phone Number, Password, Confirm Password, and reCAPTCHA

**Interface Controls & Elements:**

1. **Legal Name Inputs** – Enter applicant/parent First Name, Middle Name (optional), and Last Name.
2. **Email Address Field** – Enter a valid email address for application updates and appointment receipts.
3. **Mobile Phone Number** – Enter active 11-digit mobile number for mandatory SMS OTP verification.
4. **Password & Confirm Fields** – Create a secure password (minimum 8 characters with numbers and symbols).
5. **Create Account Button** – Validates form entries and dispatches a 6-digit SMS verification code.
6. **Back to Sign In Link** – Returns modal to the sign-in interface.

---

### INTEGRATED AUTHENTICATION MODAL – 6-DIGIT PHONE OTP VERIFICATION SCREEN
**Header:** USER AUTHENTICATION & SECURITY  
**Figure 4. Integrated Authentication Modal – 6-Digit Phone OTP Verification Screen**  
> **Figure Description:** Capture #modal-otpScreen inside #authModal displaying the masked phone number, the 6 sequential OTP input boxes, and the countdown timer

**Interface Controls & Elements:**

1. **Masked Phone Display** – Displays target mobile number with privacy masking (e.g., 09******890).
2. **6-Digit Sequential Input Cells** – Auto-advancing digit boxes for entering the SMS verification code.
3. **Resend Code Timer** – 60-second countdown before a new OTP code can be requested.
4. **Verify & Proceed Button** – Validates OTP token with Semaphore SMS gateway and completes registration.
5. **Edit Phone Number Link** – Returns to previous screen to correct a mistyped mobile number.

---

### MANDATORY FIRST-LOGIN PASSWORD CHANGE MODAL
**Header:** USER AUTHENTICATION & SECURITY  
**Figure 5. Mandatory First-Login Password Change Modal**  
> **Figure Description:** Capture the firstLoginPasswordModal.js dialog prompting the user to replace their temporary password with a new personal password

**Interface Controls & Elements:**

1. **Temporary Password Notice** – Informs user that default admin-assigned credentials must be replaced.
2. **New Password Field** – Input secure personal password meeting complexity standards.
3. **Confirm New Password** – Re-enter password to verify identical match.
4. **Password Strength Meter** – Visual bar indicating password robustness (Weak, Medium, Strong).
5. **Update Password & Continue** – Commits new password hash and unlocks portal dashboard access.

---

### INTEGRATED AUTHENTICATION MODAL – PASSWORD RECOVERY INTERFACE
**Header:** USER AUTHENTICATION & SECURITY  
**Figure 6. Integrated Authentication Modal – Password Recovery Interface**  
> **Figure Description:** Capture #modal-recoveryForm inside #authModal displaying the email input, "Send Reset Link" button, and "Back to Login" button

**Interface Controls & Elements:**

1. **Recovery Instructions** – Explains password reset procedure via verified registered email.
2. **Registered Email Field** – Enter the email address associated with the portal account.
3. **Send Reset Link Button** – Dispatches an official password recovery link via Hostinger SMTP.
4. **Back to Sign In Button** – Closes recovery view and returns to the standard login screen.

---

### SECURE SIGN-OUT CONFIRMATION MODAL
**Header:** USER AUTHENTICATION & SECURITY  
**Figure 7. Secure Sign-Out Confirmation Modal**  
> **Figure Description:** Capture logoutModal.js displaying the "Are you sure you want to log out?" confirmation dialog

**Interface Controls & Elements:**

1. **Sign-Out Prompt** – Security dialog asking user to confirm termination of the authenticated session.
2. **Confirm Sign Out Button** – Clears cached tokens, logs out of Firebase, and redirects to index.html.
3. **Cancel Button** – Dismisses the dialog and keeps the current user session active.

---

### PUBLIC HERO SECTION WITH REAL-TIME ADMISSION GATING STATUS
**Header:** PUBLIC LANDING PAGE & GUEST PORTAL  
**Figure 8. Public Hero Section with Real-Time Admission Gating Status**  
> **Figure Description:** Capture the top section of index.html showing the dynamic enrollment status pill ("Early Registration Open", "Regular Enrollment Active", or "Admissions Closed")

**Interface Controls & Elements:**

1. **School Hero Headline** – DepEd institutional motto and Vinzons Pilot Elementary School banner.
2. **Admission Status Badge** – Real-time pill indicating current gating state (Early Reg, Enrollment, Closed).
3. **Primary Enrollment CTA** – Direct action button to initiate online application during open periods.
4. **Public Advisory Message** – Informs parents of upcoming DepEd enrollment dates and office hours.

---

### PUBLIC SCHOOL ANNOUNCEMENTS SECTION ON LANDING PAGE
**Header:** PUBLIC LANDING PAGE & GUEST PORTAL  
**Figure 9. Public School Announcements Section on Landing Page**  
> **Figure Description:** Capture the announcements section on index.html displaying the three latest announcement cards with category badges, dates, and "Read More" buttons

**Interface Controls & Elements:**

1. **Section Title & Subheading** – Official School Advisories, DepEd Memoranda, and News.
2. **Announcement Cards Grid** – Displays thumbnail, headline, publication date, and summary.
3. **Category Badges** – Visual tags (Emergency Suspension, Academic Advisory, Event Notice).
4. **Read More Action** – Launches the full announcement lightbox modal (#announcementModal).
5. **View All Bulletins Button** – Opens the historical archive modal containing past announcements.

---

### ANNOUNCEMENT DETAIL LIGHTBOX MODAL
**Header:** PUBLIC LANDING PAGE & GUEST PORTAL  
**Figure 10. Announcement Detail Lightbox Modal**  
> **Figure Description:** Capture #announcementModal on index.html showing the full announcement headline, publication date, author role, full content text, and attached image

**Interface Controls & Elements:**

1. **Modal Close Button (×)** – Dismisses the announcement lightbox.
2. **Announcement Title Header** – Full official bulletin headline.
3. **Metadata Bar** – Displays publishing date, time, and posting administrator name.
4. **High-Resolution Image Viewer** – Embedded official photo or DepEd memorandum scan.
5. **Formatted Bulletin Body** – Full text announcement content with formatted paragraphs.

---

### ALL ANNOUNCEMENTS ARCHIVE LIGHTBOX MODAL
**Header:** PUBLIC LANDING PAGE & GUEST PORTAL  
**Figure 11. All Announcements Archive Lightbox Modal**  
> **Figure Description:** Capture #announcementsArchiveModal displaying the searchable grid of all historical announcements with category filter pills and pagination

**Interface Controls & Elements:**

1. **Search Announcements Input** – Filters bulletins by keyword, title, or date.
2. **Category Filter Pills** – Filter by All, Emergency Suspensions, General Advisories, or DepEd Memos.
3. **Archive List Items** – Chronological cards of all past bulletins.
4. **Close Archive Button** – Dismisses modal and returns to landing page view.

---

### ACADEMIC PROGRAMS AND CURRICULUM OFFERINGS SECTION
**Header:** PUBLIC LANDING PAGE & GUEST PORTAL  
**Figure 12. Academic Programs and Curriculum Offerings Section**  
> **Figure Description:** Capture the academic programs section on index.html displaying cards for Kindergarten, Primary, Intermediate, SSES (Science Curriculum), and SNEd (Special Needs)

**Interface Controls & Elements:**

1. **DepEd K-12 Elementary Card** – Standard elementary basic education curriculum overview.
2. **SSES Special Science Card** – Information on the Special Science Elementary School program.
3. **SNEd Inclusive Education Card** – Specialized programs for learners with disabilities and special needs.
4. **Curriculum Competencies Link** – Overview of DepEd learning areas and school facilities.

---

### ADMISSION REQUIREMENTS CHECKLIST BY GRADE LEVEL
**Header:** PUBLIC LANDING PAGE & GUEST PORTAL  
**Figure 13. Admission Requirements Checklist by Grade Level**  
> **Figure Description:** Capture the requirements section on index.html displaying tabbed checklists for Kindergarten, Transferees, and Balik-Aral applicants

**Interface Controls & Elements:**

1. **Grade Level Tabs** – Select between Kindergarten, Grade 1 to 6 Transferee, or Balik-Aral.
2. **Mandatory Documents List** – Itemized list (PSA Birth Certificate, SF9 Report Card, ID Photos).
3. **Document Format Guidelines** – Instructions on clear scanning, maximum file size, and accepted formats.
4. **Enrollment Help Desk Info** – Contact numbers of the school registrar for inquiries.

---

### VPES DATA PRIVACY POLICY INTERFACE
**Header:** PUBLIC LANDING PAGE & GUEST PORTAL  
**Figure 14. VPES Data Privacy Policy Interface**  
> **Figure Description:** Capture the privacy policy modal or page displaying compliance with RA 10173 (Data Privacy Act of 2012) and learner information protection terms

**Interface Controls & Elements:**

1. **RA 10173 Statutory Notice** – Official statement of compliance with Philippine Data Privacy Act.
2. **Data Collection Scope** – Details personal, demographic, and academic data collected.
3. **Storage & Protection Protocols** – Explains SSL encryption and role-based access security.
4. **Close / Accept Button** – Closes the privacy policy dialogue.

---

### STUDENT TYPE SELECTION MODAL (NEW APPLICANT VS. EXISTING STUDENT)
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 15. Student Type Selection Modal (New Applicant vs. Existing Student)**  
> **Figure Description:** Capture the studentTypeModal.js dialog asking the user to choose between "New Student / Transferee" and "Existing / Currently Enrolled Student"

**Interface Controls & Elements:**

1. **New Student / Transferee Option** – Launches the online admission application form (SF1).
2. **Existing Student Option** – Routes continuing learners to account linking via 12-digit LRN.
3. **Selection Information Text** – Explains requirements for each enrollment category.
4. **Dismiss Modal Option** – Exits back to portal home.

---

### STUDENT TYPE CONFIRMATION DIALOG
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 16. Student Type Confirmation Dialog**  
> **Figure Description:** Capture the confirmation dialog verifying the selected student category before proceeding to form rendering

**Interface Controls & Elements:**

1. **Selected Category Summary** – Confirms choice (e.g., Incoming Kindergarten or Transferee).
2. **Confirm & Proceed Button** – Commits choice and renders the target application form.
3. **Change Selection Button** – Returns to the selection modal to alter choice.

---

### LRN VERIFICATION AND ACCOUNT LINKING MODAL
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 17. LRN Verification and Account Linking Modal**  
> **Figure Description:** Capture the linkAccountModal.js dialog showing inputs for 12-digit LRN, Student Birthdate, and "Verify & Link Record" button

**Interface Controls & Elements:**

1. **12-Digit LRN Input** – Enter learner's official DepEd Learner Reference Number.
2. **Learner Birth Date Picker** – Verification date of birth to authenticate identity.
3. **Verify & Link Record Button** – Queries database and links student record to user account.
4. **Error Feedback Alert** – Displays warning if LRN and birth date do not match existing records.

---

### ONLINE ADMISSION FORM – STEP 1: SCHOOL INFORMATION & GRADE LEVEL SELECTION
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 18. Online Admission Form – Step 1: School Information & Grade Level Selection**  
> **Figure Description:** Capture the top of applicationform.html showing the active School Year input, Grade Level dropdown, and Learner Status selection buttons

**Interface Controls & Elements:**

1. **School Year Field** – Pre-populated active academic school year (e.g., S.Y. 2026–2027).
2. **Grade Level Dropdown** – Choose target grade level (Kindergarten to Grade 6).
3. **Learner Status Radios** – Select No LRN (Incoming Kinder), With LRN, or Returning (Balik-Aral).
4. **Next Step Button** – Validates selection and advances to Step 2 (Demographic Information).

---

### ONLINE ADMISSION FORM – STEP 2: STUDENT DEMOGRAPHIC & BEEF INFORMATION
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 19. Online Admission Form – Step 2: Student Demographic & BEEF Information**  
> **Figure Description:** Capture Form Card 2 showing fields for PSA Birth Certificate Number, Learner Name (Last, First, Middle, Extension), Birthdate, Sex, Indigenous People (IP) affiliation, and Mother Tongue

**Interface Controls & Elements:**

1. **PSA Birth Certificate Registry No.** – Official civil registrar birth certificate number.
2. **Legal Learner Name Inputs** – First Name, Middle Name, Last Name, and Name Extension (Jr./III).
3. **Birth Date & Age Calculator** – Date of birth picker with automated age computation.
4. **Sex at Birth Radios** – Male or Female selection as recorded on birth certificate.
5. **Mother Tongue Dropdown** – Primary language spoken at home (e.g., Tagalog, Bikol).
6. **IP & 4Ps Indicators** – Checkboxes for Indigenous People group and 4Ps beneficiary status.

---

### ONLINE ADMISSION FORM – STEP 3: PSGC CASCADING GEOGRAPHIC RESIDENTIAL ADDRESS
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 20. Online Admission Form – Step 3: PSGC Cascading Geographic Residential Address**  
> **Figure Description:** Capture Form Card 3 showing cascading dropdowns for Region, Province, Municipality (Vinzons), Barangay, and Street Address inputs

**Interface Controls & Elements:**

1. **Region Selector** – Administrative region (Default: Region V - Bicol).
2. **Province Selector** – Province dropdown (Default: Camarines Norte).
3. **Municipality Selector** – Municipality dropdown (Default: Vinzons).
4. **Barangay Dropdown** – Cascading list of Vinzons barangays (Poblacion, Calangcawan, etc.).
5. **Street / Sitio Address** – House number, street name, or sub-village identifier.
6. **Zip Code Field** – Auto-filled postal code (4603 for Vinzons).

---

### ONLINE ADMISSION FORM – STEP 4: PARENT AND LEGAL GUARDIAN PROFILING
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 21. Online Admission Form – Step 4: Parent and Legal Guardian Profiling**  
> **Figure Description:** Capture Form Card 4 showing input groups for Father's Full Name, Mother's Maiden Name, Legal Guardian details, and Emergency Contact Numbers

**Interface Controls & Elements:**

1. **Father's Full Name Fields** – Last Name, First Name, Middle Name, and Contact Number.
2. **Mother's Maiden Name Fields** – Legal maiden last name, first name, and contact details.
3. **Legal Guardian Information** – Name, relationship, and address if learner lives with guardian.
4. **Primary Emergency Phone** – Validated mobile number for urgent school communications.

---

### ONLINE ADMISSION FORM – STEP 5: SPECIAL NEEDS EDUCATION (SNED) & DISABILITY PROFILING
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 22. Online Admission Form – Step 5: Special Needs Education (SNEd) & Disability Profiling**  
> **Figure Description:** Capture Form Card 5 displaying BEEF Section 5 checkboxes for Medical Diagnoses (a1), Manifestations (a2), and PWD ID verification

**Interface Controls & Elements:**

1. **Has Disability Checkbox** – Toggles Special Needs Education profiling section.
2. **Medical Diagnosis Checkboxes (a1)** – Certified conditions (Autism, ADHD, Hearing, Visual).
3. **Observed Manifestations (a2)** – Learning or behavioral difficulties observed by parents.
4. **PWD ID Number Field** – Official government Person with Disability card number.
5. **Supporting Medical Certificate Upload** – Slot for specialist diagnostic evaluation file.

---

### ONLINE ADMISSION FORM – STEP 6: RETURNING LEARNER (BALIK-ARAL) AND TRANSFEREE HISTORY
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 23. Online Admission Form – Step 6: Returning Learner (Balik-Aral) and Transferee History**  
> **Figure Description:** Capture Form Card 6 showing Last Grade Level Completed, Last School Year Attended, and Previous School Name inputs

**Interface Controls & Elements:**

1. **Last Grade Completed** – Highest educational level completed prior to application.
2. **Last School Year Attended** – Academic term of last active enrollment.
3. **Previous School Name & ID** – Official name and DepEd ID of origin school.
4. **School Address** – Location of last attended educational institution.

---

### ONLINE ADMISSION FORM – STEP 7: LEARNING MODALITY PREFERENCES
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 24. Online Admission Form – Step 7: Learning Modality Preferences**  
> **Figure Description:** Capture Form Card 7 showing radio options for Face-to-Face Learning, Blended Learning, and Modular Instruction

**Interface Controls & Elements:**

1. **Preferred Modality Radios** – Full In-Person Face-to-Face, Blended, or Modular.
2. **Household Digital Devices** – Checkboxes for available internet and devices at home.
3. **Next to Uploads Button** – Commits preferences and advances to document upload step.

---

### DOCUMENT UPLOAD INTERFACE WITH GRADE-SPECIFIC REQUIREMENT SLOTS
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 25. Document Upload Interface with Grade-Specific Requirement Slots**  
> **Figure Description:** Capture the document upload area showing drag-and-drop slots for PSA Birth Certificate, SF9 Report Card, 1x1 Photos, and file status badges

**Interface Controls & Elements:**

1. **PSA Birth Certificate Slot** – Drag-and-drop file upload zone (JPG, PNG, or PDF).
2. **SF9 / Form 138 Card Slot** – Required upload slot for transferees showing past grades.
3. **2x2 / 1x1 ID Photo Slot** – Clear learner photo with white background.
4. **Upload Progress Bar** – Visual indicator showing file transfer completion.
5. **Remove / Replace Action** – Clears uploaded file before final submission.

---

### APPLICATION REVIEW, DATA PRIVACY AGREEMENT, AND DEPED CERTIFICATION
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 26. Application Review, Data Privacy Agreement, and DepEd Certification**  
> **Figure Description:** Capture the summary review section displaying all encoded BEEF data, certification checkbox, and the final "Submit Application" button

**Interface Controls & Elements:**

1. **Application Summary Card** – Comprehensive review of all entered learner and parent data.
2. **Truthfulness Certification** – DepEd statement certifying all submitted facts are legal and true.
3. **Data Privacy Consent** – Acceptance of RA 10173 terms for educational record processing.
4. **Submit Application Button** – Encrypts data and transmits submission to the registrar queue.

---

### APPLICATION SUBMISSION SUCCESS DIALOG WITH TRACKING CODE GENERATION
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 27. Application Submission Success Dialog with Tracking Code Generation**  
> **Figure Description:** Capture the success dialog displaying the generated Application Reference Number (e.g., APP-2026-XXXXX), QR code, and "Proceed to Dashboard" button

**Interface Controls & Elements:**

1. **Success Header Banner** – Green checkmark confirming successful submission.
2. **Tracking Reference Code** – Unique identifier (e.g., APP-2026-112937-042).
3. **Reference QR Code** – Scan code for quick mobile lookup at the school registrar gate.
4. **Proceed to Dashboard Button** – Enters applicant portal to manage appointment booking.

---

### APPLICANT DASHBOARD WITH 5-STAGE ADMISSION PROGRESS TIMELINE
**Header:** DOCUMENT SUBMISSION & APPOINTMENT SCHEDULER  
**Figure 28. Applicant Dashboard with 5-Stage Admission Progress Timeline**  
> **Figure Description:** Capture applicantDashboard.html showing the 5-stage progress pipeline (Submitted, Under Review, Appointment Booked, Verified, Officially Enrolled)

**Interface Controls & Elements:**

1. **Applicant Info Header** – Displays learner name, target grade level, and reference number.
2. **5-Stage Admission Pipeline** – Visual tracker highlighting current application milestone.
3. **Status Advisory Card** – Detailed instruction explaining next required applicant action.
4. **Navigation Tabs** – Access Application Details, Document Uploads, and Schedule Appointment.

---

### APPLICANT APPLICATION DETAILS TAB WITH BEEF DATA VIEWER
**Header:** DOCUMENT SUBMISSION & APPOINTMENT SCHEDULER  
**Figure 29. Applicant Application Details Tab with BEEF Data Viewer**  
> **Figure Description:** Capture the Application Details tab on applicantDashboard.html showing the complete read-only view of all submitted personal and demographic fields

**Interface Controls & Elements:**

1. **Demographic Information Panel** – Displays submitted name, birthdate, sex, and LRN.
2. **Address & Location Panel** – Shows registered residence in Vinzons, Camarines Norte.
3. **Parent / Guardian Roster** – Father, Mother, and Emergency contact profiles.
4. **Edit Request Notice** – Informs applicant how to request data corrections through registrar.

---

### APPLICANT DOCUMENT SUBMISSION MANAGEMENT & RE-UPLOAD INTERFACE
**Header:** DOCUMENT SUBMISSION & APPOINTMENT SCHEDULER  
**Figure 30. Applicant Document Submission Management & Re-upload Interface**  
> **Figure Description:** Capture the Documents tab showing uploaded files, verification status badges (Pending, Verified, Rejected), and "Re-upload" buttons for flagged files

**Interface Controls & Elements:**

1. **Document Item Cards** – List of all uploaded credentials and submission timestamps.
2. **Verification Badges** – Status pills (Green: Verified; Yellow: Pending; Red: Rejected).
3. **Re-Upload Button** – Enables file replacement if registrar marks an upload as blurred.
4. **Registrar Remarks Box** – Explains why a file was flagged for correction.

---

### DOCUMENT FULL-SCREEN REVIEW LIGHTBOX MODAL
**Header:** DOCUMENT SUBMISSION & APPOINTMENT SCHEDULER  
**Figure 31. Document Full-Screen Review Lightbox Modal**  
> **Figure Description:** Capture the image/PDF preview lightbox on applicantDashboard.html displaying an uploaded PSA Birth Certificate with zoom and rotate controls

**Interface Controls & Elements:**

1. **Lightbox Viewer Frame** – High-resolution display of uploaded credential document.
2. **Zoom In / Out Controls** – Adjusts image scaling to inspect text clarity.
3. **Rotate Image Button** – Reorients sideways photos for legible inspection.
4. **Close Lightbox Action** – Dismisses preview and returns to document list.

---

### DOCUMENT FILE REPLACEMENT MODAL
**Header:** DOCUMENT SUBMISSION & APPOINTMENT SCHEDULER  
**Figure 32. Document File Replacement Modal**  
> **Figure Description:** Capture the file replacement modal showing file selection input, drag-and-drop zone, and "Confirm Replacement" button

**Interface Controls & Elements:**

1. **Target Document Header** – Identifies which credential is being replaced.
2. **New File Dropzone** – Select new clear scan or photograph (max 5MB).
3. **Confirm Replacement Button** – Overwrites previous blurred file in cloud storage.
4. **Cancel Action** – Aborts replacement and keeps existing file.

---

### ON-SITE PHYSICAL DOCUMENT SUBMISSION DATE SELECTOR INTERFACE
**Header:** DOCUMENT SUBMISSION & APPOINTMENT SCHEDULER  
**Figure 33. On-Site Physical Document Submission Date Selector Interface**  
> **Figure Description:** Capture studentDashboard.html in the bookApptSection showing the Schedule Document Submission card, notification banner, date dropdown menu with remaining slots, and preferred time options

**Interface Controls & Elements:**

1. **Admission Approval Alert** – Informs applicant that application is approved for document verification.
2. **Date Selector Dropdown** – Dropdown menu showing approved appointment dates with available capacity.
3. **Session Window Radios** – Morning Session (8:00 AM – 12:00 PM) or Afternoon (1:00 PM – 5:00 PM).
4. **Physical Requirements Reminder** – Checklist of hardcopy documents required upon campus visit.
5. **Book Appointment Button** – Submits selected date and session to reserve appointment slot.

---

### APPOINTMENT SLOT BOOKING CONFIRMATION MODAL
**Header:** DOCUMENT SUBMISSION & APPOINTMENT SCHEDULER  
**Figure 34. Appointment Slot Booking Confirmation Modal**  
> **Figure Description:** Capture #apptModal displaying the confirmed appointment date, session time, applicant reference number, and "Confirm Booking" button

**Interface Controls & Elements:**

1. **Appointment Summary Card** – Highlights chosen calendar date and time session.
2. **School Address Location** – Campus venue (VPES Principal/Registrar Office, Vinzons).
3. **Confirm Booking Button** – Commits booking to database and decrements available slot capacity.
4. **Change Date Option** – Returns to date dropdown to pick another date.

---

### OFFICIAL DOCUMENT VERIFICATION APPOINTMENT SLIP WITH QR CODE
**Header:** DOCUMENT SUBMISSION & APPOINTMENT SCHEDULER  
**Figure 35. Official Document Verification Appointment Slip with QR Code**  
> **Figure Description:** Capture the printable appointment confirmation slip showing the DepEd header, applicant name, scheduled date/time, QR verification code, and print button

**Interface Controls & Elements:**

1. **Official DepEd Header** – Vinzons Pilot Elementary School official slip letterhead.
2. **Scheduled Visitor Information** – Applicant name, reference ID, and target grade level.
3. **Appointment Date & Time** – Clear highlight of reserved verification window.
4. **Security QR Code** – Gate pass scan code verified by campus security upon entry.
5. **Print Appointment Slip** – Launches browser print dialog to print or save as PDF.

---

### ENROLLED STUDENT DASHBOARD HOME AND ADVISORY SECTION CARD
**Header:** ENROLLED STUDENT & PARENT PORTAL  
**Figure 36. Enrolled Student Dashboard Home and Advisory Section Card**  
> **Figure Description:** Capture studentDashboard.html in enrolled mode showing learner name, 12-digit LRN, Grade Level, Section card with adviser name, and announcements feed

**Interface Controls & Elements:**

1. **Learner Identity Header** – Full name, 12-digit LRN, and enrolled academic year.
2. **Advisory Section Card** – Displays Grade Level, Section Name, and Class Adviser profile.
3. **Quick Status Overview** – Enrolled status, attendance summary, and released grade notices.
4. **School Bulletin Stream** – Live announcements from school administration and faculty.

---

### ENROLLED STUDENT WEEKLY INTERACTIVE TIMETABLE / CLASS SCHEDULE
**Header:** ENROLLED STUDENT & PARENT PORTAL  
**Figure 37. Enrolled Student Weekly Interactive Timetable / Class Schedule**  
> **Figure Description:** Capture the Schedule tab on studentDashboard.html showing the 5-day class schedule grid with subject cards, teacher names, and room numbers

**Interface Controls & Elements:**

1. **Weekly Calendar Grid** – Monday to Friday schedule intervals from 7:00 AM to 5:00 PM.
2. **Scheduled Subject Cards** – Color-coded class blocks showing Subject, Time, and Room.
3. **Teacher Designation** – Displays assigned subject teacher for each learning area.
4. **Print Timetable Button** – Generates clean printable PDF of class schedule.

---

### ENROLLED STUDENT QUARTERLY ACADEMIC GRADES DISPLAY
**Header:** ENROLLED STUDENT & PARENT PORTAL  
**Figure 38. Enrolled Student Quarterly Academic Grades Display**  
> **Figure Description:** Capture the Grades tab on studentDashboard.html displaying the DepEd SF9 report card table with Q1–Q4 ratings, final rating, and remarks

**Interface Controls & Elements:**

1. **SF9 Report Card Matrix** – Learning areas list with Quarter 1, 2, 3, and 4 columns.
2. **Final Rating & Remarks** – Weighted final mark and automated Passed/Failed indicator.
3. **General Academic Average** – Prominent card showing learner overall general average.
4. **Download Report Card (PDF)** – Exports official printable DepEd SF9 report card.

---

### ENROLLED STUDENT MAPEH COMPOSITE GRADE AND COMPONENT BREAKDOWN DRAWER
**Header:** ENROLLED STUDENT & PARENT PORTAL  
**Figure 39. Enrolled Student MAPEH Composite Grade and Component Breakdown Drawer**  
> **Figure Description:** Capture the MAPEH detail drawer showing the sub-component ratings for Music, Arts, Physical Education, and Health contributing to the composite grade

**Interface Controls & Elements:**

1. **MAPEH Composite Summary** – Overall quarterly score computed from the four components.
2. **Music Component Mark** – Encoded grade for Music learning competencies.
3. **Arts Component Mark** – Encoded grade for Visual and Creative Arts.
4. **Physical Education Mark** – Encoded grade for Physical fitness and sports.
5. **Health Component Mark** – Encoded grade for Health and nutrition competencies.

---

### ENROLLED STUDENT HISTORICAL SCHOOL YEAR GRADE ARCHIVE BROWSER
**Header:** ENROLLED STUDENT & PARENT PORTAL  
**Figure 40. Enrolled Student Historical School Year Grade Archive Browser**  
> **Figure Description:** Capture the school year archive selector on the grades tab showing past academic years and historical grades

**Interface Controls & Elements:**

1. **School Year Archive Dropdown** – Select past completed academic school years.
2. **Historical Grade Table** – Read-only display of finalized grades from previous grade levels.
3. **Promotion Record** – Confirms historical promotion status for past terms.

---

### ENROLLED STUDENT MASTER PROFILE VIEW
**Header:** ENROLLED STUDENT & PARENT PORTAL  
**Figure 41. Enrolled Student Master Profile View**  
> **Figure Description:** Capture the Profile tab on studentDashboard.html showing personal details, address, parent contacts, and password security management

**Interface Controls & Elements:**

1. **Demographic Data Card** – Official birthdate, sex, PSA registry number, and 12-digit LRN.
2. **Residential Address Card** – Full home address in Vinzons, Camarines Norte.
3. **Guardian Contacts** – Father, Mother, Guardian names and registered phone numbers.
4. **Change Password Form** – Update account security password.

---

### CONTINUING STUDENT RE-ENROLLMENT CONFIRMATION TAB
**Header:** ENROLLED STUDENT & PARENT PORTAL  
**Figure 42. Continuing Student Re-Enrollment Confirmation Tab**  
> **Figure Description:** Capture the Re-Enrollment tab on studentDashboard.html showing incoming school year, target grade level, contact update fields, and "Submit Re-Enrollment" button

**Interface Controls & Elements:**

1. **Re-Enrollment Gating Banner** – Shows whether continuation filing is active.
2. **Next Grade Level Indicator** – Target grade level based on promotion status.
3. **Contact Information Verification** – Update residential address and mobile phone.
4. **Submit Re-Enrollment Button** – Submits continuation record to registrar without paper forms.

---

### ALUMNI / GRADUATED STUDENT INTERFACE AND PERMANENT RECORD ACCESS
**Header:** ENROLLED STUDENT & PARENT PORTAL  
**Figure 43. Alumni / Graduated Student Interface and Permanent Record Access**  
> **Figure Description:** Capture the alumni view on studentDashboard.html for a graduated Grade 6 learner showing completion badge and SF10 transcript access

**Interface Controls & Elements:**

1. **Elementary Graduate Badge** – Identifies completion of elementary basic education.
2. **Graduation School Year** – Official year and date of graduation.
3. **Permanent Record Request** – Option to request official certified SF10 (Form 137) transcript.
4. **Historical Academic Portfolio** – View finalized elementary scholastic records.

---

### TEACHER DASHBOARD OVERVIEW, ADVISORY CLASS SUMMARY, AND TEACHING LOADS
**Header:** TEACHER & FACULTY PORTAL  
**Figure 44. Teacher Dashboard Overview, Advisory Class Summary, and Teaching Loads**  
> **Figure Description:** Capture teacherDashboard.html showing teacher welcome card, handled advisory section, total teaching load statistics, and fast action links

**Interface Controls & Elements:**

1. **Teacher Profile Summary** – Photo, full name, employee number, and specialization.
2. **Advisory Class Card** – Assigned homeroom section, room location, and enrolled headcount.
3. **Teaching Load Quick-Cards** – Handled subjects, weekly teaching minutes, and grading progress.
4. **Grade Encoding Shortcut** – Fast navigation to quarterly grading sheet.

---

### TEACHER RIGHT-SIDEBAR INTERACTIVE CALENDAR AND TODAY'S CLASS SCHEDULE DRAWER
**Header:** TEACHER & FACULTY PORTAL  
**Figure 45. Teacher Right-Sidebar Interactive Calendar and Today's Class Schedule Drawer**  
> **Figure Description:** Capture the right sidebar on teacherDashboard.html showing the mini calendar, current day's classes, and active class countdown

**Interface Controls & Elements:**

1. **Mini Month Calendar** – Date selector highlighting current date and scheduled events.
2. **Today's Schedule Timeline** – Chronological listing of class periods for the current day.
3. **Active Class Indicator** – Highlights ongoing class period with time remaining.
4. **Section Room Tag** – Room location for upcoming scheduled classes.

---

### TEACHER ADVISORY STUDENT ROSTER DIRECTORY
**Header:** TEACHER & FACULTY PORTAL  
**Figure 46. Teacher Advisory Student Roster Directory**  
> **Figure Description:** Capture the Advisory Class tab on teacherDashboard.html showing the pupil directory split into Male and Female sections with LRNs and guardian contacts

**Interface Controls & Elements:**

1. **Section Roster Header** – Grade level, section name, and gender distribution summary.
2. **Male Learners Directory** – Alphabetical listing of male pupils with 12-digit LRNs.
3. **Female Learners Directory** – Alphabetical listing of female pupils in standard DepEd format.
4. **Guardian Emergency Contacts** – Direct phone numbers for homeroom communication.
5. **Learner Academic Profile** – Inspect individual pupil attendance and report cards.

---

### TEACHER STUDENT PROFILE INSPECTION MODAL
**Header:** TEACHER & FACULTY PORTAL  
**Figure 47. Teacher Student Profile Inspection Modal**  
> **Figure Description:** Capture the student detail modal launched from the advisory roster showing student photo, demographic details, birthdate, and contact history

**Interface Controls & Elements:**

1. **Learner Identification** – Full name, 12-digit LRN, birthdate, and age.
2. **Complete Residential Address** – Registered home location.
3. **Parent / Guardian Information** – Father, mother, and authorized guardian details.
4. **Close Profile Button** – Dismisses inspection modal.

---

### TEACHER QUARTERLY GRADING SHEET SPREADSHEET GRID
**Header:** TEACHER & FACULTY PORTAL  
**Figure 48. Teacher Quarterly Grading Sheet Spreadsheet Grid**  
> **Figure Description:** Capture teacherGrades.html showing the Section, Subject, and Quarter selectors, along with the numerical grade input cells, color-coding, and Save button

**Interface Controls & Elements:**

1. **Section & Subject Selectors** – Choose class section and elementary subject to grade.
2. **Quarter Tabs** – Switch between 1st, 2nd, 3rd, and 4th Quarter grading sheets.
3. **Numerical Grade Cells** – Inputs restricted to valid 60–100 DepEd grading scale.
4. **Automated General Average** – Instant computation of quarterly average across pupils.
5. **Remarks Indicator** – Automated Passed (>=75) or Failed (<75) badge.
6. **Save Grades Button** – Commits encoded grades to database.

---

### TEACHER MAPEH COMPONENT BREAKDOWN AND SUB-GRADING MODAL
**Header:** TEACHER & FACULTY PORTAL  
**Figure 49. Teacher MAPEH Component Breakdown and Sub-Grading Modal**  
> **Figure Description:** Capture the MAPEH sub-grading modal showing separate grade inputs for Music, Arts, PE, and Health with real-time average calculation

**Interface Controls & Elements:**

1. **Music Grade Input** – Input quarterly score for Music competencies.
2. **Arts Grade Input** – Input quarterly score for Visual and Creative Arts.
3. **PE Grade Input** – Input quarterly score for Physical Education.
4. **Health Grade Input** – Input quarterly score for Health and Hygiene competencies.
5. **Real-Time MAPEH Average** – Auto-computed composite rating transferred to main grading sheet.

---

### TEACHER INDIVIDUAL WEEKLY TEACHING SCHEDULE AND PRINT LAYOUT
**Header:** TEACHER & FACULTY PORTAL  
**Figure 50. Teacher Individual Weekly Teaching Schedule and Print Layout**  
> **Figure Description:** Capture the teacher timetable view on teacherDashboard.html showing weekly schedule blocks and the "Print Schedule" button

**Interface Controls & Elements:**

1. **Weekly Timetable Grid** – 5-day calendar grid (Monday to Friday) showing teaching load.
2. **Subject Blocks** – Color-coded class sessions with grade, section, and room.
3. **Teaching Minutes Summary** – Total weekly instructional minutes vs. standard teaching load.
4. **Print Schedule Button** – Formats schedule for printable display in homeroom.

---

### TEACHER DEPED SCHOOL FORMS HUB (SF1 TO SF8 GENERATION CARDS)
**Header:** TEACHER & FACULTY PORTAL  
**Figure 51. Teacher DepEd School Forms Hub (SF1 to SF8 Generation Cards)**  
> **Figure Description:** Capture the School Forms tab on teacherDashboard.html displaying cards for generating SF1 (Register), SF2 (Attendance), SF5 (Promotion), and SF9 (Card)

**Interface Controls & Elements:**

1. **SF1: School Register Card** – Generate official class register in Excel or PDF format.
2. **SF2: Daily Attendance Card** – Generate monthly learner attendance report.
3. **SF5: Report on Promotion Card** – Generate end-of-year promotion and proficiency matrix.
4. **SF9: Progress Report Card Hub** – Access batch report card generator.
5. **Generate Form Button** – Triggers backend compilation of target DepEd document.

---

### TEACHER SF2 DAILY ATTENDANCE MONTH AND YEAR SELECTION MODAL
**Header:** TEACHER & FACULTY PORTAL  
**Figure 52. Teacher SF2 Daily Attendance Month and Year Selection Modal**  
> **Figure Description:** Capture the SF2 configuration dialog showing Month dropdown, School Year selector, and "Generate SF2 Report" button

**Interface Controls & Elements:**

1. **School Year Selector** – Select active academic school year.
2. **Reporting Month Dropdown** – Choose calendar month (June to March) for attendance calculation.
3. **Generate SF2 Button** – Compiles daily attendance and computes monthly average attendance.
4. **Export Format Selector** – Choose between Excel (.xlsx) and printable PDF formats.

---

### TEACHER SF9 PROGRESS REPORT CARD WORKSPACE & BATCH ZIP DOWNLOAD INTERFACE
**Header:** TEACHER & FACULTY PORTAL  
**Figure 53. Teacher SF9 Progress Report Card Workspace & Batch ZIP Download Interface**  
> **Figure Description:** Capture the SF9 workspace showing student list with "Preview Card" buttons and the "Download All (ZIP)" batch export button

**Interface Controls & Elements:**

1. **Section Pupil List** – Roster of learners with finalized quarterly marks.
2. **Preview Card Button** – Opens individual official DepEd SF9 report card PDF.
3. **Download All (ZIP) Button** – Packages all section report cards into a single ZIP file.
4. **Grading Completeness Bar** – Confirms 100% of subject grades are encoded before batch export.

---

### TEACHER ACCOUNT PROFILE AND PASSWORD SETTINGS
**Header:** TEACHER & FACULTY PORTAL  
**Figure 54. Teacher Account Profile and Password Settings**  
> **Figure Description:** Capture the teacher profile settings tab showing employee details, contact info, and password update form

**Interface Controls & Elements:**

1. **Employee Identification** – Read-only display of DepEd Employee ID and cluster assignment.
2. **Contact Information** – Update personal email and active mobile phone number.
3. **Password Update Fields** – Replace temporary password with secure new password.
4. **Save Changes Button** – Commits updated profile credentials to database.

---

### ADMINISTRATOR EXECUTIVE DASHBOARD WITH REAL-TIME KPIS AND DAILY APPOINTMENT STREAM
**Header:** ADMINISTRATOR DASHBOARD & KPI ANALYTICS  
**Figure 55. Administrator Executive Dashboard with Real-Time KPIs and Daily Appointment Stream**  
> **Figure Description:** Capture adminDashboard.html showing the executive KPI cards, enrollment metrics, and the admissions queue stream

**Interface Controls & Elements:**

1. **Executive KPI Cards Header** – Real-time metrics for Total Applications, Appointments, and Enrolled.
2. **Today's Appointments Progress** – Daily document verification queue with completion progress meter.
3. **Officially Enrolled Headcount** – Total learners active in sections vs. school capacity.
4. **Recent Activity Audit Stream** – Real-time chronological log of administrative events.
5. **Quick Actions Panel** – Direct shortcuts to evaluate applications or print school forms.

---

### ADMINISTRATOR INTERACTIVE ANALYTICS GRAPH (BAR GRAPH / LINE TREND TOGGLE)
**Header:** ADMINISTRATOR DASHBOARD & KPI ANALYTICS  
**Figure 56. Administrator Interactive Analytics Graph (Bar Graph / Line Trend Toggle)**  
> **Figure Description:** Capture the analytics panel on adminDashboard.html showing the enrollment chart with toggles for Bar Graph vs. Line Trend view

**Interface Controls & Elements:**

1. **Enrollment Distribution Graph** – Visual headcount representation across Kindergarten to Grade 6.
2. **Chart Type Toggle** – Switch between Bar Graph and Line Trend views.
3. **Gender Demographic Breakdown** – Male vs. Female enrollment ratio per grade level.
4. **Export Analytics Button** – Download chart graphic for institutional presentations.

---

### ADMINISTRATOR CLASS SECTIONS & CAPACITY PANEL WITH UNASSIGNED STUDENTS ALERT
**Header:** ADMINISTRATOR DASHBOARD & KPI ANALYTICS  
**Figure 57. Administrator Class Sections & Capacity Panel with Unassigned Students Alert**  
> **Figure Description:** Capture the section capacity monitor on adminDashboard.html showing capacity bars per section and the unassigned students warning badge

**Interface Controls & Elements:**

1. **Section Capacity Meters** – Visual progress bars showing pupil headcount per class section.
2. **Unassigned Students Alert Badge** – Red counter indicating pupils awaiting section assignment.
3. **Over-Capacity Warning** – Highlights sections approaching DepEd maximum of 45 pupils.
4. **Assign Sections Shortcut** – One-click navigation to the drag-and-drop sectioning workspace.

---

### ADMINISTRATOR OPERATIONS HUB WITH PRIORITY ACTIONS AND LIVE AUDIT STREAM
**Header:** ADMINISTRATOR DASHBOARD & KPI ANALYTICS  
**Figure 58. Administrator Operations Hub with Priority Actions and Live Audit Stream**  
> **Figure Description:** Capture the operations hub section on adminDashboard.html showing pending document tasks, system alerts, and quick actions

**Interface Controls & Elements:**

1. **Priority Task Checklist** – Pending applications and document verifications requiring action.
2. **Live Activity Stream** – Real-time ticker of user logins, enrollment filings, and grade submissions.
3. **System Status Indicator** – Confirms database connectivity, cloud storage, and mailer health.

---

### ADMINISTRATOR APPLICATIONS MANAGEMENT HUB – NEW APPLICATIONS TAB
**Header:** APPLICATIONS & ENROLLMENT MANAGEMENT  
**Figure 59. Administrator Applications Management Hub – New Applications Tab**  
> **Figure Description:** Capture applications.html under the "New Applications" tab showing status filter pills, search input, application rows, and "Review" buttons

**Interface Controls & Elements:**

1. **Status Filter Tabs** – Quick-filtering: Pending Review, Approved, Enrolled, Rejected.
2. **Universal Search Box** – Lookup by student name, tracking reference number, or LRN.
3. **Grade Level Filter** – Filter intake records by target grade level (Kindergarten to Grade 6).
4. **Applications Data Table** – Renders applicant name, grade, date filed, and current status.
5. **Review Action Button** – Opens comprehensive applicant dossier modal.

---

### ADMINISTRATOR COMPREHENSIVE APPLICATION DOSSIER EVALUATION MODAL
**Header:** APPLICATIONS & ENROLLMENT MANAGEMENT  
**Figure 60. Administrator Comprehensive Application Dossier Evaluation Modal**  
> **Figure Description:** Capture the application review modal on applications.html showing student details, uploaded document previews, and Approve / Reject / Return action buttons

**Interface Controls & Elements:**

1. **Applicant Demographic Folder** – Full view of submitted BEEF personal and address fields.
2. **Document Verification Drawer** – Inspect uploaded birth certificates and previous report cards.
3. **Approve Application Action** – Advances application to approved status for physical document intake.
4. **Return for Correction Action** – Flags deficiencies and notifies applicant via email.
5. **Reject Application Action** – Formally rejects invalid or duplicate applications.

---

### ADMINISTRATOR CONTINUING STUDENT RE-ENROLLMENT PROCESSING QUEUE
**Header:** APPLICATIONS & ENROLLMENT MANAGEMENT  
**Figure 61. Administrator Continuing Student Re-Enrollment Processing Queue**  
> **Figure Description:** Capture the Re-Enrollment tab on applications.html showing continuing student re-admission requests, academic clearance, and bulk approval controls

**Interface Controls & Elements:**

1. **Re-Enrollment Intake Queue** – Roster of continuing learners filing for the upcoming school year.
2. **Academic Promotion Clearance** – Confirms learner passed previous grade level before clearance.
3. **Bulk Approve Re-Enrollments** – Check multiple pupils to approve continuations in batch.
4. **Assign Section Action** – Directly places approved re-enrollees into target grade sections.

---

### ADMINISTRATOR STUDENT YEAR-END PROMOTION AND GRADE 6 GRADUATION WORKSPACE
**Header:** APPLICATIONS & ENROLLMENT MANAGEMENT  
**Figure 62. Administrator Student Year-End Promotion and Grade 6 Graduation Workspace**  
> **Figure Description:** Capture the promotion/graduation workspace showing Grade 6 completers, honors recognition, and graduation status confirmation controls

**Interface Controls & Elements:**

1. **Grade 6 Completers Directory** – Roster of graduating learners with general averages.
2. **Honors & Academic Awards** – Identifies With Honors, With High Honors, and With Highest Honors.
3. **Confirm Graduation Action** – Marks student records as officially Graduated Alumni.
4. **Export Graduation List** – Downloads ceremonial graduation roster for DepEd division office.

---

### ADMINISTRATOR MASTER DOCUMENT REPOSITORY IN TABLE VIEW AND DOSSIER VIEW
**Header:** DOCUMENT VERIFICATION REPOSITORY  
**Figure 63. Administrator Master Document Repository in Table View and Dossier View**  
> **Figure Description:** Capture documents.html showing the Table View / Dossier View toggle, document status filters, and the master verification queue

**Interface Controls & Elements:**

1. **View Mode Toggle** – Switch between tabular spreadsheet view and visual student dossier view.
2. **Document Category Filter** – Filter by PSA Birth Certificate, SF9 Report Card, or SNEd Medical File.
3. **Verification Status Pills** – Filter by Pending Verification, Verified, or Flagged for Re-upload.
4. **Document Record Rows** – Shows applicant name, document type, submission date, and verification action.

---

### ADMINISTRATOR ENHANCED DOCUMENT PREVIEW AND VERIFICATION LIGHTBOX
**Header:** DOCUMENT VERIFICATION REPOSITORY  
**Figure 64. Administrator Enhanced Document Preview and Verification Lightbox**  
> **Figure Description:** Capture the document verification lightbox modal on documents.html displaying an uploaded credential with Verify, Reject, and Request Re-upload controls

**Interface Controls & Elements:**

1. **High-Resolution Document Canvas** – Zoomable viewer for inspecting official seals and stamps.
2. **Mark as Verified Button** – Approves document and logs administrator ID and timestamp.
3. **Flag as Blurred / Invalid** – Opens feedback box to prompt parent for re-upload.
4. **Next / Previous Navigation** – Quickly advance across documents in queue.

---

### ADMINISTRATOR DOCUMENT VERIFICATION SLOT MANAGEMENT AND ATTENDEE ROSTER
**Header:** APPOINTMENT SLOTS MANAGEMENT  
**Figure 65. Administrator Document Verification Slot Management and Attendee Roster**  
> **Figure Description:** Capture documentSlots.html showing the calendar month selector, slot capacity indicators, and the roster of booked applicants per date

**Interface Controls & Elements:**

1. **School Year & Month Dropdown** – Set active term and month for on-site document intake.
2. **Date Slot Cards** – Displays scheduled dates with booked count vs. maximum capacity.
3. **Attendee Roster Drawer** – Inspect names, reference codes, and time windows for scheduled applicants.
4. **Mark as Attended Action** – Checks in applicant upon physical document arrival at campus.
5. **Add Date Slots Button** – Opens slot creation modal.

---

### ADMINISTRATOR BULK SLOT GENERATION MODAL
**Header:** APPOINTMENT SLOTS MANAGEMENT  
**Figure 66. Administrator Bulk Slot Generation Modal**  
> **Figure Description:** Capture the bulk slot generator modal on documentSlots.html showing date range picker, daily capacity inputs (AM/PM), and exclude weekends checkbox

**Interface Controls & Elements:**

1. **Date Range Pickers** – Define intake period start date and end date.
2. **Exclude Weekends Checkbox** – Automatically skips Saturdays and Sundays.
3. **Morning (AM) Capacity** – Maximum appointments per morning session (8:00 AM – 12:00 PM).
4. **Afternoon (PM) Capacity** – Maximum appointments per afternoon session (1:00 PM – 5:00 PM).
5. **Generate Slots Button** – Creates appointment slots across the calendar in bulk.

---

### ADMINISTRATOR MASTER STUDENT DATABASE AND FILTERING CONTROLS
**Header:** STUDENT MASTER DATABASE & LRN UPDATE  
**Figure 67. Administrator Master Student Database and Filtering Controls**  
> **Figure Description:** Capture students.html showing grade level tabs, universal search, the student master table, and row action menus

**Interface Controls & Elements:**

1. **Grade Level Filter Tabs** – Filter directory by Kindergarten, Grades 1 to 6, or All Learners.
2. **Universal Search Input** – Search by 12-digit LRN, student full name, or assigned section.
3. **Master Student Table** – Columns for Name, LRN, Sex, Grade, Section, and Enrollment Status.
4. **View Complete Profile** – Opens learner cumulative folder.
5. **Update LRN Action** – Launches DepEd LRN assignment modal (#updateLrnModal).
6. **Unlink Account Action** – Opens safety-locked guardian detachment dialog (#unlinkModal).

---

### ADMINISTRATOR SECTION ASSIGNMENT AND DRAG-AND-DROP MANAGEMENT INTERFACE
**Header:** CLASS SECTION & ADVISER MANAGEMENT  
**Figure 68. Administrator Section Assignment and Drag-and-Drop Management Interface**  
> **Figure Description:** Capture sections.html under the "Assign Students to Sections" tab showing the Unassigned Students pool on the left (with Male/Female columns, search input, and checkboxes) and Section dropzones on the right with capacity indicators and remove (×) buttons

**Interface Controls & Elements:**

1. **Target Section Dropdown** – Select target section receiving student placements.
2. **Publication Status Ribbon** – Indicates whether assignments are in DRAFT mode or PUBLISHED.
3. **Unassigned Pupils Pool (Left)** – Unallocated students separated into Male and Female columns.
4. **Section Roster Panel (Right)** – Enrolled pupils in selected section with live gender ratios.
5. **Drag-and-Drop & Bulk Assign** – Drag cards across panels or select checkboxes for bulk assignment.
6. **Unassign Action (×)** – Safely returns assigned pupil to the unassigned queue.
7. **Publish Assignments Button** – Commits assignments to official DepEd enrollment records.

---

### ADMINISTRATOR LRN UPDATE AND ACCOUNT UNLINKING MODALS
**Header:** STUDENT MASTER DATABASE & LRN UPDATE  
**Figure 69. Administrator LRN Update and Account Unlinking Modals**  
> **Figure Description:** Capture the side-by-side or composite view of #updateLrnModal (showing the 12-digit input and validation) and #unlinkModal (showing the 5-second countdown timer button)

**Interface Controls & Elements:**

1. **DepEd 12-Digit LRN Input** – Strict 12-digit numeric input with DepEd format validation.
2. **Validation Indicator** – Turns green when exactly 12 valid digits are entered.
3. **Save LRN Button** – Permanently commits official LRN to student record.
4. **Guardian Unlink Info** – Displays currently linked parent user account.
5. **5-Second Countdown Timer** – Disables confirm button for 5 seconds to prevent accidental clicks.
6. **Confirm Unlink Button** – Detaches user account from student record after countdown.

---

### ADMINISTRATOR SECTION MANAGEMENT AND CLASS ADVISER ASSIGNMENT INTERFACE
**Header:** CLASS SECTION & ADVISER MANAGEMENT  
**Figure 70. Administrator Section Management and Class Adviser Assignment Interface**  
> **Figure Description:** Capture sections.html under the "Manage Sections" tab showing section cards, room assignments, adviser dropdowns, and the "Add New Section" modal

**Interface Controls & Elements:**

1. **Create New Section Button** – Opens modal to define Section Name, Grade Level, and Room Number.
2. **Section Information Cards** – Displays Grade & Section, Room Location, and Maximum Capacity.
3. **Class Adviser Dropdown** – Assigns official homeroom faculty adviser.
4. **Capacity Utilization Bar** – Color-coded progress meter indicating pupil occupancy.
5. **Edit / Archive Section Action** – Modify section details or deactivate section.

---

### ADMINISTRATOR DEPED ELEMENTARY SUBJECT CURRICULUM MANAGEMENT
**Header:** CURRICULUM & SUBJECT MANAGEMENT  
**Figure 71. Administrator DepEd Elementary Subject Curriculum Management**  
> **Figure Description:** Capture subjectManagement.html displaying active curriculum subjects vs. archived subjects tabs, grade level filter, subject cards with units, and #subjectModal

**Interface Controls & Elements:**

1. **Curriculum View Tabs** – Toggle between Active Curriculum Subjects and Archived Subjects.
2. **Grade Level Filter Bar** – Filter learning areas by elementary grade level.
3. **Add Subject Button** – Opens #subjectModal to register a DepEd curriculum subject.
4. **Subject Form Fields** – Input Subject Name, Subject Code, Grade Level, and Units.
5. **Archive Subject Action** – Deactivates subject without deleting historical grade records.
6. **Restore Subject Action** – Re-enables archived subject back to active curriculum.

---

### ADMINISTRATOR FACULTY AND TEACHER MANAGEMENT DIRECTORY WITH CLUSTER FILTERS
**Header:** FACULTY & TEACHER DIRECTORY  
**Figure 72. Administrator Faculty and Teacher Management Directory with Cluster Filters**  
> **Figure Description:** Capture teacherManagement.html showing faculty cluster filter pills (All, Kindergarten, Primary, Intermediate), teacher profile cards, and #addTeacherModal

**Interface Controls & Elements:**

1. **Faculty Cluster Filter Pills** – Filter by All Faculty, Kindergarten, Primary, or Intermediate.
2. **Add Teacher Button** – Launches modal to register an existing user account as faculty.
3. **Teacher Account Dropdown** – Select authenticated user account (#teacherAccount).
4. **Cluster & Specialization Inputs** – Configure handled grade cluster and subject specialization.
5. **Faculty Profile Cards** – Displays teacher avatar, employee ID, specialization, and advisory section.
6. **View Timetable Action** – Opens large teacher timetable modal (#largeTeacherTimetableModal).

---

### ADMINISTRATOR FACULTY MASTER TIMETABLE INSPECTION MODAL
**Header:** FACULTY & TEACHER DIRECTORY  
**Figure 73. Administrator Faculty Master Timetable Inspection Modal**  
> **Figure Description:** Capture #largeTeacherTimetableModal on teacherManagement.html showing the teacher's full weekly 5-day schedule grid and the Print button

**Interface Controls & Elements:**

1. **Faculty Identification Header** – Displays teacher name, employee ID, and total weekly minutes.
2. **Weekly Schedule Grid** – Monday to Friday calendar grid with scheduled subject periods.
3. **Class Period Blocks** – Color-coded subject blocks displaying section and room.
4. **Advisory Homeroom Period** – Highlights periods where teacher acts as class adviser.
5. **Print Schedule Action** – Generates official individual SF7 teaching program PDF.

---

### ADMINISTRATOR TIMETABLE BUILDER – MASTER CLASS SCHEDULES OVERVIEW
**Header:** CLASS SCHEDULES & TIMETABLE BUILDER  
**Figure 74. Administrator Timetable Builder – Master Class Schedules Overview**  
> **Figure Description:** Capture scheduleManagement.html under the "Master Class Schedules" tab showing Schedule Publication Status Banner, Grade Level filters, section search input, and Section Schedule Cards grid

**Interface Controls & Elements:**

1. **Master Schedules Tab** – Overview of complete weekly timetables across all grade sections.
2. **Publication Status Toggle** – Publish schedules school-wide or keep in draft mode.
3. **Grade Level & Search Filter** – Filter schedule cards by grade or section name.
4. **Section Schedule Cards** – Displays weekly subject distribution and total minutes.
5. **Switch to Schedule Builder** – Transitions to interactive schedule editor.

---

### ADMINISTRATOR TIMETABLE SESSION CREATOR WITH AUTOMATED CONFLICT DETECTION ENGINE
**Header:** CLASS SCHEDULES & TIMETABLE BUILDER  
**Figure 75. Administrator Timetable Session Creator with Automated Conflict Detection Engine**  
> **Figure Description:** Capture scheduleManagement.html under the "Class Schedule Builder" tab showing Left Panel session creator form, Right Panel weekly grid, and the Collision Warning Modal

**Interface Controls & Elements:**

1. **Target Section Selector** – Choose class section being scheduled.
2. **Subject & Teacher Dropdowns** – Select curriculum subject and qualified faculty member.
3. **Start Time & Duration** – Time picker and duration in minutes (e.g., 50 min).
4. **Day of Week Checkboxes** – Select days (Monday, Tuesday, Wednesday, Thursday, Friday).
5. **Automated Conflict Detector** – Real-time engine that detects overlapping teacher or section hours.
6. **Collision Warning Alert** – Red modal blocking entry if a scheduling overlap occurs.
7. **Auto-Fill & Auto-Assign Tools** – Automatically populate gaps based on curriculum standards.

---

### ADMINISTRATOR USER ACCOUNT MANAGEMENT AND STAFF CREATION MODAL
**Header:** USER MANAGEMENT & SECURITY ROLES  
**Figure 76. Administrator User Account Management and Staff Creation Modal**  
> **Figure Description:** Capture users.html showing role filter pills (All, Admin, Teacher, Student/Parent), user search box, user accounts table with status toggles, and #addUserModal

**Interface Controls & Elements:**

1. **Role Filter Pills** – Filter directory by Admin, Teacher, Student/Parent, or All Accounts.
2. **User Search Bar** – Search by display name, email address, or user ID.
3. **User Directory Table** – Displays avatar, name, email, role, creation date, and status.
4. **Add User Button** – Opens modal to provision a staff or teacher account.
5. **Account Status Toggle** – Activate or suspend user login credentials instantly.
6. **Reset Password Action** – Dispatches password reset email to user.

---

### ADMINISTRATOR USER ROLE MODIFICATION DIALOG WITH DEMOTION SAFEGUARDS
**Header:** USER MANAGEMENT & SECURITY ROLES  
**Figure 77. Administrator User Role Modification Dialog with Demotion Safeguards**  
> **Figure Description:** Capture the role modification dialog on users.html showing the role selector dropdown, permissions preview, and the confirmation button with admin safeguards

**Interface Controls & Elements:**

1. **Target User Profile** – Displays user name and currently assigned system role.
2. **Role Assignment Dropdown** – Select new role (Administrator, Teacher, or Student/Parent).
3. **Demotion Safeguard Check** – Prevents demoting the last remaining active administrator.
4. **Save Role Changes Button** – Commits new role permissions and updates session tokens.

---

### ADMINISTRATOR ANNOUNCEMENTS MANAGEMENT HUB AND CATEGORY TAGGING
**Header:** ANNOUNCEMENTS & FACEBOOK SYNC  
**Figure 78. Administrator Announcements Management Hub and Category Tagging**  
> **Figure Description:** Capture announcements.html showing published announcements list, priority pinned items, and the Create Announcement modal active with Title, Category, Audience, and Content editor

**Interface Controls & Elements:**

1. **Create Announcement Button** – Opens modal to draft a new school bulletin.
2. **Title & Category Selectors** – Enter headline and category (Advisory, Suspension, DepEd Memo).
3. **Target Audience Selector** – Choose Public, Enrolled Students & Parents, or Faculty Only.
4. **Priority Pinning Toggle** – Pins urgent advisory to top of public feed with a red badge.
5. **Auto-Post to Facebook Toggle** – Synchronizes announcement to official VPES Facebook Page.
6. **Publish Announcement Action** – Immediately broadcasts advisory across portal channels.

---

### ADMINISTRATOR FACEBOOK SYNCED POST REVIEW AND APPROVAL TWO-COLUMN LIGHTBOX
**Header:** ANNOUNCEMENTS & FACEBOOK SYNC  
**Figure 79. Administrator Facebook Synced Post Review and Approval Two-Column Lightbox**  
> **Figure Description:** Capture reviewModal on announcements.html displaying the Facebook post content on the left and portal formatting controls on the right

**Interface Controls & Elements:**

1. **Pending Review Tab** – Queue of incoming Facebook Page posts captured via webhook.
2. **Facebook Source Panel (Left)** – Displays raw post content, original date, and attached photos.
3. **Portal Configuration Panel (Right)** – Customize title, portal category, and formatting.
4. **Approve & Publish Button** – Approves post and publishes it directly to portal landing page.
5. **Dismiss / Reject Post** – Removes post from queue without publishing.

---

### ADMINISTRATOR SYSTEM AUDIT AND ACTIVITY LOGS INTERFACE
**Header:** SYSTEM AUDIT & SECURITY LOGS  
**Figure 80. Administrator System Audit and Activity Logs Interface**  
> **Figure Description:** Capture auditLogs.html showing KPI stat cards, category filter pills, search input, audit trail table, and the Audit Event Detail modal (#auditDetailModal)

**Interface Controls & Elements:**

1. **KPI Stat Summary Cards** – Displays Total Logs, Actions Today, Re-Enrollments, Admissions, Security.
2. **Universal Search Box** – Real-time search by student name, LRN, performer, or description.
3. **Category Filter Pills** – Filter by All, Re-Enrollment, Admissions, Documents, Users, Sections, Settings.
4. **Date Range Filter Dropdown** – Preset ranges (All Time, Today, Yesterday, Last 7/30 Days, Custom).
5. **Audit Trail Table** – Columns for Date & Time, Event Action, Description & Details, Performed By.
6. **Audit Event Detail Modal** – Click row to inspect action code, performer email, and application ref.
7. **Live Refresh Button** – Refreshes audit event stream without page reload.

---

### ADMINISTRATOR SCHOOL YEAR MANAGEMENT AND ACTIVATION READINESS AUDIT MODAL
**Header:** SYSTEM SETTINGS & ADMISSION GATING  
**Figure 81. Administrator School Year Management and Activation Readiness Audit Modal**  
> **Figure Description:** Capture the School Year tab on settings.html showing active SY, historical SY table, and the Activation Readiness Audit dialog with verification checklist

**Interface Controls & Elements:**

1. **Active School Year Banner** – Identifies currently active DepEd term (e.g., S.Y. 2026–2027).
2. **Add School Year Button** – Opens dialog to create new school year with start and end dates.
3. **Historical School Years Table** – Archive of past academic terms and enrollment totals.
4. **Check Activation Readiness Button** – Performs automated audit of 4th-quarter grades and promotions.
5. **Readiness Checklist Modal** – Itemizes missing grades; enables "Activate School Year" once resolved.

---

### ADMINISTRATOR INDEPENDENT ADMISSION GATING SWITCHES (EARLY REG, ENROLLMENT, RE-ENROLLMENT)
**Header:** SYSTEM SETTINGS & ADMISSION GATING  
**Figure 82. Administrator Independent Admission Gating Switches (Early Reg, Enrollment, Re-Enrollment)**  
> **Figure Description:** Capture the three independent gating cards on settings.html with toggle switches and calendar date pickers

**Interface Controls & Elements:**

1. **Early Registration Switch** – Toggles pre-registration ON/OFF for Kindergarten and Grade 1.
2. **Official General Enrollment Switch** – Toggles general admission ON/OFF for all grade levels.
3. **Re-Enrollment Gating Switch** – Controls whether re-enrollment tab is active on student dashboard.
4. **Scheduled Calendar Date Pickers** – Sets automated opening and closing dates for admission forms.
5. **Closed Advisory Textbox** – Customizes public advisory notice displayed when enrollment is closed.

---

### ADMINISTRATOR SCHOOL INSTITUTIONAL PROFILE AND DEPED IDENTIFIERS CONFIGURATION
**Header:** SYSTEM SETTINGS & ADMISSION GATING  
**Figure 83. Administrator School Institutional Profile and DepEd Identifiers Configuration**  
> **Figure Description:** Capture the School Profile tab on settings.html showing School Name, DepEd ID 112937, Principal Name, Division, Region, and Logo upload

**Interface Controls & Elements:**

1. **DepEd School ID Input** – Configured official institutional identifier (112937).
2. **Official School Name** – Vinzons Pilot Elementary School.
3. **Institutional Administration** – Principal / Head Teacher name, Division, and Region.
4. **Official School Seal Uploader** – Uploads high-resolution school logo rendered on report cards.
5. **Contact Information** – Sets public office email, phone numbers, and Facebook Page URL.
6. **Save Profile Action** – Commits institutional data across all report headers.

---

### ADMINISTRATOR LANDING PAGE CONTENT MANAGEMENT SYSTEM (CMS) WITH LIVE PREVIEW
**Header:** SYSTEM SETTINGS & ADMISSION GATING  
**Figure 84. Administrator Landing Page Content Management System (CMS) with Live Preview**  
> **Figure Description:** Capture the CMS tab on settings.html showing the hero headline editor, announcement card toggles, core values editor, and the side-by-side live preview iframe

**Interface Controls & Elements:**

1. **Hero Headline & Subtitle Editor** – Customizes main banner headlines on landing page.
2. **Core Values & Programs Editor** – Updates text for Maka-Diyos, Makatao, Makakalikasan, Makabansa.
3. **Facilities & Photos Gallery** – Uploads campus photographs displayed on public portal.
4. **Live Preview Canvas** – Real-time iframe displaying how edits look before publishing.
5. **Save & Publish CMS Button** – Commits content changes to public website.

---

### ADMINISTRATOR SCHOOL FORMS & OFFICIAL REPORTS CENTER
**Header:** SCHOOL FORMS & OFFICIAL REPORTS CENTER  
**Figure 85. Administrator School Forms & Official Reports Center**  
> **Figure Description:** Capture academicRecords.html showing the School Forms & Official Reports Center catalog with the four active DepEd report cards: SF4, SF6, SF7, and SF10-ES

**Interface Controls & Elements:**

1. **Reports Catalog Header** – Title and live Refresh button to sync latest student data.
2. **SF4: Monthly Learner Movement Card** – View & Download SF4 button for monthly attendance matrix.
3. **SF6: Promotion & Proficiency Summary Card** – View & Download SF6 button for Form 20 matrix.
4. **SF7: Personnel Assignment & Profile Card** – View & Download SF7 button for faculty plantilla.
5. **SF10-ES: Permanent Academic Record Card** – Open SF10 Generator button for Form 137 workspace.
6. **Official PDF Viewer Modal** – Embedded preview with direct Download PDF and Download Excel buttons.

---

### ADMINISTRATOR BULK STUDENT CSV IMPORT INTERFACE
**Header:** ADMINISTRATIVE UTILITIES & EXPORTS  
**Figure 86. Administrator Bulk Student CSV Import Interface**  
> **Figure Description:** Capture importStudents.html showing the drag-and-drop CSV upload zone, file structure instructions, and import progress bar

**Interface Controls & Elements:**

1. **CSV Drag-and-Drop Zone** – Drop zone accepting official DepEd learner CSV files.
2. **CSV Header Format Guide** – Details required columns: lrn, last_name, first_name, gender, birth_date.
3. **Import Validation Progress Bar** – Validates duplicates and reports formatting errors.
4. **Commit Import Button** – Inserts validated student records into students table.

---

### OFFICIAL LIST OF ENROLLEES CERTIFICATE-STYLE PRINT PREVIEW TEMPLATE
**Header:** ADMINISTRATIVE UTILITIES & EXPORTS  
**Figure 87. Official List of Enrollees Certificate-Style Print Preview Template**  
> **Figure Description:** Capture preview_enrollees_template.html showing the formal ceremonial DepEd header, ornamental border, and enrolled pupil directory

**Interface Controls & Elements:**

1. **Ceremonial DepEd Header** – Republic of the Philippines, DepEd Region V, Division of Camarines Norte.
2. **Ornamental Border** – Formal certificate frame design suitable for superintendent presentation.
3. **Certified Enrollee Directory** – Itemized list of enrolled learners with LRN, Sex, and Section.
4. **Principal Certification Block** – Official signature and date line for School Principal.
5. **Print Document Action** – Formats ceremonial certificate for high-resolution printing.

---

# SECTION 9: OFFICIAL DEPED SCHOOL FORMS (SF) MASTER MATRIX

The following table summarizes the official DepEd School Forms generated, processed, and exported by VPES-SIMS:

| Form Code | Official DepEd Form Title | Responsible Role | Format & Generation Path |
| :--- | :--- | :--- | :--- |
| **SF1** | School Register | Class Adviser / Admin | Excel / PDF via Teacher Hub & Section Masterlist |
| **SF2** | Daily Attendance Report of Learners | Class Adviser | Excel / PDF with Monthly Date Selector |
| **SF3** | Books Issued and Returned | Subject Teacher / Adviser | Excel inventory export via Teacher Forms Hub |
| **SF4** | Monthly Learner Movement and Attendance | School Registrar / Admin | Legal PDF & Excel via Reports Center (`academicRecords.html`) |
| **SF5** | Report on Promotion and Level of Proficiency | Class Adviser | Consolidated end-of-year promotion grid |
| **SF6** | Summarized Report on Promotion (Form 20) | School Head / Admin | School-wide statistical matrix (`academicRecords.html`) |
| **SF7** | School Personnel Assignment List & Basic Profile | School Head / Admin | Faculty plantilla & class timetable (`academicRecords.html`) |
| **SF8** | Learner Basic Health and Nutrition Report | Class Adviser | Nutritional status and BMI assessment |
| **SF9** | Progress Report Card (Form 138) | Class Adviser / Student | Official quarterly ratings with MAPEH composite breakdown |
| **SF10-ES**| Learner Permanent Academic Record (Form 137)| School Registrar / Admin | Multi-year cumulative transcript (`academicRecords.html`) |
| **SNEd** | Special Needs Education & PWD Registry | SPED Coordinator / Admin | BEEF Section 5 compliant diagnostic directory |

---

# SECTION 10: FREQUENTLY ASKED QUESTIONS (FAQ) & TECHNICAL SUPPORT

**Q1: Is VPES-SIMS hosted locally on campus or accessible online?**  
*Answer:* VPES-SIMS is deployed on a dedicated cloud infrastructure on **Hostinger**, fully accessible online 24/7 via any modern web browser with HTTPS SSL encryption.

**Q2: Can parents create a single joint account for multiple children?**  
*Answer:* In compliance with DepEd data integrity policies, VPES-SIMS provisions **one individual account per student / applicant**. Guardians manage each child's academic records, appointments, and report cards through their respective assigned student accounts.

**Q3: How are scheduling conflicts prevented during class timetable creation?**  
*Answer:* The Schedule Builder features a real-time collision detection engine. If an administrator assigns a teacher or section to overlapping time slots, the system automatically flashes a red conflict modal, identifies the overlapping class, and blocks the entry until resolved.

**Q4: What happens if an applicant is assigned an official DepEd LRN after enrollment?**  
*Answer:* Administrators can open the Student Directory (`students.html`), click **"Update LRN"**, enter the 12-digit number in the DepEd LRN Update Modal (`#updateLrnModal`), and permanently link the official identifier.

**Q5: Who can I contact for institutional technical support?**  
* **Institution:** Vinzons Pilot Elementary School (DepEd School ID: 112937)
* **Address:** Vinzons, Camarines Norte, Region V – Bicol
* **Technical Inquiries:** Camarines Norte State College (CNSC) – Department of Computer Studies Capstone Research Group
* **System Administrator:** School Principal / Head Teacher Office – Vinzons Pilot Elementary School

---
*(End of Official User Manual Booklet – Vinzons Pilot Elementary School SIMS)*
