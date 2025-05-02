## Known bugs / issues
- The Reports (confirm/deny a user-reported image) cannot show images that are not in the project itself, making the confirmation/denial of if an image is correctly labeled require finding the image itself in the file system
- The opening screen (the page.tsx located in the app folder) is a nothing implementation; the password is hardcoded in and is not visually obscured.


## Future improvements
- Our final changes have not been well tested
- Our "Cities" page (app/cities/page.tsx) is a static page that takes the user to the "Intersections" page (app/Intersection/page.tsx), and does not actually sort based on any city. If future cities are to be addded, the link on the Cities page should send the Intersections page something to filter what it displays by.

