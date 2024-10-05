# Plant Caring Project

## Overview

The Plant Caring Project is a backend application designed to manage and monitor various environmental factors related to plant care. This project utilizes Flask as the web framework and MongoDB for data storage. The API allows users to control sensors for light, moisture, temperature, humidity, and other factors that contribute to optimal plant health.

## Features

- **Sensor Management:**
  - Add, update, and delete sensor data.
  - Activate and deactivate various sensors (e.g., light, fan, pump).
- **Settings Management:**
  - Manage different settings for sensor configurations.
  - Select and update active settings for specific conditions.
- **RESTful API:**
  - Endpoints for managing sensors and settings, providing a clear structure for interacting with the application.

## API Endpoints

### Sensors

- `GET /sensors`
  - Retrieve all sensors.
- `GET /sensor/<name>`
  - Get sensor data by name.
- `POST /sensor/<type>`
  - Set sensor values (e.g., light, moisture, temperature, humidity, pump, fan, LED).

### Settings

- `GET /settings`
  - Retrieve all settings.
- `POST /add/settings`
  - Add a new setting.
- `POST /update/settings`
  - Update an existing setting.
- `POST /delete/settings`
  - Delete a specific setting.
- `GET /get/setting`
  - Retrieve the currently selected setting.

### Activation/Deactivation

- `GET /activate/<sensor>`
  - Activate the specified sensor (e.g., fan, pump, LED).
- `GET /deactivate/<sensor>`
  - Deactivate the specified sensor (e.g., fan, pump, LED).

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/aon123/plant
   cd plant
   ```

2. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Ensure MongoDB is running and accessible.

4. Start the Flask application:

   ```bash
   python app.py
   ```

5. The API will be accessible at `http://localhost:3000`.

## Technologies Used

- **Flask:** A micro web framework for Python.
- **MongoDB:** A NoSQL database for storing sensor data and settings.
- **Python:** The programming language used for the backend logic.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

Feel free to modify any sections to better suit your project!
