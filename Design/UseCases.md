# Use Cases

## Actors
- Dispatcher
- First Responder
- Administrator

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


- UC 2: A first responder sees that an intersection in their driving route has become blocked and changes routes.
  - BR1
  - First Responder
  - Flow:
    1) First Responder has system open while en route
    2) An intersection updates its status
    3) The indicator of the intersection clearly changes
    4) If the intersection was part of their path, change directions accordingly
  - Because trains may come in while first responders are out, they will need to see information quickly, reducing the risk of getting stuck behind a train in the time it takes a dispatcher to inform them of the change.
  

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
