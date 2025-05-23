# User

The Interfact admin dashboard has a number of features. This document will show how a user can interact with the dashboard.

#### 1: Authorized Login Page
![Picture1](https://github.com/user-attachments/assets/b5c44147-1455-43a9-9d57-200f068adebe)

• Only users with access to a correct passkey will be able to bypass the introductory homescreen


#### 2: Main Dashboard Page
![Screenshot (36)](https://github.com/user-attachments/assets/0e2d7a3a-2634-48da-adae-7fef2a180452)
![Screenshot 2025-02-03 102357](https://github.com/user-attachments/assets/67a70fd6-1508-487d-81ec-f74be23efdef)

• After a correct passkey is entered, the user is taken to the main dashboard page shown above. From here, the user can:

      • View added cameras at the bottom of the page.
      
      • Filter viewed results by pressing the "Filter" button, which will then
          reveal "OPEN," "BLOCKED," and "UNDER MAINTENANCE" buttons, which will filter the search results
          based on the current status of the intersection the camera item is placed at.
      
      • Add new cameras by pressing the "+" button at the bottom of the page.
      
      • View a map of the data by accessing the interfact.live website by
          clicking the "Map View" button.
          
      • Manually refreash available data by pressing the refreash button in the
          top right corner of the city card located in the center of the screen.
      
      • Return to this page from other pages by selecting "Home" from the nav bar
          located at the top of the page.
          
      • View the cities with Interfact connected cameras by selecting "Cities"
          from the nav bar at the top of the page. 

      • View the cameras with active user reports by selecting "Requests"
          from the nav bar at the top of the page. 



#### 3: View map data from interfact.live
![Screenshot (26)](https://github.com/user-attachments/assets/165503b5-fe84-4a9d-a7c6-8af8858c33fa)

    • If the user presses the "Map View" button located on
        the main dashboard page, the user will be directed to the
        interfact.live website as pictured above.
        
    • From here, the user can login to (or create the necessary credentials
        by clicking the "Register" button) to view the data on a
        map for the city of Muncie.

#### 4: View camera data
![Screenshot (33)](https://github.com/user-attachments/assets/25545903-7f4b-4ed7-8648-0a7bb9caff66)

    • Each card item is a camera at a railway intersection. The most recent
        picture the camera has captured will be shown, otherwise the view will
        contain a stock background photo as seen on the "S Monroe St."
        card at the bottom left of the list. Camera location can be found in
        the upper left hand corner of the card.
        
Each card will have 5 indicators: 
    - A red circle in the upper right corner: Indicates the number of user reports that intersection has recieved
    - A "Last Updated" label: Provides the number of minutes since the last image capture.
    - An "Image Classification" label: Labels the intersection as Blocked or Unblocked.
    - A "Camera Status" Label: Labels the camera as Working or Not Working.
    - A Green or Red colored Bar: Will be Red if the camera is not working, & Green if operational.


#### 5: View camera details:
![Screenshot (37)](https://github.com/user-attachments/assets/c41fcf79-b5c7-4258-bc42-c2552fcbc7f3)
![Screenshot 2025-02-03 102433](https://github.com/user-attachments/assets/b3855b63-7a83-40d7-8d94-d7c67cf51ad4)

    • By clicking on a camera, a camera dashboard will appear like shown above. 
    • This view will contain additional camera specific data such as:
      - The cameras longitude and latitude
      - ID, image path for the most recent picture & it's timestamp, and status.
      - A list of reports recieved from users,
        each with an image path and a report classification. 
     • Accept or Deny user reports by clicking on the thumbs up or down images according to the 
           report's validity. 

#### 6: View Predictive Data For Specific Intersections:
![Screenshot (133)](https://github.com/user-attachments/assets/4ee9f240-5927-4fc8-8de0-42291ff1f5f8)

• Users can: 

• See how busy an intersection is during any given time of day.

• See the ammount of time on average the intersection is blocked.

• See the total ammount of time the intersection was blocked in the last 24 hours & in the last week.

#### 7: Upload Snapshot of Data to Firebase:
![Screenshot (132)](https://github.com/user-attachments/assets/4109f2c2-a5c3-4980-9df7-e1e41f0fd6ee)

• By clicking the right most button on the "Hourly Blocked Percentage" widget, a popup will appear to give the snapshot a name before clicking the upload button. 

#### 8: Refresh logs & View Agerage Block % For Each Day of the Week:
![Buttons](https://github.com/user-attachments/assets/1ada5cf8-5201-4ddc-9d41-1292cc2a473d)

• By clicking the middle button, the list of camera logs are fetched, adding new entries if new entries have been added since the page was first loaded. 

• Clicking the first button on the left will change the view from hourly throughout the week to % blocked for each day of the week!
