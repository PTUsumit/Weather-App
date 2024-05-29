# Weather with Fetch AI's uagents
Welcome to the Weather Integration project using uAgents! This project leverages Fetch.ai's uAgents to provide detailed information about the weather type,temperature,temperature felt,pressure,humididity and many more. The frontend is a React application that interacts with the uAgents backend to display this information to users.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [uAgents Endpoints](#uagents-endpoints)
- [Running the React App](#running-the-react-app)


## Features

- **Weather Information**: Get detailed weather of any city by providing the city,state and country name.

## Installation

### Backend (uAgents)

1. **Clone the repository**:
    ```bash
    git clone https://github.com/PTUsumit/Weather-App.git
    cd Weather-App
    ```

2. **Set up a virtual environment**:
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Run the uAgents backend**:
    ```bash
    cd backend/agents
    python agent.py # similarly run agents on different terminals
    ```

### Frontend (React)

1. **Navigate to the frontend directory**:
    ```bash
    cd frontend
    ```

2. **Install dependencies**:
    ```bash
    npm install
    ```

3. **Start the React app**:
    ```bash
    npm start
    ```

## Usage

1. **Ensure the uAgents backend is running**:
    ```bash
    python agent.py
    ```

2. **Ensure the React frontend is running**:
    ```bash
    npm start
    ```

3. **Access the application**:
    Open your browser and navigate to `http://localhost:3000`.

## uAgents Endpoints

The uAgents handle specific request. Here is the main agent and its functionalities:

- **Weather Agent**: Handles requests for weather forecasting and it provides you all kinds of weather data as you need most.

### Example Queries

- **Nutrition Information**: 
    ```
    POST /
    ```
    Response example:
    ```json
    {
  "coord": {
    "lon": 10.99,
    "lat": 44.34
  },
  "weather": [
    {
      "id": 501,
      "main": "Rain",
      "description": "moderate rain",
      "icon": "10d"
    }
  ],
  "base": "stations",
  "main": {
    "temp": 298.48,
    "feels_like": 298.74,
    "temp_min": 297.56,
    "temp_max": 300.05,
    "pressure": 1015,
    "humidity": 64,
    "sea_level": 1015,
    "grnd_level": 933
  },
  "visibility": 10000,
  "wind": {
    "speed": 0.62,
    "deg": 349,
    "gust": 1.18
  }
    ```

## Running the React App

1. **Navigate to the frontend directory**:
    ```bash
    cd frontend
    ```

2. **Install dependencies**:
    ```bash
    npm install
    ```

3. **Start the React app**:
    ```bash
    npm start
    ```
 **It is extreamly sorry that  you have to take the backend file in your vs code and run app.py and agent.py to get effective result.**
