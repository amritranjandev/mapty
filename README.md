
# Workout Tracker App

A web-based application to log running and cycling workouts on a map. The app leverages geolocation to detect the user's location and integrates with Leaflet.js to display the map and markers.

## Features

* **Log Workouts** : Add running or cycling workouts with details such as distance, duration, and cadence/elevation.
* **Interactive Map** : Click on the map to set a workout location.
* **Dynamic UI Updates** : View workouts with details dynamically displayed on the UI.
* **Geolocation Support** : Automatically detect the user's location for the initial map view.

## Technologies Used

* **HTML/CSS** : For structure and styling.
* **JavaScript (ES6+)** : Main application logic, including classes and methods.
* **Leaflet.js** : For map integration and marker functionality.
* **Geolocation API** : To get the user's current location.

## Setup Instructions

### Prerequisites

* A modern web browser.
* Internet connection for loading map tiles.

### Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/workout-tracker.git
   cd workout-tracker
   ```
2. **Project Structure**
   * `index.html`: Main HTML file.
   * `style.css`: Styling for the application.
   * `script.js`: Main JavaScript logic.
   * `images/`: Contains images used in the project (if any).
   * `README.md`: This file.
3. **Run the App**
   * Open `index.html` in your browser to view the application.

### Usage

1. Allow the app to access your location when prompted.
2. Click anywhere on the map to add a workout.
3. Fill in the form that appears with the workout details:
   * Select type (`Running` or `Cycling`).
   * Enter distance, duration, and cadence/elevation gain.
4. Submit the form to see your workout logged on the map and in the UI.

## Project Structure

```
mapty/
├── icon.png
├── logo.png  
├── style.css                 # CSS for the application
├── script.js                 # JavaScript code with app logic
├── index.html                # HTML structure
├── README.md                 # Documentation
```

## Screenshots

### Workout Form

### Map View

## Customization

* **Map Tiles** : Update the map tile URL in the `_loadMap` method:

```js
  L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
      attribution: '© OpenStreetMap contributors',
  }).addTo(this.#map);
```

* **Styling** : Modify `style.css` to change the app's look and feel.

## Future Enhancements

* Save workouts to `localStorage` or a database for persistence.
* Add features like editing and deleting workouts.
* Implement filters to view specific types of workouts.
* Add support for multiple users.

## Credits

* [Leaflet.js](https://leafletjs.com/) for map integration.
* OpenStreetMap for map tiles.
* Font Awesome for icons (if used).

## License

This project is open-source and available under the [MIT License](https://chatgpt.com/c/LICENSE).
