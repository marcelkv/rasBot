# RasBot - Remote Robot Control Web App

![RasBot Logo](images/rasBot.png)

## Overview

RasBot is a web application that enables remote control of a robot equipped with a live-streaming camera. Users can control the robot's movements using an intuitive joystick interface on the web app, while simultaneously viewing the robot's camera feed in real-time. This README provides an overview of the project, setup instructions, and essential information for developers and users.

## Features

- **Remote Robot Control:** Control the robot's movements from anywhere with an internet connection.
- **Live Camera Stream:** View the live camera feed from the robot on the web app.
- **Joystick Control:** Intuitive joystick interface for precise robot control.
- **Firebase Integration:** Use Firebase to store joystick position data, enabling real-time communication between the web app and the robot.
- **Raspberry Pi Integration:** The robot is powered by a Raspberry Pi, programmed in Python, to control the motors and camera.

## Technologies Used

### Frontend

- Vue.js
- TypeScript
- HTML
- LESS

### Backend (Robot Control)

- Raspberry Pi
- Python

### Data Storage and Real-time Communication

- Firebase

## Installation

### Web App

1. Clone the repository:

   ```bash
   git clone https://github.com/marcelkv/rasBot-webApp.git

2. Navigate to the project directory:

   ```bash
   cd rasBot-webApp

3. Install project dependencies:

   ```bash
   npm install

4. Configure Firebase:

- Create a Firebase project: [Firebase Console](https://console.firebase.google.com/)
- Copy your Firebase configuration (API keys, database URL, etc.) and replace them in the project configuration files.

5. Build and run the web app:

    ```bash
    npm run serve

6. Access the web app at `http://localhost:8080` in your browser.

### Raspberry Pi

1. Connect your Raspberry Pi to the robot hardware components (motors and camera).

2. Install Python on your Raspberry Pi if not already installed.

3. Clone the Raspberry Pi control code to your Raspberry Pi:

    ```bash
    https://github.com/marcelkv/rasBot-rpi.git

4. Navigate to the Raspberry Pi control code directory:

    ```bash
    cd rasbot-rpi

5. Install the required Python packages:

    ```bash
    pip install -r requirements.txt

6. Run the Python script to control the robot:
    ```
    python rasbot_control.py

## Usage

1. Open the RasBot web app in your browser.

2. Use the joystick interface to control the robot's movements.

3. Observe the live camera stream to see where the robot is going.

4. The web app sends joystick position data to Firebase, which the Raspberry Pi reads to move the robot accordingly.

## Contributing

We welcome contributions to RasBot! Feel free to submit bug reports, feature requests, or pull requests to help improve the project.

## Contact

If you have any questions or need assistance, please contact us at [marcel_kv@hotmail.com](mailto:marcel_kv@hotmail.com).

Happy Robot Controlling with RasBot! 🤖🚀
