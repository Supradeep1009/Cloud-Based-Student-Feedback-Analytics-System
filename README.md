Cloud-Based Student Feedback Analytics System

<div align="center">
Show Image
Show Image
Show Image
Show Image
Show Image

<br/>
A cloud-powered system that collects student feedback through a web form, stores responses in real time on Google Cloud Firestore, and delivers actionable faculty performance insights through an interactive Power BI dashboard.

<br/>
Live Feedback Form  ·  View Power BI Dashboard

</div>

About The Project

In most universities, collecting and acting on student feedback is a slow, manual process. Forms get printed, collected, and often never properly analyzed. This project changes that.

Students fill out a simple web form — sharing how they feel about their faculty's teaching style, interaction quality, language of instruction, and overall performance. The moment they hit submit, their response is saved instantly to Google Cloud Firestore. From there, the data is automatically pulled into Google Sheets and visualized in a live Power BI dashboard — giving faculty coordinators a clear, real-time view of how each professor is performing across different subjects.

The goal is simple: make student voices count, and make faculty improvement measurable.


Built as part of a Cloud Computing project at KL University (2026), this system demonstrates a complete end-to-end data pipeline — from a student clicking "Submit" to a coordinator reading insights on a dashboard.




Live Dashboard

Explore the fully interactive Power BI report here:

Open Power BI Dashboard

Show Image

What the Dashboard Shows

VisualInsightSum of Rating by FacultyDr. Nilu Sing leads with 28.57% of total ratingsCount of Interaction by FacultyDr. Leena Arya has the highest student interaction (4)Faculty & Rating by SubjectCovers Cloud Security, Data Analytics, Network Infrastructure & Software ValidationLanguage Preference76.92% of students prefer Telugu; rest prefer English or HindiTeaching Style BreakdownPer-subject analysis at ratings 3, 4, and 5 across all faculty


Backend — Google Cloud Firestore

Every student submission is stored as a document inside the feedbacks collection in real time.

Show Image

Each document captures:

FieldExamplenameHussainrollNumber2300039032facultyDr. Nilu SingsubjectData Analytics and VisualizationoverallRating4interactionFrequentlyteachingStyleBetterlanguageEnglishtimestamp28 March 2026 at 16:15 UTC+5:30secureRollHash(hashed for student privacy)


Roll numbers are hashed before storage — student identity is never exposed in the database.




How It All Connects

+--------------+     +---------------------+     +----------------+     +-------------+
|              |     |                     |     |                |     |             |
|  HTML Form   |---->|  Cloud Firestore    |---->| Google Sheets  |---->|  Power BI   |
|  (Frontend)  |     |  (NoSQL Real-time)  |     | (Fetch Script) |     |  Dashboard  |
|              |     |                     |     |                |     |             |
+--------------+     +---------------------+     +----------------+     +-------------+
 Student submits       Stored instantly             Auto-exported          Visual insights
 feedback online       in the cloud                 to spreadsheet         for coordinators


Key Features

FeatureDescriptionSimple Web FormStudents rate faculty, subject, teaching style, interaction & language preferenceReal-Time Cloud StorageEvery response is instantly saved to Google Cloud Firestore — no delaysAutomated Data PipelineFirestore data is fetched and exported to Google Sheets automaticallyInteractive DashboardPower BI report with filters, charts, and per-faculty/subject breakdownsStudent PrivacyRoll numbers are securely hashed before being storedWorks EverywhereThe feedback form is fully responsive — mobile, tablet, and desktop


Tech Stack

Frontend


HTML5, CSS3, Vanilla JavaScript
Firebase SDK (Firestore write integration)


Cloud Backend


Google Cloud Firestore (NoSQL, real-time database)


Data Pipeline


JavaScript Fetch API
Google Sheets (as intermediate data store)
.xlsx export for Power BI ingestion


Analytics


Microsoft Power BI Desktop & Power BI Service



Getting Started

Prerequisites


A modern web browser
Google Cloud account with Firestore enabled
Node.js v16+
Power BI Desktop (free from Microsoft)




<div align="center">
Built with dedication at KL University  |  Cloud Computing Project 2026

<br/>
Live Feedback Form  ·  View Power BI Dashboard

<br/>

</div>
