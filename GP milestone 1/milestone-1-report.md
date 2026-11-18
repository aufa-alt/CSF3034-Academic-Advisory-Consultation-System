# GP Milestone 1: Requirements and Use Case Model

## 1. Project Background

### 1.1 Problem Statement and Justification
In a university environment, students frequently need to consult their lecturers to discuss academic matters such as understanding lecture topics, completing assignments, discussing coursework, and preparing for examinations. However, arranging consultation sessions between students and lecturers can sometimes be challenging due to scheduling conflicts, limited communication, and difficulties in identifying lecturer's available consultation hours. 

Furthermore, students may make a mistake by setting a time with their lecturer during their scheduled classes or other academic activities. This can lead to time conflicts, missed consultation opportunities, and inefficient time management. Students may also face difficulties identifying which lecturers teach their registered subjects or who their assigned academic mentors are when they need academic guidance. 

One of the main problems about setting an appointment with their lecturer is searching for a time that matches both students' and lecturers' schedules since both have different timetables and free time. Students may approach lecturers through informal communication methods such as WhatsApp messages, Telegram, or face-to-face discussions to request consultation sessions. However, these methods do not allow students to check lecturers' availability. As a result, students may experience difficulties finding suitable consultation times, while lecturers may receive multiple appointment requests that overlap with their existing schedules. 

Therefore, the proposed Student-Lecturer Consultation Booking System is introduced to overcome these problems by providing a centralized and systematic platform for managing consultation appointments. The system objectives are to simplify the appointment booking process, improve communication between students and lecturers, reduce scheduling conflicts, and ensure that consultation sessions can be arranged more efficiently. 

### 1.2 Proposed System Overview
The proposed Student-Lecturer Consultation Booking System is a web-based system designed to facilitate and organize consultation appointments between university students and lecturers. The system provides a centralized platform that allows students to identify their assigned lecturers and academic mentors, check lecturer consultation availability, and request appointments based on suitable time slots. 

When students access the system for the first time, they are required to register by providing their personal academic information, such as student ID, full name, and programme. After successfully logging in, the system will display their personal profiles, a list of lecturers who teach their registered subjects, and their mentor. 

Students can select a lecturer from the displayed list that they want to book an appointment with. Then, they can view the lecturer’s information, including the lecturer’s name, subjects taught, and consultation timetable. The timetable will indicate available and unavailable time slots, allowing students to identify suitable consultation sessions. Students can select an available time slot based on their preferred date and time, if it does not conflict with their scheduled classes. 

After selecting a suitable time slot, students are required to provide the purpose of their consultation. The system will display the selected appointment details for confirmation before the request is submitted to the lecturer. 

Unlike an automatic booking system, it uses a lecturer approval process. Once a student submits an appointment request, the request will be sent to the selected lecturer for review. The appointment status will initially be displayed as "Pending". The lecturer can then approve or reject the request based on their availability and schedule. 

If the lecturer approves the request, the appointment status will change to "Approved", and the lecturer’s consultation timetable will be updated automatically. The selected time slot will become unavailable to prevent other students from booking the same time. However, if the lecturer rejects the request, the appointment status will change to "Rejected", and the selected time slot will become available again.

### 1.3 Project Planning (Roles, GitHub & Timeline)
Project planning is an important part of the software development process to make sure that the project is completed systematically. It involves assigning responsibilities to team members, managing project activities through GitHub, and preparing a timeline to monitor the progress of the project. 

#### Roles and Responsibilities
Each team member will be assigned specific roles and responsibilities to ensure that all project activities are completed effectively. The distribution of tasks will encourage teamwork, improve coordination, and ensure that every member contributes to the development of the Student-Lecturer Consultation Booking System. 

| Team Member | Position | Responsibilities |
| :--- | :--- | :--- |
| **Muhammad Fitri Bin Asmadi** (S88487) | Team Leader | Coordinate team activities, distribute tasks, monitor project progress and ensure deadlines are met. |
| **Nur Amalin Aisyah Binti Rosdi** (S87402) | System Analyst and Documentation | Analyse the system requirements, prepare project documentation, and ensure the system meets its objective. |
| **Aufa Nazuha Binti Mohd Nazri** (S85139) | UI/UX Designer | Design the system interface including student dashboard, lecturer profiles and appointment booking pages. |
| **Ahmad Ihab Halim Bin Mohd Zamani** (S87287) | Developer and Testing | Develop system functions, implement appointment booking features, and conduct system testing. |

#### Team Members Biography
* **Muhammad Fitri Bin Asmadi (S88487 - Team Leader):** Pursuing Computer Science. Responsible for coordinating team activities, managing project progress, and ensuring that all assigned tasks are completed according to the project timeline.
* **Nur Amalin Aisyah Binti Rosdi (S87402 - System Analyst and Documentation):** Pursuing Computer Science. Responsible for analyzing system requirements, preparing project documentation, and ensuring the system meets its objectives.
* **Aufa Nazuha Binti Mohd Nazri (S85139 - UI/UX Designer):** Pursuing Computer Science. Responsible for designing the system interface including the student dashboard, lecturer profiles, and appointment booking pages.
* **Ahmad Ihab Halim Bin Mohd Zamani (S87287 - Developer and Testing):** Pursuing Computer Science. Responsible for developing system functions, implementing appointment booking features, and conducting system testing.

#### GitHub Activity Details
GitHub is used as a collaborative platform to manage and monitor development activities. It allows team members to share project files, manage source code, track changes, and collaborate throughout the software development process.

* Repository Link: `https://github.com/aufa-alt/CSF3034-Academic-Advisory-Consultation-System.git`

#### Project Timeline
| No. | Project Activities | Estimated Duration |
| :--- | :--- | :--- |
| 1. | Project Selection and Planning | 22 October 2026 |
| 2. | Project Background, Problem Statement and Requirement Gathering | 27 October 2026 |
| 3. | Milestone 1 : Requirements and Use Case Model | 5 November 2026 |
| 4. | Review Requirements and Prepare System Design | 7 November 2026 |
| 5. | Milestone 2 : System Design | 19 November 2026 |
| 6. | Database and User Interface Development | 30 November 2026 |
| 7. | Student Module Development (Student Profile and Appointment Booking) | 5 December 2026 |
| 8. | Lecturer Module Development (Lecturer Schedule and Appointment Approval) | 10 December 2026 |
| 9. | System Integration, Testing and Debugging | 15 December 2026 |
| 10. | Submission of Final Report | 24 December 2026 |
| 11. | Final Presentation Preparation | 30 December 2026 |
| 12. | Final Project Presentation | 3-7 January 2027 |

---

## 2.0 System Requirements

### 2.1 Stakeholder Identification & Requirement Gathering
Before designing the Academic Advisory & Consultation System, our team gathered feedback directly from people involved in the daily consultation process on campus. Relying purely on our own assumptions would risk overlooking real scheduling habits, so we focused on three main stakeholder groups:
* **Undergraduate Students (Primary Users):** Students who regularly need academic advising, course registration help, or guidance from their lecturers.
* **Academic Lecturers (Secondary Users):** Faculty members who balance teaching hours, research, meetings, and student consultation slots throughout the week.
* **System Administrator:** Team leader responsible for maintaining user accounts, managing database health, and handling access permissions.

To understand what these users actually deal with, we used two requirements-gathering methods:
* **Short interviews:** We spoke with several lecturers from the Faculty of Computer Science and Mathematics to ask how they currently handle student appointments. Most shared that managing ad-hoc walk-ins alongside scattered messages on WhatsApp and email often leads to double-booked times or missed appointments.
* **Student Questionnaire:** We shared a quick survey with fellow UMT students to learn about their experiences booking consultations. A recurring frustration was walking all the way to the lecturer’s office only to find they were in a meeting or out of the office.

### 2.2 Functional Requirements
Functional requirements describe specific actions the system must perform. These requirements are grouped into four main modules:

* **Module 1: User Authentication & Profile Management**
  * **FR1.1:** Users (students, lecturers, and administrators) must be able to register and log in using their official university email and password.
  * **FR1.2:** Upon logging in, the system will recognize the user’s role and direct them to their matching workspace (Students Dashboard, Lecturer Dashboard, or Admin Panel).
  * **FR1.3:** Users must be able to view and update their basic profile details and reset forgotten passwords securely.

* **Module 2: Lecturer Schedule & Availability Management**
  * **FR2.1:** Lecturers must be able to set up, edit, and update their weekly consultation hours alongside their regular class schedule.
  * **FR2.2:** Lecturers must be able to customize consultation durations and block off specific dates or times when they are unavailable.
  * **FR2.3:** Whenever a slot is booked, cancelled, or blocked, the system must immediately update its status on the timetable ("Available", "Booked", or "Unavailable").

* **Module 3: Real-Time Slot Checking & Consultation Booking**
  * **FR3.1:** Students must be able to search for a lecturer by name, department, or course code to view their consultation schedule.
  * **FR3.2:** When clicking on an open slot, students must be able to fill in a brief reason for the consultation and confirm their booking in one step.
  * **FR3.3:** Once a student confirms a booking, the system must immediately lock that slot so another student cannot accidentally book the same time.

* **Module 4: Appointment Tracking & Notifications**
  * **FR4.1:** Both students and lecturers must have access to an appointment history page showing upcoming, completed, and cancelled consultations.
  * **FR4.2:** Students and lecturers must be able to cancel or reschedule an upcoming consultation, which automatically reopens that slot on the lecturer’s schedule.
  * **FR4.3:** The system must display clear on-screen alerts and status updates whenever a booking is confirmed, changed, or cancelled.

### 2.3 Non-Functional Requirements
| ID | Category | Description |
| :--- | :--- | :--- |
| **NFR1** | Performance | Lecturer schedules and booking confirmation should load within 2 seconds under normal campus Wi-Fi or mobile data connections. |
| **NFR2** | Usability | The layout should be clean and straightforward on both laptops and mobile browsers, allowing quick navigation. |
| **NFR3** | Reliability & Availability | The platform should stay accessible at least 99.99% of the time during active academic weeks. |
| **NFR4** | Security & Privacy | User passwords must be encrypted in the database, and inactive login sessions should time out automatically. |
| **NFR5** | Data Accuracy | If two students click the exact same time slot at the same second, the database must process only the first request. |
| **NFR6** | Maintainability | The source code should be neatly organized into separate modules and tracked on GitHub. |

### 2.4 Quality & Completeness of Requirements
* **Clear Traceability:** Every functional requirement connects directly to actors and actions shown in the Use Case Diagram and UI wireframes.
* **Verifiable Outcomes:** Each requirement describes a concrete action that can be tested later.
* **Clear Role Boundaries:** Student actions and lecturer controls are kept separate to avoid confusion.
