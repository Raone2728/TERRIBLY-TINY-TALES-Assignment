# Terribly Tiny Tales Assignment

## Hosting

The application has been deployed on Netlify. 

check it out https://12001565-terriblytinytales.netlify.app/

## Getting Started

To run the application locally, follow these steps:

1. Clone the repository: git clone https://github.com/Raone2728/TERRIBLY-TINY-TALES-Assignment/tree/main

2. Install the dependencies: npm install

3. Start the development server: npm start

4. Open [http://localhost:3000](http://localhost:3000) in your web browser to view the application.

## Components

The application is structured into the following components:

- **Api**: This component exports a function called fetchApi that fetches data from an API endpoint https://www.terriblytinytales.com/test.txt. It uses the fetch function to make the HTTP request and returns the response as a text string.
- **components**:HistogramChart.js: This component is a reusable React functional component called HistogramChart. It receives a data prop, which is an array of objects containing letter and frequency data. It dynamically adjusts the width and height of the chart based on the window size using the useState hook. It also handles resizing of the chart with the useEffect hook. The component renders a responsive bar chart using the 
- **Utils**:This component contains utility functions for data processing. The filterAlphabet function filters out non-alphabetic characters from an object, returning a new object with only alphabetic keys. The objToArr function converts an object into an array of objects, sorting them based on frequency in descending order. The calculateWordFrequencies function calculates word frequencies from a text string, filters out non-alphabetic characters, and returns the top 20 most frequent words as an array of objects.
- **App.js**:This component is the main component of the application. It imports functions and components from other files. It manages the state with the useState hook, storing the wordArray and loading states. The fetchData function fetches data using fetchApi, calculates word frequencies using calculateWordFrequencies, and updates the wordArray state. The component renders a container with a heading and a fetch button. When the fetch button is clicked, it triggers the fetchData function, which fetches data and updates the state. If the wordArray state is not empty, it renders the HistogramChart component with the wordArray data and a download button for exporting the data as a CSV file. The download button triggers the downloadData function, which converts the data to CSV format and initiates the download.

## Libraries 

The project utilizes the following libraries:

- **recharts**: This library provides charting components for React
- **react**:A JavaScript library for building user interfaces
- **react-dom**:react-dom is a package that serves as the entry point to the DOM and is specifically designed for React applications. 

 


