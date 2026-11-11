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
> **Figure Description:** Open index.html in a desktop browser. Capture the full viewport showing the top header bar with VPES logo and DepEd School ID (112937), the main navigation menu, the hero headline with school motto, the active admission status ribbon, and the primary "Enroll Now" and "Login" action buttons.

**Interface Controls & Elements:**

1. **Institutional Header & Logo** – Displays the official seals of DepEd and Vinzons Pilot Elementary School, school name, and DepEd School ID: 112937.
2. **Main Navigation Menu** – Fast navigation links to Home, About Us, Academic Programs, Announcements, and Contact Information.
3. **Dynamic Admission Status Ribbon** – Real-time status pill indicating whether Early Registration, Official Enrollment, or Re-enrollment is currently OPEN or CLOSED.
4. **Primary "Enroll Now" CTA Button** – Directs prospective kindergarten pupils and transferees to the online admission application form.
5. **Header "Login" Action Button** – Triggers the integrated authentication modal (#authModal) without leaving the landing page.
6. **Latest Announcements Feed** – Live display cards of urgent school bulletins, advisories, and Facebook-synced posts.

---

### INTEGRATED AUTHENTICATION MODAL – USER SIGN-IN INTERFACE
**Header:** USER AUTHENTICATION & SECURITY  
**Figure 2. Integrated Authentication Modal – User Sign-In Interface**  
> **Figure Description:** On index.html, click the "Login" button in the top navigation bar to launch #authModal in default Sign-In view. Capture the modal showing the "Welcome Back!" greeting, Email/Phone input field, password input with unmask eye icon, "Sign In to VPES" button, "Forgot Password?" link, and "Register" tab switch.

**Interface Controls & Elements:**

1. **Email or Mobile Input Field (#modal-loginEmail)** – Enter registered email address or active 11-digit Philippine mobile phone number.
2. **Password Input Field (#modal-loginPassword)** – Enter account password with masked security characters.
3. **Show / Hide Password Toggle (#modal-togglePassword)** – Click the eye icon to unmask and verify password characters.
4. **"Sign In to VPES" Button (#modal-submitBtn)** – Submits credentials to Firebase Authentication, updates last_login_at timestamp, and routes to role-specific dashboard.
5. **"Forgot Password?" Link (#modal-forgotPasswordLink)** – Switches modal to password recovery view (#modal-recoveryForm).
6. **"Register" Switch Tab (#modal-headerRegisterBtn)** – Expands modal into new applicant account registration view (#modal-signupForm).

---

### INTEGRATED AUTHENTICATION MODAL – ACCOUNT REGISTRATION VIEW
**Header:** USER AUTHENTICATION & SECURITY  
**Figure 3. Integrated Authentication Modal – Account Registration View**  
> **Figure Description:** Inside #authModal on index.html, click the "Register" tab to display #modal-signupForm. Capture the registration view showing First Name, Middle Name, Last Name, Email, Mobile Phone Number, Password, Confirm Password fields, and the "Create Account" button.

**Interface Controls & Elements:**

1. **Legal First Name Field (#modal-signupFirstName)** – Enter applicant/guardian official first name (Required).
2. **Middle Name Field (#modal-signupMiddleName)** – Enter legal middle name as recorded on civil documents (Optional).
3. **Last Name Field (#modal-signupLastName)** – Enter family surname (Required).
4. **Email Address Field (#modal-signupEmail)** – Enter valid email address for application tracking and appointment confirmations.
5. **Mobile Phone Number (#modal-signupPhone)** – Enter 11-digit Philippine mobile number (09XXXXXXXXX) required for mandatory SMS OTP verification.
6. **Password & Confirm Fields (#modal-signupPassword, #modal-signupConfirmPassword)** – Set secure password (min. 8 characters with numbers and symbols).
7. **"Create Account" Button (#modal-submitRegisterBtn)** – Validates inputs and triggers the 6-digit SMS OTP verification sequence.

---

### INTEGRATED AUTHENTICATION MODAL – 6-DIGIT PHONE OTP VERIFICATION SCREEN
**Header:** USER AUTHENTICATION & SECURITY  
**Figure 4. Integrated Authentication Modal – 6-Digit Phone OTP Verification Screen**  
> **Figure Description:** Submit the registration form in #authModal to trigger the SMS OTP gateway. Capture the #modal-otpScreen showing the masked phone display (e.g., 09******890), the six sequential OTP digit input boxes, the 60-second countdown timer, and "Verify & Proceed" button.

**Interface Controls & Elements:**

1. **Target Phone Display (#modal-otpPhoneDisplay)** – Displays masked recipient mobile number to protect user privacy.
2. **Sequential OTP Digit Boxes (.otp-input)** – Six auto-advancing input cells for entering the one-time PIN received via Semaphore SMS.
3. **Resend Code Countdown Timer (#modal-otpTimer)** – 60-second security countdown preventing rapid SMS gateway spamming.
4. **"Verify & Proceed" Button (#modal-verifyOtpBtn)** – Authenticates the 6-digit token, provisions the user account, and signs in the user.
5. **"Edit Phone Number" Action** – Returns to registration form if the mobile number was mistyped.

---

### MANDATORY FIRST-LOGIN PASSWORD CHANGE MODAL
**Header:** USER AUTHENTICATION & SECURITY  
**Figure 5. Mandatory First-Login Password Change Modal**  
> **Figure Description:** Log in with an administrator-provisioned teacher or staff account that has must_change_password = 1. Capture the modal injected by JS/firstLoginPasswordModal.js showing the mandatory change alert, New Password input (#flmNewPassword), Confirm Password input (#flmConfirmPassword), password strength validation chips (#chip-len, #chip-upper, #chip-lower, #chip-num, #chip-match), and "Update Password & Continue" button (#flmSubmitBtn).

**Interface Controls & Elements:**

1. **Security Mandatory Alert (#flmTitle)** – Explains that the temporary password assigned by the administrator must be updated before accessing the system.
2. **New Password Input (#flmNewPassword)** – Enter personal secure password with unmask toggle (#flmToggleNew).
3. **Confirm Password Input (#flmConfirmPassword)** – Re-enter new password with unmask toggle (#flmToggleConfirm).
4. **Real-Time Validation Chips** – Dynamic badges: 8+ chars (#chip-len), Uppercase (#chip-upper), Lowercase (#chip-lower), Number (#chip-num), Passwords Match (#chip-match).
5. **"Update Password & Continue" Button (#flmSubmitBtn)** – Updates password in Firebase Auth, clears must_change_password flag in MySQL, and opens portal dashboard.

---

### INTEGRATED AUTHENTICATION MODAL – PASSWORD RECOVERY INTERFACE
**Header:** USER AUTHENTICATION & SECURITY  
**Figure 6. Integrated Authentication Modal – Password Recovery Interface**  
> **Figure Description:** Inside #authModal on index.html, click "Forgot Password?" to transition to #modal-recoveryForm. Capture the recovery view showing the instructions banner, registered email input field, "Send Reset Link" action button, and "Back to Sign In" button.

**Interface Controls & Elements:**

1. **Recovery Advisory Header** – Outlines the automated email verification link procedure.
2. **Registered Email Field (#modal-recoveryEmail)** – Enter the email address associated with the portal account.
3. **"Send Reset Link" Button (#modal-sendResetBtn)** – Dispatches an official password recovery link via Hostinger SMTP / Firebase Auth.
4. **"Back to Sign In" Button (#modal-backToLoginBtn)** – Returns modal view to the standard sign-in form.

---

### SECURE SIGN-OUT CONFIRMATION MODAL
**Header:** USER AUTHENTICATION & SECURITY  
**Figure 7. Secure Sign-Out Confirmation Modal**  
> **Figure Description:** On any authenticated dashboard (Admin, Teacher, or Student), click "Logout" in the sidebar or user menu to trigger JS/logoutModal.js. Capture the SweetAlert2 confirmation dialog showing the warning icon, "Are you sure you want to log out?" prompt, "Confirm Logout" button, and "Cancel" button.

**Interface Controls & Elements:**

1. **Logout Confirmation Prompt** – Dialog asking user to verify session termination.
2. **"Confirm Logout" Action Button** – Clears sessionStorage, revokes Firebase auth tokens, and safely redirects to index.html.
3. **"Cancel" Action Button** – Dismisses dialog and maintains active portal session.

---

### PUBLIC HERO SECTION WITH REAL-TIME ADMISSION GATING STATUS
**Header:** PUBLIC LANDING PAGE & GUEST PORTAL  
**Figure 8. Public Hero Section with Real-Time Admission Gating Status**  
> **Figure Description:** Open index.html and capture the hero section displaying the institutional background image, the primary headline, the dynamic enrollment status pill (#admissionGatingPill showing "Early Registration Open", "Regular Enrollment Active", or "Admissions Closed"), and the primary call-to-action button.

**Interface Controls & Elements:**

1. **Hero School Headline** – Formal institutional banner and DepEd Region V educational motto.
2. **Admission Status Pill (#admissionGatingPill)** – Reflects real-time gating switches configured in administrative settings.
3. **Primary Enrollment CTA (#enrollBtn)** – Action button labeled "Enroll Now" when admissions are active, or "View Requirements" when closed.
4. **Portal Login CTA (#loginBtn)** – Direct shortcut triggering the integrated authentication modal.

---

### PUBLIC SCHOOL ANNOUNCEMENTS SECTION ON LANDING PAGE
**Header:** PUBLIC LANDING PAGE & GUEST PORTAL  
**Figure 9. Public School Announcements Section on Landing Page**  
> **Figure Description:** Scroll to the Announcements section (#announcementsSection) on index.html. Capture the section showing the section title, the three latest published bulletin cards with thumbnail photos, category tags, timestamps, "Read More" buttons, and the "View All Announcements" button.

**Interface Controls & Elements:**

1. **Announcements Header** – Section title: "School Advisories & Bulletins".
2. **Announcement Thumbnail & Photo** – High-resolution graphics or official DepEd memorandum cover.
3. **Category Badges** – Color-coded tags (Emergency Suspension, Academic Advisory, DepEd Memorandum).
4. **"Read More" Button** – Launches the full bulletin lightbox modal (#announcementModal).
5. **"View All Announcements" Button (#viewAllAnnBtn)** – Opens the complete historical archive lightbox.

---

### ANNOUNCEMENT DETAIL LIGHTBOX MODAL
**Header:** PUBLIC LANDING PAGE & GUEST PORTAL  
**Figure 10. Announcement Detail Lightbox Modal**  
> **Figure Description:** On index.html, click "Read More" on any announcement card to launch #announcementModal. Capture the modal displaying the headline, author role, date, full announcement text, and attached document image.

**Interface Controls & Elements:**

1. **Modal Close Button (#closeAnnouncementBtn)** – Closes the lightbox dialog.
2. **Official Bulletin Headline** – Complete title of the administrative notice.
3. **Publication Metadata** – Posting date, time, and posting authority (e.g., Office of the School Principal).
4. **Embedded Document Viewer** – High-resolution display of signed memoranda or advisory infographics.
5. **Full Bulletin Body** – Formatted announcement text with paragraph spacing.

---

### ALL ANNOUNCEMENTS ARCHIVE LIGHTBOX MODAL
**Header:** PUBLIC LANDING PAGE & GUEST PORTAL  
**Figure 11. All Announcements Archive Lightbox Modal**  
> **Figure Description:** On index.html, click "View All Announcements" to launch #announcementsArchiveModal. Capture the modal showing the announcement search input, category filter pills, chronological archive cards, and close button.

**Interface Controls & Elements:**

1. **Archive Search Box** – Filters historical announcements by keyword or date.
2. **Category Filter Tabs** – Filter archive by All, Emergency Suspensions, General Advisories, or DepEd Memos.
3. **Chronological Archive Cards** – Scrollable catalog of all historical bulletins.
4. **Close Archive Action** – Dismisses modal and returns to landing page view.

---

### ACADEMIC PROGRAMS AND CURRICULUM OFFERINGS SECTION
**Header:** PUBLIC LANDING PAGE & GUEST PORTAL  
**Figure 12. Academic Programs and Curriculum Offerings Section**  
> **Figure Description:** Scroll to #programsSection on index.html. Capture the curriculum offerings grid displaying cards for Kindergarten, Primary (Grades 1–3), Intermediate (Grades 4–6), Special Science Elementary School (SSES), and Special Needs Education (SNEd).

**Interface Controls & Elements:**

1. **Standard K-12 Elementary Card** – Highlights DepEd MATATAG basic curriculum learning areas.
2. **SSES Science Program Card** – Outlines enriched curriculum in Science, Mathematics, and Robotics.
3. **SNEd Inclusive Education Card** – Details SPED accommodations for learners with disabilities.
4. **Curriculum Information Links** – Access to DepEd curriculum standards and classroom guidelines.

---

### ADMISSION REQUIREMENTS CHECKLIST BY GRADE LEVEL
**Header:** PUBLIC LANDING PAGE & GUEST PORTAL  
**Figure 13. Admission Requirements Checklist by Grade Level**  
> **Figure Description:** Scroll to #requirementsSection on index.html. Capture the tabbed admission checklist showing tabs for Kindergarten, Transferee, and Balik-Aral, displaying mandatory physical documents and file format specifications.

**Interface Controls & Elements:**

1. **Applicant Category Tabs** – Toggle between Kindergarten, Transferee, and Balik-Aral requirements.
2. **Document Checklist Items** – Itemizes PSA Birth Certificate, SF9 Report Card, 1x1 Photos, and Certificates.
3. **Upload Guidelines Box** – Reminds parents of max file sizes (5MB) and accepted formats (JPG, PNG, PDF).
4. **Registrar Support Contacts** – Contact numbers for enrollment assistance.

---

### VPES DATA PRIVACY POLICY INTERFACE
**Header:** PUBLIC LANDING PAGE & GUEST PORTAL  
**Figure 14. VPES Data Privacy Policy Interface**  
> **Figure Description:** Click "Privacy Policy" in the footer of index.html or navigate to privacy-policy.html. Capture the page showing the RA 10173 statutory compliance notice, data collection boundaries, data sharing limitations, and security measures.

**Interface Controls & Elements:**

1. **Statutory RA 10173 Notice** – Statement of compliance with Philippine Data Privacy Act of 2012.
2. **Data Scope Disclosure** – Specifies personal, demographic, and academic data collected for DepEd LIS.
3. **Data Security Protocols** – Explains cloud SSL encryption, role-based controls, and automated audit trails.
4. **Learner Rights Notice** – Outlines parent rights to inspect and request correction of student data.

---

### STUDENT TYPE SELECTION MODAL (NEW APPLICANT VS. EXISTING STUDENT)
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 15. Student Type Selection Modal (New Applicant vs. Existing Student)**  
> **Figure Description:** After signing up as a new applicant or clicking "Enroll Now" on index.html, capture the dialog injected by JS/studentTypeModal.js showing the two primary cards: "New Student / Transferee" and "Existing / Currently Enrolled Student".

**Interface Controls & Elements:**

1. **"New Student / Transferee" Card** – Directs new learners to the online admission application form (SF1).
2. **"Existing / Currently Enrolled Student" Card** – Routes continuing learners to LRN verification and account linking.
3. **Category Descriptions** – Explains eligibility criteria for incoming pupils vs. continuing pupils.
4. **Modal Dismiss Action** – Closes modal and returns to dashboard.

---

### STUDENT TYPE CONFIRMATION DIALOG
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 16. Student Type Confirmation Dialog**  
> **Figure Description:** Select "New Student / Transferee" in the student type modal to trigger JS/studentTypeConfirmationModal.js. Capture the confirmation dialog displaying the chosen enrollment path and "Confirm & Proceed" button.

**Interface Controls & Elements:**

1. **Enrollment Path Summary** – Confirms selected admission category.
2. **"Confirm & Proceed" Button** – Commits student type and opens applicationform.html.
3. **"Change Selection" Button** – Returns to previous modal to select a different option.

---

### LRN VERIFICATION AND ACCOUNT LINKING MODAL
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 17. LRN Verification and Account Linking Modal**  
> **Figure Description:** Select "Existing Student" in the student type modal to trigger JS/lrnVerificationModal.js (#linkAccountModal). Capture the modal showing inputs for 12-digit LRN (#linkLrn), Student Birthdate (#linkBirthDate), and "Verify & Link Record" button (#btnLinkAccount).

**Interface Controls & Elements:**

1. **Official 12-Digit LRN Input (#linkLrn)** – Enter learner's official DepEd Learner Reference Number.
2. **Learner Birth Date Picker (#linkBirthDate)** – Date of birth required to match database records.
3. **"Verify & Link Record" Button (#btnLinkAccount)** – Queries MySQL database and attaches student record to guardian user account.
4. **Error Alert Box (#linkMessage)** – Displays warning notice if LRN or birthdate is incorrect.

---

### ONLINE ADMISSION FORM – STEP 1: SCHOOL INFORMATION & GRADE LEVEL SELECTION
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 18. Online Admission Form – Step 1: School Information & Grade Level Selection**  
> **Figure Description:** Navigate to applicationform.html. Capture Step 1 of the multi-step form showing the active School Year field (#schoolYear), Grade Level dropdown (#gradeLevel), Learner Status selection buttons (#withLrnNo, #withLrnYes, #returningLearner, #transferLearner), and "Next" button.

**Interface Controls & Elements:**

1. **School Year Field (#schoolYear)** – Pre-populated active academic term (e.g., S.Y. 2026–2027).
2. **Grade Level Dropdown (#gradeLevel)** – Select incoming grade level (Kindergarten to Grade 6).
3. **Learner Status Radios** – No LRN (Incoming Kinder), With LRN, Returning (Balik-Aral), or Transferee.
4. **Kindergarten Section Selector (#kindergartenSection)** – Appears when Kindergarten is selected.
5. **"Next Step" Action Button** – Validates entries and advances to Step 2 (Demographic Information).

---

### ONLINE ADMISSION FORM – STEP 2: STUDENT DEMOGRAPHIC & BEEF INFORMATION
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 19. Online Admission Form – Step 2: Student Demographic & BEEF Information**  
> **Figure Description:** Advance to Step 2 on applicationform.html. Capture the form showing PSA Birth Certificate No. (#psaBirth), Learner Name fields (#lastName, #firstName, #middleName, #extensionName), Birthdate (#birthDate), Sex radios (#sexMale, #sexFemale), Mother Tongue (#motherTongue), and 4Ps checkbox (#is4Ps).

**Interface Controls & Elements:**

1. **PSA Birth Certificate Registry No. (#psaBirth)** – Official civil registry birth certificate number.
2. **Legal Name Fields (#lastName, #firstName, #middleName, #extensionName)** – Learner full legal name.
3. **Birthdate Picker (#birthDate)** – Date of birth input with automatic age computation.
4. **Sex at Birth Radios (#sexMale, #sexFemale)** – Official gender classification for DepEd SF1.
5. **Mother Tongue Dropdown (#motherTongue)** – Primary native language spoken at home.
6. **4Ps Beneficiary Checkbox (#is4Ps)** – Flag for Pantawid Pamilyang Pilipino Program recipients.

---

### ONLINE ADMISSION FORM – STEP 3: PSGC CASCADING GEOGRAPHIC RESIDENTIAL ADDRESS
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 20. Online Admission Form – Step 3: PSGC Cascading Geographic Residential Address**  
> **Figure Description:** Advance to Step 3 on applicationform.html. Capture the cascading address dropdowns showing Region (#regionSelect - Region V), Province (#provinceSelect - Camarines Norte), Municipality (#municipalitySelect - Vinzons), Barangay dropdown (#barangaySelect), House No./Street (#streetAddress), and Zip Code (#zipCode - 4603).

**Interface Controls & Elements:**

1. **Region Selector (#regionSelect)** – Administrative region (Default: Region V - Bicol).
2. **Province Selector (#provinceSelect)** – Province dropdown (Default: Camarines Norte).
3. **Municipality Selector (#municipalitySelect)** – Municipality dropdown (Default: Vinzons).
4. **Barangay Cascading Dropdown (#barangaySelect)** – List of Vinzons barangays (Poblacion, Calangcawan, Mangcayo, etc.).
5. **House No. / Street Address (#streetAddress)** – Specific residential location.
6. **Postal Zip Code (#zipCode)** – Pre-filled postal code (4603 for Vinzons).

---

### ONLINE ADMISSION FORM – STEP 4: PARENT AND LEGAL GUARDIAN PROFILING
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 21. Online Admission Form – Step 4: Parent and Legal Guardian Profiling**  
> **Figure Description:** Advance to Step 4 on applicationform.html. Capture the parent profiling fields showing Father's Name (#fatherLastName, #fatherFirstName), Mother's Maiden Name (#motherLastName, #motherFirstName), Guardian details (#guardianLastName, #guardianFirstName), and Emergency Contact Number (#emergencyContact).

**Interface Controls & Elements:**

1. **Father's Full Name Fields** – Surname, first name, middle name, and mobile number.
2. **Mother's Maiden Name Fields** – Legal maiden surname, first name, middle name, and mobile phone.
3. **Legal Guardian Profile** – Guardian name and relationship if learner does not reside with parents.
4. **Primary Emergency Mobile (#emergencyContact)** – Validated 11-digit mobile contact for urgent notices.

---

### ONLINE ADMISSION FORM – STEP 5: SPECIAL NEEDS EDUCATION (SNED) & DISABILITY PROFILING
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 22. Online Admission Form – Step 5: Special Needs Education (SNEd) & Disability Profiling**  
> **Figure Description:** Advance to Step 5 on applicationform.html. Capture the BEEF Section 5 profiling section showing "Has Disability" toggle (#hasDisability), Medical Diagnoses checkboxes (a1: Autism, ADHD, Cerebral Palsy, Visual, Hearing), Manifestations checkboxes (a2), and PWD ID Number input (#pwdIdNumber).

**Interface Controls & Elements:**

1. **Special Needs Toggle (#hasDisability)** – Activates BEEF Section 5 inclusive education profiling.
2. **Medical Diagnoses Checkboxes (a1)** – Certified conditions diagnosed by licensed medical specialists.
3. **Observed Manifestations Checkboxes (a2)** – Observed learning, mobility, or communication difficulties.
4. **PWD ID Number Field (#pwdIdNumber)** – Official government Person with Disability card number.
5. **Medical Assessment Upload Slot** – Optional attachment for diagnostic assessment reports.

---

### ONLINE ADMISSION FORM – STEP 6: RETURNING LEARNER (BALIK-ARAL) AND TRANSFEREE HISTORY
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 23. Online Admission Form – Step 6: Returning Learner (Balik-Aral) and Transferee History**  
> **Figure Description:** Advance to Step 6 on applicationform.html. Capture the previous school history fields showing Last Grade Level Completed (#lastGradeCompleted), Last School Year Attended (#lastSchoolYear), Previous School Name (#previousSchoolName), and School ID (#previousSchoolId).

**Interface Controls & Elements:**

1. **Last Grade Completed (#lastGradeCompleted)** – Educational attainment prior to current application.
2. **Last School Year Attended (#lastSchoolYear)** – Academic year of last active school attendance.
3. **Previous School Name (#previousSchoolName)** – Official name of school of origin.
4. **Previous DepEd School ID (#previousSchoolId)** – 6-digit DepEd institutional identifier.

---

### ONLINE ADMISSION FORM – STEP 7: LEARNING MODALITY PREFERENCES
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 24. Online Admission Form – Step 7: Learning Modality Preferences**  
> **Figure Description:** Advance to Step 7 on applicationform.html. Capture the learning modality preferences card showing radio options for Face-to-Face, Blended, and Modular learning, digital device access checkboxes, and "Proceed to Document Upload" button.

**Interface Controls & Elements:**

1. **Learning Modality Radios** – Preferred instructional setup (In-Person Face-to-Face, Blended, Modular).
2. **Household Digital Devices** – Checkboxes for smartphone, tablet, laptop, desktop, and internet connectivity.
3. **"Proceed to Document Upload" Button** – Commits form entries and navigates to uploadDocument.html.

---

### DOCUMENT UPLOAD INTERFACE WITH GRADE-SPECIFIC REQUIREMENT SLOTS
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 25. Document Upload Interface with Grade-Specific Requirement Slots**  
> **Figure Description:** Navigate to uploadDocument.html. Capture the document upload slots for PSA Birth Certificate (#section-birth-cert), SF9 / Form 138 Report Card (#section-report-card), Kinder Certificate (#section-kinder-cert), file dropzones, and upload progress indicators.

**Interface Controls & Elements:**

1. **PSA Birth Certificate Slot (#section-birth-cert)** – Mandatory upload zone for digitized birth record.
2. **SF9 Report Card Slot (#section-report-card)** – Required upload zone for transferees showing past grades.
3. **1x1 / 2x2 ID Photo Slot** – Learner photo with white background.
4. **File Drag-and-Drop Dropzone** – Supports JPG, PNG, and PDF files up to 5MB.
5. **"Proceed to Review" Action Button** – Advances to final verification review on review.html.

---

### APPLICATION REVIEW, DATA PRIVACY AGREEMENT, AND DEPED CERTIFICATION
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 26. Application Review, Data Privacy Agreement, and DepEd Certification**  
> **Figure Description:** Navigate to review.html. Capture the comprehensive application summary displaying applicant demographic details, address, parent contacts, missing documents alert (#missingDocsAlert), Data Privacy Agreement checkbox, and "Submit Application" button.

**Interface Controls & Elements:**

1. **Missing Documents Alert (#missingDocsAlert)** – Flags if mandatory credentials are not yet uploaded.
2. **Comprehensive Review Panels** – Displays all encoded BEEF personal, address, and parent data.
3. **Truthfulness Certification Checkbox** – Legal certification that submitted information is true and correct.
4. **Data Privacy Consent Checkbox** – Formal agreement under RA 10173 terms.
5. **"Submit Application" Button** – Encrypts and transmits application to the registrar's review queue.

---

### APPLICATION SUBMISSION SUCCESS DIALOG WITH TRACKING CODE GENERATION
**Header:** ONLINE ADMISSIONS (DEPED BEEF COMPLIANCE)  
**Figure 27. Application Submission Success Dialog with Tracking Code Generation**  
> **Figure Description:** Submit the application on review.html to trigger the success dialog. Capture the confirmation dialog showing the green checkmark icon, the generated Application Reference Number (e.g., APP-2026-112937-042), QR tracking code, and "Proceed to Dashboard" button.

**Interface Controls & Elements:**

1. **Submission Success Confirmation** – Confirms successful database storage and queue placement.
2. **Unique Application Reference Number** – Official tracking code (e.g., APP-2026-112937-042).
3. **Tracking QR Code** – Quick-scan code for verification at the campus security gate.
4. **"Proceed to Dashboard" Button** – Navigates to applicantDashboard.html to schedule document submission.

---

### APPLICANT DASHBOARD WITH 5-STAGE ADMISSION PROGRESS TIMELINE
**Header:** DOCUMENT SUBMISSION & APPOINTMENT SCHEDULER  
**Figure 28. Applicant Dashboard with 5-Stage Admission Progress Timeline**  
> **Figure Description:** Open applicantDashboard.html. Capture the applicant home screen showing the learner header, reference code, current application status banner, and the 5-stage progress timeline (Submitted, Under Review, Appointment Booked, Verified, Officially Enrolled).

**Interface Controls & Elements:**

1. **Applicant Information Header** – Displays pupil name, reference ID, and target grade level.
2. **5-Stage Admission Pipeline** – Visual progress tracker highlighting current processing milestone.
3. **Status Advisory Notification** – Actionable instructions explaining next required applicant step.
4. **Dashboard Navigation Menu** – Tabs for Application Details, Documents, and Schedule Appointment.

---

### APPLICANT APPLICATION DETAILS TAB WITH BEEF DATA VIEWER
**Header:** DOCUMENT SUBMISSION & APPOINTMENT SCHEDULER  
**Figure 29. Applicant Application Details Tab with BEEF Data Viewer**  
> **Figure Description:** Click the "Application Details" tab on applicantDashboard.html (or open applicationDetails.html). Capture the full read-only dossier displaying submitted personal, address, parent, and SNEd information.

**Interface Controls & Elements:**

1. **Personal Information Panel** – Read-only display of legal name, birthdate, sex, and LRN.
2. **Residential Address Panel** – Registered residence in Vinzons, Camarines Norte.
3. **Parent / Guardian Panel** – Profiles and phone contacts of father, mother, and guardian.
4. **Data Correction Advisory** – Instructions for requesting updates through the school registrar.

---

### APPLICANT DOCUMENT SUBMISSION MANAGEMENT & RE-UPLOAD INTERFACE
**Header:** DOCUMENT SUBMISSION & APPOINTMENT SCHEDULER  
**Figure 30. Applicant Document Submission Management & Re-upload Interface**  
> **Figure Description:** Click the "Documents" tab on applicantDashboard.html. Capture the uploaded documents list showing verification status pills (Verified, Pending, Flagged), registrar feedback remarks, and "Re-upload" buttons for flagged files.

**Interface Controls & Elements:**

1. **Uploaded Document Cards** – Itemizes submitted credentials and timestamps.
2. **Status Badges** – Green (Verified), Yellow (Pending Review), Red (Flagged / Rejected).
3. **Registrar Feedback Box** – Explains reason for rejection (e.g., blurred scan or missing page).
4. **"Re-upload" Action Button** – Opens replacement modal to submit a clear document copy.

---

### DOCUMENT FULL-SCREEN REVIEW LIGHTBOX MODAL
**Header:** DOCUMENT SUBMISSION & APPOINTMENT SCHEDULER  
**Figure 31. Document Full-Screen Review Lightbox Modal**  
> **Figure Description:** On the documents tab, click "View" on any uploaded file to trigger #viewModal. Capture the full-screen lightbox displaying an uploaded PSA Birth Certificate with zoom controls, "Open in New Tab" button (#viewOpenNewTabBtn), and close button (#closeViewBtn).

**Interface Controls & Elements:**

1. **Lightbox Canvas (#documentPreview)** – High-resolution rendering of JPG, PNG, or PDF file.
2. **Zoom & Pan Controls** – Inspect fine print and civil registry stamps.
3. **"Open in New Tab" Action (#viewOpenNewTabBtn)** – Launches native browser PDF viewer.
4. **Close Viewer Button (#closeViewBtn)** – Dismisses lightbox.

---

### DOCUMENT FILE REPLACEMENT MODAL
**Header:** DOCUMENT SUBMISSION & APPOINTMENT SCHEDULER  
**Figure 32. Document File Replacement Modal**  
> **Figure Description:** Click "Re-upload" on a flagged document card on applicantDashboard.html. Capture the file replacement modal showing target document title, drag-and-drop file dropzone, file name display, and "Confirm Replacement" button.

**Interface Controls & Elements:**

1. **Target Document Indicator** – Identifies which credential is being replaced.
2. **Replacement File Dropzone** – Select new clear document file (max 5MB).
3. **"Confirm Replacement" Button** – Overwrites blurred file in cloud storage and resets status to Pending.
4. **Cancel Button** – Aborts file replacement.

---

### ON-SITE PHYSICAL DOCUMENT SUBMISSION DATE SELECTOR INTERFACE
**Header:** DOCUMENT SUBMISSION & APPOINTMENT SCHEDULER  
**Figure 33. On-Site Physical Document Submission Date Selector Interface**  
> **Figure Description:** Navigate to the Schedule Appointment section (#bookApptSection) on studentDashboard.html. Capture the interface showing the approved application alert banner, the appointment date dropdown displaying open dates with remaining capacity (e.g., "Monday, November 9, 2026 — 30 slots left"), and preferred session radio options.

**Interface Controls & Elements:**

1. **Admission Clearance Banner** – Confirms online application is approved for on-site verification.
2. **Appointment Date Dropdown** – Lists available DepEd verification dates with remaining slot counts.
3. **Session Radios** – Morning Session (8:00 AM – 12:00 PM) or Afternoon Session (1:00 PM – 5:00 PM).
4. **Mandatory Physical Checklist** – Reminds parents to bring original PSA certificate and Form 138.
5. **"Book Appointment" Action Button** – Submits date selection to launch confirmation dialog.

---

### APPOINTMENT SLOT BOOKING CONFIRMATION MODAL
**Header:** DOCUMENT SUBMISSION & APPOINTMENT SCHEDULER  
**Figure 34. Appointment Slot Booking Confirmation Modal**  
> **Figure Description:** Select an appointment date and session on studentDashboard.html and click "Book Appointment" to trigger #apptModal. Capture the confirmation modal displaying the chosen date, session hours, applicant reference number, and "Confirm Booking" button.

**Interface Controls & Elements:**

1. **Reserved Schedule Card** – Highlights selected date and morning/afternoon session window.
2. **Campus Venue Location** – Vinzons Pilot Elementary School Registrar / Principal Office.
3. **"Confirm Booking" Button** – Commits appointment to slot_bookings table and decrements slot capacity.
4. **"Change Date" Button** – Returns to date selector to choose a different date.

---

### OFFICIAL DOCUMENT VERIFICATION APPOINTMENT SLIP WITH QR CODE
**Header:** DOCUMENT SUBMISSION & APPOINTMENT SCHEDULER  
**Figure 35. Official Document Verification Appointment Slip with QR Code**  
> **Figure Description:** Confirm an appointment slot to generate the official printable Appointment Slip. Capture the slip view showing the official DepEd letterhead, applicant name, scheduled date/time, QR verification code, and print button.

**Interface Controls & Elements:**

1. **DepEd Institutional Letterhead** – Region V, Division of Camarines Norte, Vinzons Pilot Elementary School.
2. **Visitor & Applicant Details** – Pupil name, tracking reference number, and grade level.
3. **Scheduled Date & Time Window** – Clear highlight of reserved document submission session.
4. **Security QR Verification Code** – Scannable gate pass code verified by school security personnel.
5. **"Print Slip" Action Button** – Launches browser print dialog to print or save as PDF.

---

### ENROLLED STUDENT DASHBOARD HOME AND ADVISORY SECTION CARD
**Header:** ENROLLED STUDENT & PARENT PORTAL  
**Figure 36. Enrolled Student Dashboard Home and Advisory Section Card**  
> **Figure Description:** Log in with an officially enrolled student account on studentDashboard.html. Capture the enrolled home screen showing the learner header with 12-digit LRN badge, Section Information Card (#studentInfoCard) with section name, room number, and class adviser name, and announcements feed.

**Interface Controls & Elements:**

1. **Learner Header Card** – Student legal name, 12-digit LRN (#studentLinkedLrn), and school year.
2. **Advisory Section Card (#studentInfoCard)** – Section Name (#studentLinkedSection), Room (#studentLinkedRoom), and Adviser.
3. **Quick Navigation Tabs** – Fast links to Schedule, Grades (SF9), Re-Enrollment, and Profile.
4. **School Bulletins Feed** – Live administrative announcements and weather suspension alerts.

---

### ENROLLED STUDENT WEEKLY INTERACTIVE TIMETABLE / CLASS SCHEDULE
**Header:** ENROLLED STUDENT & PARENT PORTAL  
**Figure 37. Enrolled Student Weekly Interactive Timetable / Class Schedule**  
> **Figure Description:** Click the "Schedule" tab on studentDashboard.html. Capture the 5-day weekly class timetable grid (Monday to Friday, 7:00 AM–5:00 PM) showing color-coded subject cards, assigned teacher names, classroom locations, and "Print Schedule" button.

**Interface Controls & Elements:**

1. **Weekly Timetable Grid** – 5-column calendar schedule for the enrolled section.
2. **Subject Schedule Blocks** – Displays subject code, title, time interval, and assigned room.
3. **Subject Teacher Designation** – Identifies faculty member instructing each learning area.
4. **"Print Timetable" Button** – Formats schedule for printable display.

---

### ENROLLED STUDENT QUARTERLY ACADEMIC GRADES DISPLAY
**Header:** ENROLLED STUDENT & PARENT PORTAL  
**Figure 38. Enrolled Student Quarterly Academic Grades Display**  
> **Figure Description:** Click the "Grades" tab on studentDashboard.html. Capture the official DepEd SF9 electronic report card matrix displaying learning areas, Quarter 1 to 4 numeric grades, Final Rating, Remarks (Passed/Failed), General Academic Average card, and "Download SF9 (PDF)" button.

**Interface Controls & Elements:**

1. **SF9 Academic Grades Table** – Official curriculum subjects with Q1, Q2, Q3, and Q4 columns.
2. **Final Rating & Remarks Column** – Computed weighted grade and automated Passed/Failed status.
3. **General Average Card** – Highlights learner overall general academic average.
4. **"Download SF9 (PDF)" Button** – Exports official printable DepEd SF9 progress report card.

---

### ENROLLED STUDENT MAPEH COMPOSITE GRADE AND COMPONENT BREAKDOWN DRAWER
**Header:** ENROLLED STUDENT & PARENT PORTAL  
**Figure 39. Enrolled Student MAPEH Composite Grade and Component Breakdown Drawer**  
> **Figure Description:** On the Grades tab of studentDashboard.html, click on the MAPEH row or the component breakdown drawer button. Capture the drawer displaying quarterly ratings for Music, Arts, Physical Education, and Health that compose the overall MAPEH rating.

**Interface Controls & Elements:**

1. **MAPEH Composite Score** – Quarterly composite mark derived from the 4 sub-areas.
2. **Music Sub-Grade** – Numerical rating for Music competencies.
3. **Arts Sub-Grade** – Numerical rating for Visual and Applied Arts.
4. **Physical Education Sub-Grade** – Numerical rating for Physical activity and sports.
5. **Health Sub-Grade** – Numerical rating for Health, hygiene, and nutrition.

---

### ENROLLED STUDENT HISTORICAL SCHOOL YEAR GRADE ARCHIVE BROWSER
**Header:** ENROLLED STUDENT & PARENT PORTAL  
**Figure 40. Enrolled Student Historical School Year Grade Archive Browser**  
> **Figure Description:** On the Grades tab of studentDashboard.html, open the School Year archive selector dropdown. Capture the historical view showing past academic terms and archived finalized grades from previous grade levels.

**Interface Controls & Elements:**

1. **School Year Archive Dropdown** – Select past completed academic terms.
2. **Historical Grades Table** – Read-only display of finalized marks from previous grade levels.
3. **Historical Promotion Status** – Confirms promotion record for past school years.

---

### ENROLLED STUDENT MASTER PROFILE VIEW
**Header:** ENROLLED STUDENT & PARENT PORTAL  
**Figure 41. Enrolled Student Master Profile View**  
> **Figure Description:** Click the "Profile" tab on studentDashboard.html. Capture the profile view showing learner demographic details, PSA registry number, 12-digit LRN, registered address in Vinzons, parent contacts, and password management form.

**Interface Controls & Elements:**

1. **Learner Demographic Card** – Official legal name, birthdate, sex, and DepEd 12-digit LRN.
2. **Residential Address Card** – Registered home address in Vinzons, Camarines Norte.
3. **Parent / Guardian Contacts** – Father, Mother, Guardian profiles and phone numbers.
4. **Password Update Form** – Update portal account security password.

---

### CONTINUING STUDENT RE-ENROLLMENT CONFIRMATION TAB
**Header:** ENROLLED STUDENT & PARENT PORTAL  
**Figure 42. Continuing Student Re-Enrollment Confirmation Tab**  
> **Figure Description:** Click the "Re-Enrollment" tab (#reEnrollmentNavItem) on studentDashboard.html when re-enrollment gating is active. Capture the tab showing incoming school year, target grade level, address/contact update inputs, and "Submit Re-Enrollment" button.

**Interface Controls & Elements:**

1. **Re-Enrollment Status Banner** – Indicates continuation filing is active for the upcoming year.
2. **Target Incoming Grade Level** – Auto-computed next grade level based on year-end promotion.
3. **Contact Information Verification** – Update current home address and mobile phone.
4. **"Submit Re-Enrollment" Button** – Submits continuation intent directly to the registrar queue.

---

### ALUMNI / GRADUATED STUDENT INTERFACE AND PERMANENT RECORD ACCESS
**Header:** ENROLLED STUDENT & PARENT PORTAL  
**Figure 43. Alumni / Graduated Student Interface and Permanent Record Access**  
> **Figure Description:** Log in with an alumni account (a learner who graduated Grade 6). Capture studentDashboard.html showing the "Elementary Graduate" completion badge, graduation school year, and permanent academic record (SF10) request access.

**Interface Controls & Elements:**

1. **Elementary Graduate Badge** – Confirms completion of elementary education at VPES.
2. **Graduation Academic Term** – Official school year and date of elementary graduation.
3. **Permanent Record Request** – Option to request certified SF10 (Form 137) transcript for high school enrollment.
4. **Historical Academic Transcript** – Permanent archive of complete elementary marks.

---

### TEACHER DASHBOARD OVERVIEW, ADVISORY CLASS SUMMARY, AND TEACHING LOADS
**Header:** TEACHER & FACULTY PORTAL  
**Figure 44. Teacher Dashboard Overview, Advisory Class Summary, and Teaching Loads**  
> **Figure Description:** Log in with a teacher account on teacherDashboard.html. Capture the dashboard showing active school year badge (#activeSchoolYearBadge), teacher name (#teacherName), total classes (#totalClasses), total students (#totalStudents), total teaching hours (#totalTeachingHours), advisory section card (#advisorySectionName), and today's schedule drawer.

**Interface Controls & Elements:**

1. **Teacher Identification Header** – Profile photo, full name (#teacherName), and role badge.
2. **Workload Summary Metrics** – Total Classes (#totalClasses), Students (#totalStudents), and Hours (#totalTeachingHours).
3. **Advisory Section Card (#advisorySectionName)** – Displays handled homeroom section and pupil count.
4. **Today's Schedule Drawer (#todayScheduleContainer)** – Highlights scheduled periods for the current day.
5. **Grading Sheet Shortcut** – Fast link to quarterly grade encoding interface.

---

### TEACHER RIGHT-SIDEBAR INTERACTIVE CALENDAR AND TODAY'S CLASS SCHEDULE DRAWER
**Header:** TEACHER & FACULTY PORTAL  
**Figure 45. Teacher Right-Sidebar Interactive Calendar and Today's Class Schedule Drawer**  
> **Figure Description:** On teacherDashboard.html, expand the right sidebar (#rightSidebar). Capture the interactive mini calendar (#calendarMonth), today's class schedule timeline (#todayScheduleContainer), active class countdown badge, and room numbers.

**Interface Controls & Elements:**

1. **Interactive Mini Calendar (#calendarMonth)** – Month calendar with date selection.
2. **Today's Class Schedule Timeline** – Chronological list of teaching periods for the active day.
3. **Active Class Countdown Badge** – Highlights ongoing subject period with time remaining.
4. **Classroom Location Tag** – Assigned room number for upcoming classes.

---

### TEACHER ADVISORY STUDENT ROSTER DIRECTORY
**Header:** TEACHER & FACULTY PORTAL  
**Figure 46. Teacher Advisory Student Roster Directory**  
> **Figure Description:** Navigate to teacherStudents.html. Capture the advisory pupil directory showing total students stat (#totalStudents), search input (#studentSearch), section filter (#sectionFilter), and students table (#studentsTableBody) separated into Male and Female DepEd roster format.

**Interface Controls & Elements:**

1. **Total Advisory Count (#totalStudents)** – Headcount summary for the advisory section.
2. **Pupil Search Bar (#studentSearch)** – Filter by student name or 12-digit LRN.
3. **Male Pupils Directory** – Alphabetical listing of male learners with LRN and birthdate.
4. **Female Pupils Directory** – Alphabetical listing of female learners in official DepEd format.
5. **Parent Contact Numbers** – Direct phone numbers for emergency homeroom communication.
6. **"View Profile" Action Button** – Opens student detail inspection modal (#viewProfileModal).

---

### TEACHER STUDENT PROFILE INSPECTION MODAL
**Header:** TEACHER & FACULTY PORTAL  
**Figure 47. Teacher Student Profile Inspection Modal**  
> **Figure Description:** On teacherStudents.html, click "View Profile" on any student row to trigger #viewProfileModal. Capture the modal displaying student photo, 12-digit LRN (#modalProfileLrn), birthdate, address, and parent contact history.

**Interface Controls & Elements:**

1. **Learner Demographic Details** – Full legal name, 12-digit LRN (#modalProfileLrn), and age.
2. **Permanent Address Panel** – Complete residence in Vinzons, Camarines Norte.
3. **Parent / Guardian Profiles** – Father, Mother, Guardian names and registered phone numbers.
4. **Close Profile Button** – Dismisses modal.

---

### TEACHER QUARTERLY GRADING SHEET SPREADSHEET GRID
**Header:** TEACHER & FACULTY PORTAL  
**Figure 48. Teacher Quarterly Grading Sheet Spreadsheet Grid**  
> **Figure Description:** Navigate to teacherGrades.html. Capture the grading interface showing the section selector (#sectionsGrid), subject chips tabs (#subjectChipsList), grading quarter tabs (#masterPeriodButtons: Q1, Q2, Q3, Q4), numeric grade input cells (.grade-input), auto-computed general average, and Save button.

**Interface Controls & Elements:**

1. **Section Selector Cards (#sectionsGrid)** – Choose handled class section.
2. **Subject Chips Tabs (#subjectChipsList)** – Select DepEd curriculum learning area to grade.
3. **Quarter Selector Tabs (#masterPeriodButtons)** – Toggle between 1st, 2nd, 3rd, and 4th Quarter.
4. **Numerical Grade Input Cells (.grade-input)** – Inputs restricted to valid 60–100 DepEd scale.
5. **Auto-Computed General Average** – Real-time computation of learner quarterly average.
6. **Automated Remarks Badge** – Displays Passed (>=75) or Failed (<75) badge.
7. **"Save Grades" Action Button** – Commits encoded grades to database.

---

### TEACHER MAPEH COMPONENT BREAKDOWN AND SUB-GRADING MODAL
**Header:** TEACHER & FACULTY PORTAL  
**Figure 49. Teacher MAPEH Component Breakdown and Sub-Grading Modal**  
> **Figure Description:** On teacherGrades.html, select MAPEH and click "Breakdown" on any pupil row to launch #mapehBreakdownModal. Capture the modal showing student name (#mapehModalStudentName), quarter (#mapehModalQuarter), separate grade inputs for Music, Arts, PE, and Health, and live computed average.

**Interface Controls & Elements:**

1. **Student Header (#mapehModalStudentName)** – Identifies pupil and active quarter.
2. **Music Grade Input** – Numerical mark for Music curriculum competencies.
3. **Arts Grade Input** – Numerical mark for Visual and Creative Arts.
4. **Physical Education Grade Input** – Numerical mark for Physical fitness and sports.
5. **Health Grade Input** – Numerical mark for Health and hygiene competencies.
6. **Computed MAPEH Average** – Auto-calculated average transferred to main grading spreadsheet.

---

### TEACHER INDIVIDUAL WEEKLY TEACHING SCHEDULE AND PRINT LAYOUT
**Header:** TEACHER & FACULTY PORTAL  
**Figure 50. Teacher Individual Weekly Teaching Schedule and Print Layout**  
> **Figure Description:** Navigate to teacherSchedule.html. Capture the weekly timetable view showing total classes (#totalClasses), total hours (#totalHours), 5-day schedule grid (#teacherTimetableBody), subject schedule blocks with room numbers, and "Print Schedule" button.

**Interface Controls & Elements:**

1. **Workload Summary Header** – Displays total handled classes, sections, and teaching hours.
2. **Weekly Schedule Grid (#teacherTimetableBody)** – 5-day calendar grid (Monday to Friday, 7:00 AM–5:00 PM).
3. **Class Schedule Blocks** – Color-coded subject blocks displaying section and classroom location.
4. **Class Details Modal (#classDetailsModal)** – Click any block to inspect full period details.
5. **"Print Schedule" Action Button** – Formats individual teaching schedule for classroom display.

---

### TEACHER DEPED SCHOOL FORMS HUB (SF1 TO SF8 GENERATION CARDS)
**Header:** TEACHER & FACULTY PORTAL  
**Figure 51. Teacher DepEd School Forms Hub (SF1 to SF8 Generation Cards)**  
> **Figure Description:** Navigate to teacherSchoolForms.html. Capture the catalog grid (#teacherCatalogGrid) displaying generation cards for SF1 (School Register), SF2 (Daily Attendance), SF5 (Promotion Report), and SF9 (Progress Report Card).

**Interface Controls & Elements:**

1. **SF1: School Register Card** – Generate official class register in Excel or PDF format.
2. **SF2: Daily Attendance Card** – Generate monthly learner attendance report.
3. **SF5: Report on Promotion Card** – Generate end-of-year promotion and proficiency matrix.
4. **SF9: Progress Report Card Hub** – Access batch report card generator workspace.
5. **"Generate Form" Button** – Opens form options modal (#formOptionsModal).

---

### TEACHER SF2 DAILY ATTENDANCE MONTH AND YEAR SELECTION MODAL
**Header:** TEACHER & FACULTY PORTAL  
**Figure 52. Teacher SF2 Daily Attendance Month and Year Selection Modal**  
> **Figure Description:** On teacherSchoolForms.html, click "Generate SF2" to trigger the attendance configuration modal. Capture the dialog showing School Year selector, Month dropdown (June to March), and "Generate SF2 Report" button.

**Interface Controls & Elements:**

1. **School Year Selector** – Select active academic school year.
2. **Reporting Month Dropdown** – Choose calendar month (June to March) for attendance calculation.
3. **"Generate SF2 Report" Button** – Compiles daily attendance and computes monthly average attendance.
4. **Export Format Selector** – Choose between Excel (.xlsx) and printable PDF formats.

---

### TEACHER SF9 PROGRESS REPORT CARD WORKSPACE & BATCH ZIP DOWNLOAD INTERFACE
**Header:** TEACHER & FACULTY PORTAL  
**Figure 53. Teacher SF9 Progress Report Card Workspace & Batch ZIP Download Interface**  
> **Figure Description:** On teacherSchoolForms.html, open the SF9 workspace (#teacherWorkspaceView). Capture the student list (#sf9StudentTableSection) showing pupil rows with "Preview Card" buttons, grading completeness indicator, and "Download All (ZIP)" batch export button (#sf9ActionsContainer).

**Interface Controls & Elements:**

1. **Section Pupil List (#sf9StudentTableSection)** – Roster of learners with finalized quarterly marks.
2. **"Preview Card" Action Button** – Opens individual official DepEd SF9 report card PDF.
3. **"Download All (ZIP)" Button (#sf9ActionsContainer)** – Packages all section report cards into a single ZIP file.
4. **Grading Completeness Bar** – Confirms 100% of subject grades are encoded before batch export.

---

### TEACHER ACCOUNT PROFILE AND PASSWORD SETTINGS
**Header:** TEACHER & FACULTY PORTAL  
**Figure 54. Teacher Account Profile and Password Settings**  
> **Figure Description:** Navigate to teacherSettings.html. Capture the Profile tab (#profileTab) and Account tab (#accountTab) showing employee details, contact info (#displayName, #email, #phone), and password update form (#passwordForm).

**Interface Controls & Elements:**

1. **Profile Information Form (#profileForm)** – Display Name (#displayName), Email (#email), Phone (#phone).
2. **Profile Picture Uploader (#profilePicInput)** – Upload personal avatar photo.
3. **Password Update Form (#passwordForm)** – Current Password, New Password, Confirm Password.
4. **Password Strength Meter (#passwordStrength)** – Visual indicator of password robustness.
5. **"Save Changes" Button** – Commits updated profile credentials to database.

---

### ADMINISTRATOR EXECUTIVE DASHBOARD WITH REAL-TIME KPIS AND DAILY APPOINTMENT STREAM
**Header:** ADMINISTRATOR DASHBOARD & KPI ANALYTICS  
**Figure 55. Administrator Executive Dashboard with Real-Time KPIs and Daily Appointment Stream**  
> **Figure Description:** Log in with an administrator account on adminDashboard.html. Capture the executive dashboard showing the four KPI summary cards: Total Applications (#kpiTotalApps), Pending Review (#kpiPendingApps), Today's Appointments (#kpiTodayAppts), Enrolled Students (#kpiEnrolledApps), and the admissions queue table (#applicationsTable).

**Interface Controls & Elements:**

1. **Executive KPI Cards Header** – Real-time counts: Total Apps (#kpiTotalApps), Pending (#kpiPendingApps), Appointments (#kpiTodayAppts), Enrolled (#kpiEnrolledApps).
2. **Today's Appointments Stream** – Real-time queue of scheduled on-site document verification visits.
3. **Admissions Queue Table (#applicationsTable)** – Embedded list of recent applicants with status badges.
4. **"Refresh Dashboard" Button (#btnDashboardRefresh)** – Refreshes all KPI metrics without page reload.
5. **Fast Operations Shortcuts** – Direct access buttons to evaluate applications or assign sections.

---

### ADMINISTRATOR INTERACTIVE ANALYTICS GRAPH (BAR GRAPH / LINE TREND TOGGLE)
**Header:** ADMINISTRATOR DASHBOARD & KPI ANALYTICS  
**Figure 56. Administrator Interactive Analytics Graph (Bar Graph / Line Trend Toggle)**  
> **Figure Description:** On adminDashboard.html, scroll to the analytics chart section. Capture the enrollment distribution graph showing headcount across Kindergarten to Grade 6, gender ratio bars (Male vs. Female), and the Bar Graph vs. Line Trend view toggle button.

**Interface Controls & Elements:**

1. **Enrollment Distribution Chart** – Headcount visualization per grade level (Kinder to Grade 6).
2. **Chart View Toggle** – Switch between Bar Graph and Line Trend modes.
3. **Gender Breakdown Legend** – Displays Male (Blue) vs. Female (Pink) enrollment proportions.
4. **Export Chart Graphic Button** – Downloads chart image for school executive reports.

---

### ADMINISTRATOR CLASS SECTIONS & CAPACITY PANEL WITH UNASSIGNED STUDENTS ALERT
**Header:** ADMINISTRATOR DASHBOARD & KPI ANALYTICS  
**Figure 57. Administrator Class Sections & Capacity Panel with Unassigned Students Alert**  
> **Figure Description:** On adminDashboard.html, locate the Section Capacity monitor. Capture the panel showing occupancy progress bars for each section, capacity ratios (e.g., 38/45), and the red "Unassigned Students" alert badge (#unassignedStudentsBadge).

**Interface Controls & Elements:**

1. **Section Capacity Progress Bars** – Visual occupancy meter for each active section.
2. **Unassigned Students Alert Badge (#unassignedStudentsBadge)** – Red counter indicating pupils awaiting sectioning.
3. **Capacity Limit Warning** – Flags sections approaching maximum DepEd class size (45 pupils).
4. **"Assign Sections" Shortcut** – Direct link to the drag-and-drop sectioning workspace.

---

### ADMINISTRATOR OPERATIONS HUB WITH PRIORITY ACTIONS AND LIVE AUDIT STREAM
**Header:** ADMINISTRATOR DASHBOARD & KPI ANALYTICS  
**Figure 58. Administrator Operations Hub with Priority Actions and Live Audit Stream**  
> **Figure Description:** On adminDashboard.html, capture the Operations Hub section (JS/operationsHub.js) showing pending application tasks, document verification alerts, system status indicators, and live audit event stream.

**Interface Controls & Elements:**

1. **Priority Tasks Checklist** – Outstanding applications and document reviews needing attention.
2. **Live Activity Ticker** – Real-time stream of user logins, submissions, and status changes.
3. **System Health Status** – Confirms database, Firebase, mailer, and SMS gateway connectivity.

---

### ADMINISTRATOR APPLICATIONS MANAGEMENT HUB – NEW APPLICATIONS TAB
**Header:** APPLICATIONS & ENROLLMENT MANAGEMENT  
**Figure 59. Administrator Applications Management Hub – New Applications Tab**  
> **Figure Description:** Navigate to applications.html under the "New Applications" tab (#newApplicationsTab). Capture the filter tabs (All #totalCount, Pending #pendingCount, Approved #approveCount, Enrolled #enrolledCount), search input (#searchInput), grade filter (#gradeFilter), applications table (#applicationsTable), and "Review" buttons.

**Interface Controls & Elements:**

1. **Status Filter Tabs** – Filter by All (#totalCount), Pending (#pendingCount), Approved (#approveCount), Enrolled (#enrolledCount).
2. **Universal Search Input (#searchInput)** – Filter by student name, tracking reference number, or LRN.
3. **Grade Level Dropdown (#gradeFilter)** – Filter applications by target grade (Kindergarten to Grade 6).
4. **Applications Data Table (#applicationsTable)** – Columns for Applicant Name, Grade, Date Filed, Status.
5. **"Review" Action Button** – Launches comprehensive applicant dossier modal (#actionModal).

---

### ADMINISTRATOR COMPREHENSIVE APPLICATION DOSSIER EVALUATION MODAL
**Header:** APPLICATIONS & ENROLLMENT MANAGEMENT  
**Figure 60. Administrator Comprehensive Application Dossier Evaluation Modal**  
> **Figure Description:** On applications.html, click "Review" on any applicant row to launch #actionModal. Capture the modal displaying student personal info, uploaded documents preview drawer, "Approve for Verification" button (#approveBtn), "Enroll" button (#enrollBtn), and "Reject / Return" action buttons.

**Interface Controls & Elements:**

1. **Applicant Dossier Header** – Pupil name, tracking reference ID, and target grade level.
2. **Submitted BEEF Profile Viewer** – Full demographic, address, parent, and SNEd details.
3. **Document Verification Drawer** – Inspect uploaded birth certificates and previous report cards.
4. **"Approve for Verification" Action (#approveBtn)** – Clears application for physical document intake.
5. **"Officially Enroll" Action (#enrollBtn)** – Prompts enrollment modal to finalize class enrollment.
6. **"Return for Revision" Action** – Flags deficiencies and dispatches email notification to parent.

---

### ADMINISTRATOR CONTINUING STUDENT RE-ENROLLMENT PROCESSING QUEUE
**Header:** APPLICATIONS & ENROLLMENT MANAGEMENT  
**Figure 61. Administrator Continuing Student Re-Enrollment Processing Queue**  
> **Figure Description:** On applications.html, switch to the "Re-Enrollment" tab (#reEnrollmentTab). Capture the queue showing active school year (#reCurrentSchoolYear), re-enrollment stats (#reStatTotal, #reStatPending, #reStatConfirmed), continuing pupil rows, and bulk approval checkboxes.

**Interface Controls & Elements:**

1. **Re-Enrollment Statistics Bar** – Counters for Total (#reStatTotal), Pending (#reStatPending), Confirmed (#reStatConfirmed).
2. **Continuing Pupil Roster** – Lists continuing learners requesting admission for next school year.
3. **Academic Clearance Indicator** – Verifies learner passed all subjects in previous school year.
4. **Bulk Approval Checkboxes** – Select multiple re-enrollees for simultaneous approval.
5. **"Assign Section" Action** – Directly allocates approved re-enrollees to target grade sections.

---

### ADMINISTRATOR STUDENT YEAR-END PROMOTION AND GRADE 6 GRADUATION WORKSPACE
**Header:** APPLICATIONS & ENROLLMENT MANAGEMENT  
**Figure 62. Administrator Student Year-End Promotion and Grade 6 Graduation Workspace**  
> **Figure Description:** Open the promotion/graduation workspace on applications.html or settings.html. Capture the table showing Grade 6 completers, general averages, honors classifications (With Honors, High Honors, Highest Honors), and "Confirm Graduation" action buttons.

**Interface Controls & Elements:**

1. **Grade 6 Completers Directory** – Roster of graduating learners with final general averages.
2. **Honors Classification Badges** – Identifies With Honors (90–94), High Honors (95–97), Highest Honors (98–100).
3. **"Confirm Graduation" Action Button** – Updates student state to officially Graduated Alumni.
4. **Export Graduation Roster** – Downloads certified graduation directory for division office.

---

### ADMINISTRATOR MASTER DOCUMENT REPOSITORY IN TABLE VIEW AND DOSSIER VIEW
**Header:** DOCUMENT VERIFICATION REPOSITORY  
**Figure 63. Administrator Master Document Repository in Table View and Dossier View**  
> **Figure Description:** Navigate to documents.html. Capture the master document repository showing the Table View / Dossier View toggle (#btnTableView, #btnDossierView), document statistics (#statTotalDocs, #statVerifiedDocs, #statPendingDocs), document type filter (#docTypeFilter), and documents table (#documentsTableBody).

**Interface Controls & Elements:**

1. **View Mode Toggles (#btnTableView, #btnDossierView)** – Switch between tabular spreadsheet view and visual student dossier cards.
2. **Document Summary Stats** – Total (#statTotalDocs), Verified (#statVerifiedDocs), Pending (#statPendingDocs), Action Required (#statActionDocs).
3. **Document Type Filter (#docTypeFilter)** – Filter by PSA Birth Certificate, SF9 Report Card, or Medical Certificate.
4. **Documents Data Table (#documentsTableBody)** – Lists pupil name, document category, upload date, status.
5. **"View Document" Action** – Launches high-resolution document preview lightbox.

---

### ADMINISTRATOR ENHANCED DOCUMENT PREVIEW AND VERIFICATION LIGHTBOX
**Header:** DOCUMENT VERIFICATION REPOSITORY  
**Figure 64. Administrator Enhanced Document Preview and Verification Lightbox**  
> **Figure Description:** On documents.html, click "View" on any document row to launch the verification lightbox. Capture the lightbox displaying an uploaded PSA Birth Certificate with zoom and rotate controls, "Verify Document" button, and "Flag for Re-upload" feedback prompt.

**Interface Controls & Elements:**

1. **Document Preview Canvas** – High-resolution rendering of uploaded credential.
2. **Zoom In / Out & Rotate Controls** – Inspect fine print, registrar seals, and signatures.
3. **"Verify Document" Action Button** – Sets status to Verified, recording admin ID and timestamp.
4. **"Flag for Re-upload" Action Button** – Prompts feedback dialog to notify parent of unreadable file.

---

### ADMINISTRATOR DOCUMENT VERIFICATION SLOT MANAGEMENT AND ATTENDEE ROSTER
**Header:** APPOINTMENT SLOTS MANAGEMENT  
**Figure 65. Administrator Document Verification Slot Management and Attendee Roster**  
> **Figure Description:** Navigate to documentSlots.html. Capture the interface showing the Bookings Tab (#tabBtn-bookings) vs. Slots Tab (#tabBtn-slots), slot statistics (#statTotalSlots, #statActiveSlots, #statTotalBookings), calendar month selector, booked applicants table (#allBookingsTableBody), and "Add New Slot" button.

**Interface Controls & Elements:**

1. **Module Tabs (#tabBtn-bookings, #tabBtn-slots)** – Switch between Attendee Bookings Roster and Slot Capacity Configuration.
2. **Slot Statistics Bar** – Counters for Total Slots (#statTotalSlots), Active Slots (#statActiveSlots), Total Bookings (#statTotalBookings).
3. **Booked Applicants Table (#allBookingsTableBody)** – Lists scheduled applicants, reference IDs, session hours, and status.
4. **"Mark as Attended" Action Button** – Confirms physical document submission upon campus arrival.
5. **"Add Slot" Button (#slotModal)** – Opens modal to create individual intake slots for specific dates.

---

### ADMINISTRATOR BULK SLOT GENERATION MODAL
**Header:** APPOINTMENT SLOTS MANAGEMENT  
**Figure 66. Administrator Bulk Slot Generation Modal**  
> **Figure Description:** On documentSlots.html, click "Bulk Generate Slots" to launch #bulkModal. Capture the modal showing start and end date pickers, Exclude Weekends checkbox, Morning Session capacity input (AM), Afternoon Session capacity input (PM), and "Generate Slots" button.

**Interface Controls & Elements:**

1. **Date Range Pickers** – Define intake period Start Date and End Date.
2. **"Exclude Weekends" Checkbox** – Automatically omits Saturdays and Sundays.
3. **Morning (AM) Capacity Input** – Set maximum appointments per morning session (8:00 AM – 12:00 PM).
4. **Afternoon (PM) Capacity Input** – Set maximum appointments per afternoon session (1:00 PM – 5:00 PM).
5. **"Generate Slots" Action Button** – Commits recurring daily appointment capacity across target date range.

---

### ADMINISTRATOR MASTER STUDENT DATABASE AND FILTERING CONTROLS
**Header:** STUDENT MASTER DATABASE & LRN UPDATE  
**Figure 67. Administrator Master Student Database and Filtering Controls**  
> **Figure Description:** Navigate to students.html. Capture the master student database showing the grade level count pills (#kindergarten-count to #grade6-count), universal search input (#searchInput), grade filter (#gradeFilter), section filter (#sectionFilter), students table (#studentsTable), and row action menus.

**Interface Controls & Elements:**

1. **Grade Level Count Pills** – Headcount badges for Kindergarten, Grade 1 to Grade 6.
2. **Universal Search Box (#searchInput)** – Fast search by 12-digit LRN, student name, or section.
3. **Master Students Table (#studentsTable)** – Columns for Name, LRN, Sex, Grade, Section, Status.
4. **"View Profile" Action Button** – Opens student master profile modal (#viewProfileModal).
5. **"Update LRN" Action Button** – Launches DepEd LRN assignment modal (#updateLrnModal).
6. **"Unlink Account" Action Button** – Triggers guardian detachment modal (#unlinkModal).

---

### ADMINISTRATOR SECTION ASSIGNMENT AND DRAG-AND-DROP MANAGEMENT INTERFACE
**Header:** CLASS SECTION & ADVISER MANAGEMENT  
**Figure 68. Administrator Section Assignment and Drag-and-Drop Management Interface**  
> **Figure Description:** Navigate to sections.html and click the "Assign Students to Sections" tab (#tabBtnAssignStudents). Capture the workspace showing Target Section selector (#sectionViewFilter), publication status banner (#sectionRosterPublishBanner: Draft vs. Published), Unassigned Students pool on left (separated into Male and Female columns with checkboxes), and Section Dropzones on right with capacity indicators (e.g., 18/36) and remove (×) buttons.

**Interface Controls & Elements:**

1. **Target Section Selector (#sectionViewFilter)** – Choose section receiving student assignments.
2. **Publication Status Banner (#sectionRosterPublishBanner)** – Indicates whether assignments are in DRAFT mode or PUBLISHED.
3. **Unassigned Pupils Pool (Left)** – Enrolled pupils separated into Male (Blue) and Female (Pink) columns for gender balancing.
4. **Assigned Section Dropzone (Right)** – Section card displaying current pupils, live gender counts, and capacity progress bar.
5. **Drag-and-Drop & Bulk Assign** – Drag individual pupil cards across panels, or check multiple pupils and click "Bulk Assign".
6. **Unassign Pupil Action (×)** – One-click button to safely return assigned pupil to the unassigned queue.
7. **"Publish Section Roster" Button** – Commits section assignments to official DepEd enrollment records.

---

### ADMINISTRATOR LRN UPDATE AND ACCOUNT UNLINKING MODALS
**Header:** STUDENT MASTER DATABASE & LRN UPDATE  
**Figure 69. Administrator LRN Update and Account Unlinking Modals**  
> **Figure Description:** On students.html, capture a composite view showing #updateLrnModal (displaying student name, current temporary LRN, 12-digit numeric input with green validation indicator, and Save button) alongside #unlinkModal (displaying linked guardian info, 5-second countdown timer, and Confirm Unlink button).

**Interface Controls & Elements:**

1. **DepEd 12-Digit LRN Input (#updateLrnModal)** – Input restricted strictly to 12 digits with real-time DepEd format validation.
2. **LRN Validation Indicator** – Turns green when exactly 12 valid digits are entered.
3. **"Save LRN" Button** – Permanently updates learner record in students table.
4. **Linked Guardian Info (#unlinkModal)** – Displays guardian name, email, and original binding date.
5. **5-Second Safety Lock Timer** – Disables confirmation button for 5 seconds to prevent accidental unlinking.
6. **"Confirm Unlink" Button** – Enables after countdown; detaches guardian account and logs security audit trail.

---

### ADMINISTRATOR SECTION MANAGEMENT AND CLASS ADVISER ASSIGNMENT INTERFACE
**Header:** CLASS SECTION & ADVISER MANAGEMENT  
**Figure 70. Administrator Section Management and Class Adviser Assignment Interface**  
> **Figure Description:** Navigate to sections.html under the "Manage Sections" tab (#tabBtnManageSections). Capture the section cards grid (#sectionsGrid), grade level filter (#gradeLevelFilter), section details (Section Name, Room Number, Capacity bar, Class Adviser dropdown), and "Create New Section" modal (#sectionModal).

**Interface Controls & Elements:**

1. **"Create Section" Action Button** – Opens #sectionModal to register a new grade section.
2. **Grade Level Filter Bar (#gradeLevelFilter)** – Filter sections by Kindergarten, Primary (Grades 1–3), or Intermediate (Grades 4–6).
3. **Section Information Cards (#sectionsGrid)** – Displays Grade & Section Name, Room Location, and Maximum Capacity.
4. **Class Adviser Dropdown** – Assigns official homeroom faculty adviser.
5. **Capacity Progress Bar** – Color-coded occupancy meter (Green: Open slots; Red: Full section at 45 pupils).
6. **Edit / Archive Actions** – Modify room and adviser settings, or safely archive section.

---

### ADMINISTRATOR DEPED ELEMENTARY SUBJECT CURRICULUM MANAGEMENT
**Header:** CURRICULUM & SUBJECT MANAGEMENT  
**Figure 71. Administrator DepEd Elementary Subject Curriculum Management**  
> **Figure Description:** Navigate to subjectManagement.html. Capture the interface showing the Active Curriculum tab (#tabActive) vs. Archived Subjects tab (#tabArchived), grade level filter (#gradeLevelFilter), subject cards with Subject Code and Units, and the "Add Subject" modal (#subjectModal).

**Interface Controls & Elements:**

1. **Curriculum View Tabs (#tabActive, #tabArchived)** – Toggle between Active Curriculum Subjects and Archived Subjects.
2. **Grade Level Filter Bar (#gradeLevelFilter)** – Filter learning areas by elementary grade level.
3. **"Add Subject" Action Button** – Opens #subjectModal to register a DepEd curriculum subject.
4. **Subject Modal Form Fields** – Subject Name (#subjectName), Subject Code (#subjectCode), Grade Level (#gradeLevel), Units (#subjectUnits).
5. **"Archive Subject" Action Button** – Deactivates subject without deleting historical grade records.
6. **"Restore Subject" Action Button** – Restores previously archived subjects back to active curriculum status.

---

### ADMINISTRATOR FACULTY AND TEACHER MANAGEMENT DIRECTORY WITH CLUSTER FILTERS
**Header:** FACULTY & TEACHER DIRECTORY  
**Figure 72. Administrator Faculty and Teacher Management Directory with Cluster Filters**  
> **Figure Description:** Navigate to teacherManagement.html. Capture the faculty directory showing the cluster filter pills (#clusterPillAll, #clusterPillKinder, #clusterPillPrimary, #clusterPillIntermediate), teacher search input (#searchInput), teacher profile cards (#teachersTableBody), and "Add New Teacher" modal (#teacherModal).

**Interface Controls & Elements:**

1. **Faculty Cluster Filter Pills** – Filter by All Faculty, Kindergarten, Primary (Grades 1–3), or Intermediate (Grades 4–6).
2. **"Add New Teacher" Action Button (#addTeacherBtn)** – Opens modal to provision an existing user account as faculty.
3. **Teacher User Account Dropdown (#teacherAccount)** – Select authenticated user from system user directory.
4. **Grade Cluster & Specialization Selectors** – Configure handled grade cluster and subject specialization.
5. **Faculty Profile Cards (#teachersTableBody)** – Displays teacher avatar, employee ID, specialization, and advisory section.
6. **"View Timetable" Action Button** – Launches large teacher timetable modal (#largeTeacherTimetableModal).

---

### ADMINISTRATOR FACULTY MASTER TIMETABLE INSPECTION MODAL
**Header:** FACULTY & TEACHER DIRECTORY  
**Figure 73. Administrator Faculty Master Timetable Inspection Modal**  
> **Figure Description:** On teacherManagement.html, click "View Timetable" on any teacher card to launch #largeTeacherTimetableModal. Capture the modal displaying the teacher identification header, the 5-day weekly schedule grid (Monday to Friday, 7:00 AM–5:00 PM), subject blocks with section labels, and the "Print Timetable" button.

**Interface Controls & Elements:**

1. **Teacher Identification Header** – Displays teacher full name, employee number, specialization, and total teaching minutes.
2. **Weekly Timetable Grid** – 5-column calendar grid (Monday to Friday, 7:00 AM–5:00 PM).
3. **Scheduled Class Blocks** – Color-coded subject blocks displaying subject title, grade & section, and classroom.
4. **Advisory Homeroom Highlight** – Highlights periods where teacher acts as homeroom class adviser.
5. **"Print Timetable" Action Button** – Formats weekly schedule into official individual SF7 teaching program PDF.

---

### ADMINISTRATOR TIMETABLE BUILDER – MASTER CLASS SCHEDULES OVERVIEW
**Header:** CLASS SCHEDULES & TIMETABLE BUILDER  
**Figure 74. Administrator Timetable Builder – Master Class Schedules Overview**  
> **Figure Description:** Navigate to scheduleManagement.html under the "Master Class Schedules" tab (#tabBtnMasterSectionsCalendar). Capture the interface showing the Schedule Publication Status Banner (#masterSchedPublishBanner: Draft vs. Published), Grade Level filter (#masterSchedGradeFilter), section search input (#masterSchedSectionSearch), and Section Schedule Cards grid (#masterSectionSchedulesGrid).

**Interface Controls & Elements:**

1. **Master Schedules Tab (#tabBtnMasterSectionsCalendar)** – Default overview of complete weekly timetables across all grade sections.
2. **Publication Status Ribbon (#masterSchedPublishBanner)** – Toggle to publish schedules school-wide or keep in draft mode.
3. **Grade Level Filter (#masterSchedGradeFilter)** – Filter section cards by Kindergarten or Grades 1 to 6.
4. **Section Search Box (#masterSchedSectionSearch)** – Instant search by section name.
5. **Section Schedule Cards (#masterSectionSchedulesGrid)** – Summarizes weekly subject load, total minutes, and publication status.
6. **"Switch to Schedule Builder" Action (#tabBtnScheduleEditor)** – Transitions to interactive schedule editor.

---

### ADMINISTRATOR TIMETABLE SESSION CREATOR WITH AUTOMATED CONFLICT DETECTION ENGINE
**Header:** CLASS SCHEDULES & TIMETABLE BUILDER  
**Figure 75. Administrator Timetable Session Creator with Automated Conflict Detection Engine**  
> **Figure Description:** On scheduleManagement.html, switch to the "Class Schedule Builder" tab (#tabBtnScheduleEditor). Capture the dual-panel interface showing the Left Panel session creator form (#createForm: Section, Subject, Teacher, Start Time, Duration in minutes, Day of week checkboxes, Room), the Right Panel 5-day weekly timetable grid, and the Collision Warning Modal flashing when an overlap occurs.

**Interface Controls & Elements:**

1. **Target Section Selector** – Choose section being scheduled (e.g., Grade 4 - Mabini).
2. **Create Session Form (#createForm)** – Configure Subject, Assigned Teacher, Start Time, Duration (min), Days, and Room.
3. **Real-Time Automated Conflict Detection Engine** – Instantly detects if teacher, section, or room is double-booked.
4. **Collision Warning Alert Modal** – Red modal blocking entry if a scheduling overlap occurs, specifying conflicting section and teacher.
5. **Interactive Weekly Grid** – 5-day visual schedule grid; click any block to edit or delete.
6. **"Auto-Fill Missing Schedules" Button** – Automatically populates timetable gaps based on DepEd curriculum time allocations.
7. **"Auto-Assign Teachers" Button** – Intelligently assigns qualified teachers based on cluster specializations.
8. **"Save Schedule" Action Button** – Commits finalized section timetable to database.

---

### ADMINISTRATOR USER ACCOUNT MANAGEMENT AND STAFF CREATION MODAL
**Header:** USER MANAGEMENT & SECURITY ROLES  
**Figure 76. Administrator User Account Management and Staff Creation Modal**  
> **Figure Description:** Navigate to users.html. Capture the user management interface showing the role filter pills (All, Admin #adminCount, Teacher #teacherCount, Student #studentCount), user search box (#searchInput), user accounts table (#usersTable) with active/suspended toggles, and "Add User" modal (#addUserModal).

**Interface Controls & Elements:**

1. **Role Filter Pills** – Categorize accounts: All (#totalUsers), Admin (#adminCount), Teacher (#teacherCount), Student (#studentCount).
2. **Universal User Search (#searchInput)** – Lookup accounts by display name, email address, or user ID.
3. **User Accounts Data Table (#usersTable)** – Columns for Avatar, Full Name, Email, Role, Creation Date, Status.
4. **"Add User" Action Button (#addUserModal)** – Opens modal to provision a staff/teacher account with temporary password.
5. **Account Status Toggle Switch** – Instant toggle to activate or suspend user login credentials.
6. **"Reset Password" Action Button** – Dispatches official password reset email to user.

---

### ADMINISTRATOR USER ROLE MODIFICATION DIALOG WITH DEMOTION SAFEGUARDS
**Header:** USER MANAGEMENT & SECURITY ROLES  
**Figure 77. Administrator User Role Modification Dialog with Demotion Safeguards**  
> **Figure Description:** On users.html, click "Edit Role" on any user row to launch #editRoleModal. Capture the role modification dialog showing target user details (#editRoleUserInfo), role assignment dropdown (#newRole: Administrator, Teacher, Student/Parent), administrator demotion safeguard warning, and "Save Role Changes" button.

**Interface Controls & Elements:**

1. **Target User Profile Card (#editRoleUserInfo)** – Displays user display name, registered email, and current role.
2. **Role Assignment Dropdown (#newRole)** – Select new system role (Administrator, Teacher, or Student/Parent).
3. **Demotion Safeguard Check** – Automated rule preventing demoting the last remaining active administrator.
4. **"Save Role Changes" Action Button** – Commits role designation and updates session security claims.

---

### ADMINISTRATOR ANNOUNCEMENTS MANAGEMENT HUB AND CATEGORY TAGGING
**Header:** ANNOUNCEMENTS & FACEBOOK SYNC  
**Figure 78. Administrator Announcements Management Hub and Category Tagging**  
> **Figure Description:** Navigate to announcements.html. Capture the announcements hub showing status tabs (Published #tabPublished, Pending Review #tabPending, Archived #tabArchived), priority pinned bulletins, and the "Create Announcement" modal (#createAnnouncementModal) active with Title (#annTitle), Category (#annCategory), Target Audience, Content editor, Priority Pinning toggle, and Auto-Post to Facebook toggle (#postToFacebook).

**Interface Controls & Elements:**

1. **"Create Announcement" Action Button** – Opens modal to draft a new school bulletin.
2. **Title & Category Selectors (#annTitle, #annCategory)** – Enter headline and category (General Advisory, Academic News, Emergency Suspension, DepEd Memo).
3. **Target Audience Radios** – Target bulletin to Public, Enrolled Students & Parents, or Faculty Only.
4. **Priority Pinning Toggle** – Pins urgent advisory to top of public feed with a high-priority red badge.
5. **Auto-Post to Facebook Toggle (#postToFacebook)** – Synchronizes announcement simultaneously to the official VPES Facebook Page.
6. **"Publish Announcement" Action Button** – Broadcasts advisory across selected channels.

---

### ADMINISTRATOR FACEBOOK SYNCED POST REVIEW AND APPROVAL TWO-COLUMN LIGHTBOX
**Header:** ANNOUNCEMENTS & FACEBOOK SYNC  
**Figure 79. Administrator Facebook Synced Post Review and Approval Two-Column Lightbox**  
> **Figure Description:** On announcements.html, switch to the "Pending Review" tab (#tabPending) and click "Review" on an incoming Facebook post to launch #reviewModal. Capture the two-column lightbox showing the raw Facebook post and photo on the left panel, and portal category and formatting controls on the right panel.

**Interface Controls & Elements:**

1. **"Pending Review" Tab (#tabPending)** – Queue of incoming Facebook Page posts captured via webhook.
2. **Facebook Source Panel (Left)** – Displays raw post content, original publishing timestamp, and attached photos.
3. **Portal Formatting Panel (Right)** – Customize headline, select portal category, and adjust visibility.
4. **"Approve & Publish to Portal" Button** – Approves post and publishes it directly to the public landing page feed.
5. **"Dismiss / Reject Post" Button** – Removes post from review queue without publishing to portal.

---

### ADMINISTRATOR SYSTEM AUDIT AND ACTIVITY LOGS INTERFACE
**Header:** SYSTEM AUDIT & SECURITY LOGS  
**Figure 80. Administrator System Audit and Activity Logs Interface**  
> **Figure Description:** Navigate to auditLogs.html. Capture the audit logs interface showing the 5 KPI summary cards (#statTotalLogs, #statTodayLogs, #statReEnrollLogs, #statAdmissionsLogs, #statSecurityLogs), category filter pills, date range filter dropdown (#auditDateFilter), search box (#auditSearchInput), audit trail data table (#auditTableBody), and row-click Audit Event Detail modal (#auditDetailModal).

**Interface Controls & Elements:**

1. **Top KPI Summary Cards** – Total Logs (#statTotalLogs), Actions Today (#statTodayLogs), Re-Enrollments (#statReEnrollLogs), Admissions (#statAdmissionsLogs), Security (#statSecurityLogs).
2. **Universal Search Box (#auditSearchInput)** – Real-time search by student name, 12-digit LRN, administrator name, or event description.
3. **Category Quick-Filter Pills** – Filter stream by All Logs, Re-Enrollment, Admissions, Documents, Users & Security, Sections & Schedules, System Settings.
4. **Date Range Filter Dropdown (#auditDateFilter)** – Preset ranges (All Time, Today, Yesterday, Last 7/30 Days, Custom Date Range).
5. **Audit Trail Data Table (#auditTableBody)** – Columns for Date & Time, Event Action (with category badge), Description & Details, Performed By.
6. **Audit Event Detail Modal (#auditDetailModal)** – Click any row to inspect programmatic action code, timestamp, performer email, description, and application ref.
7. **"Refresh Logs" Action Button (#btnRefreshLogs)** – Polls for newly recorded events without reloading the page.

---

### ADMINISTRATOR SCHOOL YEAR MANAGEMENT AND ACTIVATION READINESS AUDIT MODAL
**Header:** SYSTEM SETTINGS & ADMISSION GATING  
**Figure 81. Administrator School Year Management and Activation Readiness Audit Modal**  
> **Figure Description:** Navigate to settings.html under the "School Year" tab (#schoolYearTab). Capture the active school year banner (#activeSchoolYearText), historical school years table, "Add School Year" modal, "Check Activation Readiness" button, and the Activation Readiness Audit modal displaying the verification checklist (grades, promotions, sections).

**Interface Controls & Elements:**

1. **Active School Year Display Banner (#activeSchoolYearText)** – Identifies currently active DepEd term (e.g., S.Y. 2026–2027).
2. **"Add School Year" Action Button** – Opens dialog to create new academic year with start and end dates.
3. **Historical School Years Table** – Archive of past academic terms and enrollment totals.
4. **"Check Activation Readiness" Action Button** – Runs automated institutional audit of 4th-quarter grades and promotions.
5. **Readiness Checklist & Resolution Modal** – Itemizes missing grades; enables "Activate School Year" button once resolved.

---

### ADMINISTRATOR INDEPENDENT ADMISSION GATING SWITCHES (EARLY REG, ENROLLMENT, RE-ENROLLMENT)
**Header:** SYSTEM SETTINGS & ADMISSION GATING  
**Figure 82. Administrator Independent Admission Gating Switches (Early Reg, Enrollment, Re-Enrollment)**  
> **Figure Description:** On settings.html, locate the three admission gating cards. Capture the interface showing the independent toggle switches for Early Registration (#toggleEarlyRegBtn), Official General Enrollment (#toggleEnrollmentBtn), and Re-Enrollment (#toggleReEnrollmentBtn), scheduled calendar date pickers, and public closed advisory textboxes.

**Interface Controls & Elements:**

1. **Early Registration Gating Switch (#toggleEarlyRegBtn)** – Toggles pre-registration ON/OFF for Kindergarten and Grade 1.
2. **Official General Enrollment Switch (#toggleEnrollmentBtn)** – Toggles general admission ON/OFF for all grade levels across public portal.
3. **Student Re-Enrollment Gating Switch (#toggleReEnrollmentBtn)** – Controls whether re-enrollment tab is active on student dashboard.
4. **Scheduled Calendar Date Pickers** – Sets automated opening and closing calendar dates for admission forms.
5. **Public Closed Advisory Textbox** – Customizes advisory message displayed on public portal when enrollment is closed.

---

### ADMINISTRATOR SCHOOL INSTITUTIONAL PROFILE AND DEPED IDENTIFIERS CONFIGURATION
**Header:** SYSTEM SETTINGS & ADMISSION GATING  
**Figure 83. Administrator School Institutional Profile and DepEd Identifiers Configuration**  
> **Figure Description:** On settings.html, switch to the "School Profile" tab. Capture the official DepEd Institutional Profile form showing School Name (Vinzons Pilot Elementary School), DepEd ID (112937), Principal Name, Division (Camarines Norte), Region (Region V - Bicol), School Seal uploader, and Save button.

**Interface Controls & Elements:**

1. **DepEd School ID Field** – Configured official institutional identifier (112937).
2. **Official School Name Field** – Vinzons Pilot Elementary School.
3. **Administrative Identifiers** – Principal / Head Teacher name, Division (Camarines Norte), and Region (Region V - Bicol).
4. **Official School Seal Uploader** – Uploads high-resolution school logo rendered on report cards and official certificates.
5. **Public Contact Details** – Configures public office email, phone numbers, and official Facebook Page URL.
6. **"Save Profile" Action Button** – Commits institutional data across all report headers.

---

### ADMINISTRATOR LANDING PAGE CONTENT MANAGEMENT SYSTEM (CMS) WITH LIVE PREVIEW
**Header:** SYSTEM SETTINGS & ADMISSION GATING  
**Figure 84. Administrator Landing Page Content Management System (CMS) with Live Preview**  
> **Figure Description:** On settings.html, switch to the CMS tab. Capture the landing page editor showing hero headline editor, announcement card toggles, DepEd core values editor, photo gallery uploader, and the side-by-side live preview canvas iframe.

**Interface Controls & Elements:**

1. **Hero Headline & Subtitle Editor** – Customizes main banner headlines on landing page.
2. **Core Values & Programs Editor** – Updates text for Maka-Diyos, Makatao, Makakalikasan, Makabansa.
3. **Campus Facilities Photo Gallery** – Uploads photographs displayed on public portal.
4. **Live Preview Canvas Iframe** – Real-time preview displaying how edits look before publishing.
5. **"Save & Publish CMS" Button** – Commits content changes to public website.

---

### ADMINISTRATOR SCHOOL FORMS & OFFICIAL REPORTS CENTER
**Header:** SCHOOL FORMS & OFFICIAL REPORTS CENTER  
**Figure 85. Administrator School Forms & Official Reports Center**  
> **Figure Description:** Navigate to academicRecords.html. Capture the School Forms & Official Reports Center catalog showing the four active DepEd report cards: SF4 (Monthly Movement), SF6 (Promotion Summary), SF7 (Personnel Assignment), SF10-ES (Permanent Record), and the live PDF viewer modal (#sf10ModalOverlay) with "Download PDF" and "Download Excel (.xlsx)" buttons.

**Interface Controls & Elements:**

1. **Reports Catalog Header** – Displays "School Forms & Official Reports Center" with a live Refresh button.
2. **SF4: Monthly Learner Movement Card** – "View & Download SF4" button launches live modal showing monthly attendance matrix.
3. **SF6: Promotion & Proficiency Summary Card** – "View & Download SF6" button launches live modal showing Form 20 matrix.
4. **SF7: School Personnel Assignment List Card** – "View & Download SF7" button launches live modal showing faculty plantilla.
5. **SF10-ES: Permanent Academic Record Card** – "Open SF10 Generator" button launches Form 137 workspace (#workspace-sf10).
6. **Official PDF Viewer Modal (#sf10ModalOverlay)** – Embedded viewer with direct "Download PDF" and "Download Excel (.xlsx)" buttons.

---

### ADMINISTRATOR BULK STUDENT CSV IMPORT INTERFACE
**Header:** ADMINISTRATIVE UTILITIES & EXPORTS  
**Figure 86. Administrator Bulk Student CSV Import Interface**  
> **Figure Description:** Navigate to importStudents.html. Capture the bulk student CSV import interface showing the drag-and-drop CSV upload zone (#uploadArea), file input (#fileInput), CSV header format instructions (lrn, last_name, first_name, gender, birth_date), validation progress bar (#progressBar, #progressFill), and "Import Students" button (#importBtn).

**Interface Controls & Elements:**

1. **CSV Drag-and-Drop Zone (#uploadArea)** – Drop zone accepting official DepEd learner CSV files.
2. **CSV Header Format Guide** – Details required columns: lrn, last_name, first_name, gender, birth_date.
3. **Validation Progress Bar (#progressBar, #progressFill)** – Validates duplicate LRNs and reports formatting errors.
4. **"Import Students" Action Button (#importBtn)** – Commits validated student records into students table.

---

### OFFICIAL LIST OF ENROLLEES CERTIFICATE-STYLE PRINT PREVIEW TEMPLATE
**Header:** ADMINISTRATIVE UTILITIES & EXPORTS  
**Figure 87. Official List of Enrollees Certificate-Style Print Preview Template**  
> **Figure Description:** Navigate to preview_enrollees_template.html. Capture the ceremonial Official List of Enrollees template (#sheetPreview) showing the formal DepEd Region V & Division of Camarines Norte header, ornamental border, Grade & Section title (#previewGradeSection), enrolled pupil roster (#rosterTbody), Boys/Girls/Total counts, School Principal certification block, and print button.

**Interface Controls & Elements:**

1. **Ceremonial DepEd Header** – Republic of the Philippines, DepEd Region V, Division of Camarines Norte.
2. **Ornamental Frame Border** – Formal certificate border suitable for superintendent presentation.
3. **Certified Enrollee Directory (#rosterTbody)** – Itemized list of enrolled learners with LRN, Sex, and Section.
4. **Gender Count Summary** – Summary tallies for Boys (#previewBoysCount), Girls (#previewGirlsCount), Total (#previewTotalCount).
5. **Principal Certification Block** – Official signature and date line for School Principal.
6. **"Print Document" Action Button** – Formats ceremonial certificate for high-resolution printing.

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
