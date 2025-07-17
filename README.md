# Overview

This is a simple Timestamp Microservice built with Node.js and Express. It accepts a date string or a Unix timestamp as a parameter and returns a JSON response containing the Unix timestamp (in milliseconds) and the UTC string representation of that date.

If no date parameter is provided, it returns the current date and time.

If the date parameter is invalid, it returns a JSON object with an error message.

## About

This project was completed as part of the [freeCodeCamp](https://www.freecodecamp.org/) Backend Development and APIs curriculum. It helped me practice working with Express, routing, and date handling in JavaScript.

---

## Usage

- **GET** `/api/:date?` — The date parameter is optional.

### Examples

- `/api/2015-12-25`  
    Returns:  `{ "unix": 1451001600000, "utc": "Fri, 25 Dec 2015 00:00:00 GMT" }`
    
- `/api/1451001600000`  
    Returns:  `{ "unix": 1451001600000, "utc": "Fri, 25 Dec 2015 00:00:00 GMT" }`
    
- `/api/invalid-date`  
    Returns:  `{ "error": "Invalid Date" }`
    
- `/api/` (no date)  
    Returns current date/time in both unix and utc.

---

## Technologies Used

- Node.js
    
- Express