# Architecture

## Pre-existing parts
### Camera
The trail camera is set up pointing at a railroad `Intersection.` It can take and send `Pictures`, with the fastest time being once every 3 minutes. It is connected to a solar panel.
**FUNCTION:** Sends `Pictures` from `Intersection` to `Email`

### Email
Receives `Pictures` from multiple `Cameras.` Currently interfact.camera@gmail.com
**FUNCTION:** Holds `Pictures` for `Python Status Checker`

### Python Status Checker
Routinely and periodically checks `Email` for new `Pictures.` Is also triggered when `Email` receives a message.
**FUNCTION:** Takes `Picture` from `Email.` Identify if `Picture` is a `Train` or not. Send `STATUS`, based on indentification result, and `Picture` in `DataBase` for this `Intersection.` Store `STATUS` and `Picture` in local archive. Send `Users` That have this `Intersection` marked a Notification.

### DataBase
Currently FireBase. 
**FUNCTION:** Stores a latest `Picture` and `STATUS` for each `Intersection`

