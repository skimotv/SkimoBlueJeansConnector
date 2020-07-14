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
Use GET[https://api.bluejeans.com/v1/user/{userID}/meeting_history]

