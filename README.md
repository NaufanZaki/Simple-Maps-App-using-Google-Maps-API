This project is a simple **Map Application** built for Android. It allows users to input a starting location and a destination, search for directions, and retrieve latitude and longitude using the Geocoder API.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Setup](#setup)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [How It Works](#how-it-works)
  - [Geocoder API](#geocoder-api)
  - [Google Maps API](#google-maps-api)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)

---

## Overview

This Map App allows users to:
- Input starting and destination addresses.
- Search for directions using a button.
- Display latitude and longitude of both locations.
- Integrate Google Maps for route visualization.

---

## Features

- **Search Functionality**: Retrieve geographic coordinates for locations using Geocoder.
- **Google Maps Integration**: Display route and navigation on a map.
- **User-Friendly Interface**: Simple fields for input and dynamic results display.

---

## Setup

### Prerequisites

1. **Android Studio** installed on your machine.
2. **Google Maps API Key**:
   - You must have a Google Maps API key for the project. Follow the [Google Maps API Documentation](https://developers.google.com/maps/gmp-get-started) to obtain one.

### Installation

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/username/map-android-java.git
    cd map-android-java
    ```

2. **Set Up `local.properties`**:
    - Open the `local.properties.example` file in the root of the project directory.
    - Copy the contents to a new `local.properties` file.
    - Replace `MAPS_API_KEY` with your actual API key.
      ```properties
      sdk.dir=C\:\\Users\\user\\AppData\\Local\\Android\\Sdk
      MAPS_API_KEY=YOUR_GOOGLE_MAPS_API_KEY
      ```

3. **Open the Project in Android Studio**:
    - Navigate to the project directory and open it in Android Studio.
    - Sync the project with Gradle.

4. **Build and Run**:
    - Connect an Android device or use an emulator.
    - Click **Run** to build and deploy the app.

---

## Usage

1. **Input Locations**:
   - Enter the starting location and destination in the provided text fields.

2. **Search Coordinates**:
   - Click the **Search** button to retrieve the latitude and longitude of both locations.

3. **View Map**:
   - Display the route between the locations on a Google Map.

---

## How It Works

### Geocoder API

1. **Fetch Latitude and Longitude**:
   - Converts user-inputted addresses into geographic coordinates.

2. **Display Results**:
   - The latitude and longitude are dynamically shown in the app's interface.

### Google Maps API

1. **Integrate API Key**:
   - Uses the Maps API key provided in `local.properties` to authenticate requests.

2. **Display Routes**:
   - Maps the route between the two locations on the interface.

---

## Technologies Used

- **Android Studio**: Development environment
- **Google Maps API**: Route visualization
- **Geocoder API**: Convert addresses to geographic coordinates
- **Java**: Programming language

---

## Project Structure

```
map-android-java/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── com.example.mapapp/
│   │   │   │       ├── MainActivity.java  # Main activity of the app
│   │   │   └── res/
│   │   │       ├── layout/
│   │   │       │   └── activity_main.xml  # User interface
│   │   │       ├── values/
│   │   │       │   └── strings.xml        # App strings
├── local.properties                       # Configuration file
└── README.md                              # Project documentation
```

---
