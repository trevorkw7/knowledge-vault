
Question 1a

Original Answer  
1. Create an upcoming event with details
2. Display upcoming events
3. Filter upcoming events by type 
4. Automatically register for events by filling in the user's email address and PID

Correction with Explanation  
1. Display upcoming events
2. Filter upcoming events by type 
3. Automatically register for events by filling in the user's email address and PID

I thought that "Create an upcoming event with details" was a feature for this app that had to be implemented in order for the other app's other features like "Display upcoming events" to function. However, it actually isn't a feature as creating upcoming events isn't a feature that is applicable to end-users who in this case would be students using the app to browse and sign up for events. Thus, in the correction I removed this from the feature list as all features need an end-user observable feature. Source: Day 05 Slides, slide #9

Question 2c

Original Answer:
1. Implement a drag and drop modal that lets users drop images from their device into the current itinerary
2. Embed a Google Images search bar for users to search for images and add them into the current itinerary

Correction with Explanation:
1. Create the "add images" button and implement a popup window for users to upload an image through the file explorer when the "add images" button is pressed
2. Create save functions that make a POST request to the database with the newly added image and have the save functions be called after the user uploads new images to the itinerary 

The two features I originally wrote were too unspecific in how the UI would be implemented and the logic behind that UI was not included. Furthermore, the two tasks I wrote implemented the same feature in two different ways rather than addressing the feature in it's entirety with a UI and backend logic component. This didn't address best address the story as we learned in lecture a good starting point has one Task each for a backend, UI, and core feature code. Thus, in the correction, I updated the UI related task with a more specific logic flow that describes a button and popup window and replaced the redundant Google Images search bar implementation of the feature with a task that describes the backend function that needs to be created and called. Source: Day 07 Slides, slide #9




