# Functional Requirements

+ FR1 - UC1 (LOW PRIORITY)
  
View an interactive and responsive map that has railroad crossings marked with their status

+ FR2 - UC1 (LOW PRIORITY)

Click/tap on railroad crossings to view coordinates and the latest image from the camera feed

+ FR3 - UC1 (LOW PRIORITY)

Predict which railroad crossings will be blocked by seeing which intersections have been crossed and when. 

+ FR4 - UC1 (HIGH PRIORITY)

A REST API with endpoints for crossing locations, crossing status, and most recent crossing images that can be accessed by the ArcGIS system.

+ FR5 - UC3 (MEDIUM PRIORITY)

An admin dashboard that can be used to see and manipulate data from a relational database and firebase.

+ FR6 - UC4 (MEDIUM PRIORITY)

New cameras can be easily added to the existing Interfact system. 

+ FR7 - UC7 (MEDIUM PRIORITY)

The system should include user authentication and role-based authorization for admin, standard users, and system operators.

+ FR8 - UC8 (MEDIUM PRIORITY)

Notifications or alerts should be sent to users when a railroad intersection becomes blocked.

FR9 - UC9 (LOW PRIORITY)

The system should allow users to access and analyze historical data on railroad crossings, including camera feed history and blockage trends.

# Non-Functional Requirements

+ NR1 (HIGH PRIORITY)

The intersection indicators must load in under 5 seconds

+ NR2 - (LOW PRIORITY)

The system must be able to be updated without downtime

+ NR3 - (LOW PRIORITY)

The admin dashboard and the webapp should be accessible on multiple platforms (e.g., desktop, tablet, mobile) to ensure flexibility for users in different roles
