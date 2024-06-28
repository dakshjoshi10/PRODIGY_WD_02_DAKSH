# PRODIGY_WD_02_DAKSH
This HTML code creates a simple stopwatch application with a user interface to start, pause, reset, and record lap times. Here's a breakdown of the components and their theoretical roles:

### HTML Structure

#### Document Metadata
- `<!DOCTYPE html>`: Declares the document type and version of HTML.
- `<html lang="en">`: Indicates the language of the document (English).
- `<head>`: Contains metadata and links to resources.
  - `<meta charset="UTF-8" />`: Specifies the character encoding (UTF-8).
  - `<meta http-equiv="X-UA-Compatible" content="IE=edge" />`: Ensures compatibility with Internet Explorer.
  - `<meta name="viewport" content="width=device-width, initial-scale=1.0" />`: Sets the viewport for responsive design.
  - `<title>Stopwatch</title>`: The title of the webpage, displayed in the browser tab.
  - `<link rel="stylesheet" href="./styles.css" />`: Links to an external CSS file for styling.

#### Document Body
- `<body>`: Contains the visible content of the webpage.
  - `<h1 class="heading">`: A heading element.
    - `<a href="index.html">Stopwatch</a>`: A hyperlink that navigates to `index.html`.
  - `<div class="container">`: A container for the stopwatch components.
    - `<div class="timer-display">`: Displays the timer (hours:minutes:seconds:milliseconds).
      - `00 : 00 : 00 : 000`: Initial display value of the timer.
    - `<div class="buttons">`: Container for the control buttons.
      - `<button id="start-timer">Start</button>`: Button to start the timer.
      - `<button id="pause-timer">Pause</button>`: Button to pause the timer.
      - `<button id="reset-timer">Reset</button>`: Button to reset the timer.
      - `<button id="lap-timer" class="timer-button">Lap</button>`: Button to record lap times.
  - `<h2 class="lap-list lap-label">Laps</h2>`: A heading for the lap list section.
  - `<ul class="lap-list" id="lap-list"></ul>`: An unordered list to display recorded lap times.
  - `<script src="./index.js"></script>`: Links to an external JavaScript file that adds functionality to the stopwatch.

### Theoretical Explanation

1. **Structure and Styling**: 
   - The HTML sets up a basic structure with headings, buttons, and containers. 
   - CSS (linked in the `<head>`) is used for styling, ensuring a visually appealing and consistent design across different browsers and devices.

2. **Interactive Elements**:
   - Buttons with specific `id` attributes (`start-timer`, `pause-timer`, `reset-timer`, `lap-timer`) are defined. These will be referenced in JavaScript to add functionality.
   - The `timer-display` div shows the current time of the stopwatch, which will be updated dynamically.
   - The `lap-list` ul element is where the lap times will be listed.

3. **JavaScript Integration**:
   - The external JavaScript file (`index.js`) is linked at the end of the body, ensuring the DOM is fully loaded before any scripts run.
   - This script will likely handle the logic for starting, pausing, resetting the timer, and recording lap times.

### Key Points
- **Separation of Concerns**: HTML handles structure, CSS handles styling, and JavaScript handles interactivity.
- **Responsive Design**: The viewport meta tag ensures the layout adapts to different screen sizes.
- **Interactivity**: The buttons and dynamic content (timer display and lap list) provide user interaction.
  
This setup forms the foundation of a stopwatch application, with the actual functionality implemented in the linked JavaScript file.

