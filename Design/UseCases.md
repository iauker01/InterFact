# Use Cases

## Actors
- Dispatcher
- First Responder
- Administrator
- Interfact User

## Use Cases
- UC1: A dispatcher finds the quickest route to a target location as first responders make their way there
  - BR1
  - Dispatcher
  -This is the only necessary use case for the client. The client needs a system that dispatchers
can rely on to help first responders make informed decisions on the quickest and best route to take.
The use cases for this software can be expanded upon in the future but for the requirements the client has
there is only one use case currently.

  - Flow:
    1) Dispatcher Opens the System Dashboard:
    - The dispatcher logs into the system and is presented with a map-based dashboard that shows the status of all monitored train intersections.
    2) Check for Blocked Intersections:
    - The dashboard clearly marks any blocked intersections
with a red indicator, while clear intersections are marked in green.
    - The dispatcher can quickly identify problematic areas from the map overview.
    3) View a Blocked Intersection:
    - The dispatcher clicks on a red-marked intersection to open the latest picture from the camera feed at the intersection.
    4) Verify the Blockage with Visual Data:
    - The dispatcher reviews the feed to confirm the blockage or any ongoing issues, ensuring that the status is accurate.
    5) Notify First Responders:
    - The Dispatcher uses the information received from the system to advise first responders on the quickest and most efficient route.


- UC 2: An Interfact user sees that an intersection in their driving route has become blocked and changes routes.
  - BR1
  - Interfact User
  - Flow:
    1) User has system open before trip or while en route
    2) An intersection updates its status
    3) The indicator of the intersection clearly changes
    4) If the intersection was part of their path, change directions accordingly
  - Because trains may come in while users are already en route, they will need to see information quickly, reducing the risk of getting stuck while a train is crossing.
  

- UC 3: A dispatcher corrects an intersection wrongly marked as blocked or open
  - BR1
  - Dispatcher
  - Flow:
    1) Dispatcher has system open
    2) Dispatcher selects an intersection
    3) Dispatcher compares latest picture of intersection to its status in the system
    4) If the picture and status do not match, select button reporting issue
  - There is potential for bad actors here. While it is desirable that when one dispatcher notices the inconsistency, it is corrected for all dispatchers, a single button click affecting an intersection on all systems is ripe for misuse or a misclick causing problems. On the other hand, requiring multiple reports to fix the inconsistency slows down the actual effectiveness of being able to mark something as wrong.


- UC 4: An administrator sets up a new camera at a new intersection and adds it to the system
  - BR2
  - Administrator
  - Flow:
    1) Set up new camera pointed at intersection
    3) Open administrator portal
    4) Press "Add new intersection"
    5) Input intersection name, coordinates
    6) Hook camera to picture-sending email using the intersection name
    7) Once the new intersection in the system receives pictures, appear on the user dashboard
  - This is to facilitate the expansion of the system. To prevent bad actors or incorrectly setting up, the new intersections should not appear on the user end unless they begin to receive images

- UC 5: An Admin Merges and Manipulates Collected Data
  - BR3
  - Administrator
  - Flow:
    1) The admin uses the dashboard to access collected data from both a relational database and Firebase.
    2) The admin generates reports and views merged data across multiple intersections.
   
- UC 6: A system admin updates the system with no downtime in the service
  - NR2, BR1
  - Administrator
  - Flow:
    1) The system updates its data and software components without disrupting dispatcher access to crossing statuses and feeds.

- UC 7: User Authentication and Role-Based Authorization
  - BR3, FR7
  - Interfact User (Administrator or Standard User)
  - Flow:
    1) Open the login page.
    2) Input username and password.
    3) System verifies credentials.
    4) Based on user role, access is granted to relevant system features:
      - Admin: Full access, including admin dashboard.
      - Standard User: Access to map, status updates.
      - Operator: Access to camera feeds, crossing data.
    5) User is redirected to their respective dashboard with role-specific permissions.
    - This ensures proper access control, allowing only authorized users to perform certain tasks based on their role.

  UC 8: A user receives a notification when a railroad intersection is blocked
    - FR8
    - Interfact User
    - Flow
      1) The system continuously monitors railroad crossing statuses.
      2) A railroad intersection becomes blocked.
      3) System generates a notification (e.g., email, SMS, in-app alert).
      4) The user receives the notification on their device or platform.
      5) The user acknowledges the notification and can take appropriate action.
    - This ensures users are promptly notified of blocked intersections, helping with real-time response and planning.
      
  UC 9: An admin views and analyzes historical railroad crossing data
    - FR9
    - Administrator
    - Flow
      1) Admin logs into the admin dashboard.
      2) Navigates to the "Historical Data" section.
      3) Select the type of data to view (crossing status, camera feeds, etc).
      4) Apply filters (by date range, location, or crossing, etc).
      5) The system displays the requested historical data along with trends and analytics (number of blockages over time, etc).
      6) Admin analyzes the data for decision-making or reporting.
    - This ensures users are promptly notified of blocked intersections, helping with real-time response and planning.
  
