# Dictionary Web App using HTML, CSS, JS, and API Integration
## Overview
This Dictionary Web Application provides a simple interface for users to search for word definitions and phonetics. Leveraging the Dictionary API, this app offers real-time word meanings and examples, along with pronunciation audio where available. The application is built using HTML, CSS, and JavaScript, making it lightweight and easy to use.

![image](https://github.com/areeba0/Dictionary-Web-Application-Html-CSS-JS-with-API/assets/136759791/ecdfd77a-388d-4beb-bb87-f530de2aa10a)

## Responsive Web Design =

![image](https://github.com/areeba0/Dictionary-Web-Application-Html-CSS-JS-with-API/assets/136759791/d340d873-6ad1-4c50-82cf-03071cbfb019)


# Key Features
- Word Search: Enter a word and get its meaning, phonetic transcription, and examples.
- Phonetics Audio: Play pronunciation audio for words with phonetic data.
- Responsive Design: Compatible with various devices and screen sizes.
- Error Handling: Displays an error message if the word is not found.

# Dependencies
- Html
- CSS
- JavaScript
- Dictionary API (link for the API used) =
  ####  https://dictionaryapi.dev/
- For Icons =
   Font Awesome: (For the volume icon in the pronunciation button)
  #### https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css
- For Font =
   Google Fonts: For the Poppins font used in the app
   #### https://fonts.googleapis.com/css2?family=Poppins&display=swap

# User Interface
- A header with the application title.
- A search box for inputting the word.
- A search button to initiate the lookup.
- A result area that displays the word's details or an error message if the word is not found.

# Files
### index.html: Contains the HTML structure of the app.
### style.css: Provides the styling for the app.
### script.js: Handles the functionality, including fetching data from the API and updating the UI.

# Technical Implementation
The app uses the Dictionary API to fetch word data. JavaScript handles the API request and dynamically updates the HTML to display the results. CSS is used to style the application, making it visually appealing and user-friendly.

#  API Integration
The Dictionary Web Application integrates with the Dictionary API to fetch real-time word definitions, phonetic transcriptions, and example sentences. Here's how the API is integrated technically:

## API Endpoint:
The application uses the endpoint provided by the Dictionary API (https://api.dictionaryapi.dev/api/v2/entries/en/). This endpoint allows querying for English words and returns JSON data with detailed information about the word.

## Fetching Data:
When a user enters a word and clicks the search button, JavaScript fetches data from the API using fetch(). The word entered by the user is appended to the API endpoint to retrieve specific word details.

## Handling Responses: 
The response from the API is processed using .then() and .catch() Promises methods. The application parses the JSON response to extract information such as part of speech, phonetic transcription, definitions, and examples if the word is found.

## Error Handling: 
If the API returns an error (e.g. if the word is not found), the application displays an error message to the user.

## Audio Pronunciation:
If available, the application also retrieves and plays the pronunciation audio associated with the word using the phonetics data provided by the API.

