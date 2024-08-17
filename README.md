# Weather-app-js

This weather app is a responsive, user-friendly web application designed to provide real-time weather information for any city. The app is built using HTML, CSS, and JavaScript, with weather data sourced from the OpenWeatherMap API. It features a modern design with a gradient background, rounded corners, and a clean, easy-to-read layout.

1. Key Features

- User Input for City Search

The app includes a search bar where users can enter the name of a city. This input is captured by a text field with a placeholder indicating "enter city name." A search button next to the input field triggers the weather search.

- API Integration

The app uses the OpenWeatherMap API to fetch current weather data for the city entered by the user. The API URL is constructed using the base API endpoint, the city name, and a unique API key provided by OpenWeatherMap.

- Dynamic Data Display

Once the weather data is retrieved, the app dynamically updates the user interface to display the city name, temperature, humidity, and wind speed. These values are inserted into corresponding HTML elements using JavaScript's innerHTML property.

- Weather Icons

The app includes different weather icons (e.g., clouds, clear sky, rain) that are displayed based on the current weather conditions in the selected city. The icons are updated dynamically by checking the weather condition returned by the API and then setting the src attribute of the image element accordingly.

- Error Handling

If the API returns a 404 error (e.g., when the city name is invalid or not found), the app displays an error message and hides the weather information. This ensures that users receive immediate feedback when their search query is incorrect.

- Responsive Design

The app is designed to be fully responsive, with a flexible card layout that adjusts to different screen sizes. The CSS uses a combination of percentage-based widths, maximum widths, and media queries to ensure the app looks good on both desktop and mobile devices.

- Modern UI/UX

The app uses a custom Google Font ("Poppins") for a clean and modern appearance. The color scheme includes a dark background with a gradient card, providing a visually appealing contrast that enhances readability. Buttons and input fields are styled to be intuitive and easy to interact with, featuring rounded corners and subtle shading.

2. Technical Overview
   
- HTML Structure

The HTML document is structured with a main div container (card) that holds all the elements of the app, including the search bar, error message, and weather details. Semantic tags like H1, H2, and P are used for textual content, while images are used for weather icons.

- CSS Styling

The CSS file provides the visual design, including the overall layout, colors, fonts, and responsiveness. It uses flexbox for aligning elements within the search bar and weather details section, ensuring consistent spacing and alignment.

- JavaScript Functionality

The core logic is handled by JavaScript, which includes:

checkWeather(city)

An asynchronous function that fetches weather data from the API, processes the response, and updates the DOM with the relevant weather information.

    async function checkWeather(city) {
      // Function implementation
    }

Event Listener

The app adds an event listener to the search button, triggering the checkWeather() function when the user clicks it. This allows users to search for weather data interactively.

    searchBtn.addEventListener("click", ()=>{
      // Function implementation
    }

Error Handling

The app includes basic error handling to manage situations where the user inputs an invalid city name. If an error occurs, the app displays a message informing the user and hides the weather data to prevent confusion.



In summary, this weather app is a practical tool that leverages modern web technologies to provide users with up-to-date weather information. Its clean design, coupled with robust functionality, makes it both aesthetically pleasing and highly usable.
