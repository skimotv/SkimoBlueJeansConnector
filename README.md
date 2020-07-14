# Overview
## SkimoBlueJeansConnector
This repository has the connector to connect to the Blue Jeans conference service provider

The connector extends the SkimoConnectorTemplate, which utilizes Springboot and Thymeleaf

(refer to the template README for more info)

The connector uses the BlueJeans REST API to obtain data.

Visit the Skimo Website to test functionality.

## Functional Capabilities
**bold text** FULL ELABORATION FOR FUNCTIONS LISTED IN NEXT SECTION
Allow users to login to BlueJeans account using OAuth 2.0

Retrieve a list of rooms that the user is a member of

Retrieve a list of items in the selected room's drive

Retrieve a list of meetings from the items in the drive

Display a list of BlueJeans meetings on the Skimo website for the user

Allow user to select a recording and upload recording to the Skimo server

# Specific Functions
For each function - summarize step by step how the function works at a user level (UI inputs outputs)
      - summarize the code used to achieve said functionality 
      
## BlueJeans LogIn Using OAuth 2.0
Must used a registered BlueJeans Account

## Retreiving List of User ID's
Use GET https://api.bluejeans.com/v1/user/{userID}/tags. This shows all the users who have joined a meeting. 
## Retrieving List of Joined Meetings
Use GET https://api.bluejeans.com/v1/user/{userID}/meeting_history/recordings?pageSize=10&pageNumber=1&sortBy=start_time&order=desc. This shows all the meetings a user has joined.
## Retrieving List of Recordings
Use GET https://api.bluejeans.com/v1/user/{userID}/meeting_history/{meetingID}/recordings. This shows all the recordings within a meeting. 
## Display List of Calls in Skimo
## Meetings Select and Upload
# Source
http://https://bluejeans.github.io/api-rest-meetings/site/index.html
# Contributing & Support
We'd love that you contribute to the project. Before doing so, please contact vishruth.mattegunta@sjsu.edu for more info.





