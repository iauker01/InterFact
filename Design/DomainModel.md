# Domain Model
```mermaid
classDiagram
  class Train
    Train : +beAtCrossing()
    Train : +leaveCrossing()
  Intersection "1" --> "0..1" Train
  class Intersection
    Intersection : -String name
    Intersection : -Coordinates location
  class CameraImage
    CameraImage : -Intersection crossing
    CameraImage : -RawPhoto lastPicture
    CameraImage : -takePicture() RawPhoto
    CameraImage : +send()
  CameraImage "1" --> "1" Intersection
  CameraImage --> "1" TrainPictureDetector : SendsTo
  class TrainPictureDetector
    TrainPictureDetector : +detectTrain(CameraImage) ProcessedImage
  TrainPictureDetector --> ProcessedImage
  class Status
    <<Enumeration>> Status
    Status : OPEN
    Status : BLOCKED
    Status : WILL_BE_BLOCKED
  class ProcessedImage
    ProcessedImage: -Status status
    ProcessedImage: +getOpen() String
  ProcessedImage --|> CameraImage
  ProcessedImage "1" --> "1" Status
  class Website
    Website : +getStatusOfIntersection(ProcessedImage) String
    Website : +getImageofIntersection(ProcessedImage) RawPhoto
    Website : +updateIntersection(ProcessedImage)
  Website "1" *-- "*" ProcessedImage
  class Dispatcher
    Dispatcher : +Map roadMap
    Dispatcher : +receiveCall(Coordinates)
    Dispatcher : -determineRoute(EmergencyResponder, Coordinates) String
    Dispatcher : -dispatchResponders(Coordinates)
  Dispatcher --> "1" Website
  Dispatcher o-- "*" FirstResponder
  class FirstResponder
    FirstResponder : -bool available
    FirstResponder : +setOptimalRoute(route)
    FirstResponder : -playSirenToClearTraffic()
    FirstResponder : +helpPeople()
  FirstResponder --|> Driver
  class Driver
    Driver : -String route
    Driver : -drive(route)
    Driver : +getStuckInTraffic()
  
    
```
