# Razer AI Service

## Overview
The **RazerAIService** project is a video recording and communication service designed to handle video capture, processing, and communication tasks. It integrates with AI-based systems to manage video recording sessions, upload recorded content, and interact with external systems through HTTPS-based communication.


## Features
- **Video Recording**: Captures video content and manages recording sessions.
- **AI Communication**: Interacts with AI systems to process and upload recorded videos.
- **WYVRN SDK**: Uses WYVRN SDK game events.


## Key Components
1. **Shiny moments**:
   - Manages video recording sessions.
   - Handles starting, stopping, and saving video recordings.
   - Communicates with external systems to upload videos and manage recording configurations.

2. **AI Communication**:
   - Sends HTTP requests to external AI systems for tasks like saving files, starting/stopping recordings, bug detection.

3. **WYVRN SDK**:
   - Fetch WYVRN game events


## How It Works
1. **Initialization**:
   - The service is initialized with a binary path and arguments for the video recording process.
   - It sets up communication with AI systems using HTTP.

2. **Video Recording**:
   - The service can start and stop video recording sessions.
   - Recorded videos are saved and uploaded to external systems.

3. **Communication**:
   - HTTP requests are used to interact with external systems for tasks like:
     - Starting/stopping recordings.
     - Selecting windows for capture.
     - Uploading recorded videos.


## Dependencies
- **Simple-Web-Server**
- **Simple-Web-Socket**
- **Windows APIs**
- **Boost**
- **OpenSSL**

## Usage
1. **Setup**:
   - Ensure all dependencies are installed and configured.
   - Build the project using a C++20-compatible compiler (e.g., Visual Studio 2022).

2. **Running the Service**:
   - Service is automatically started after installation

3. **Configuration**:
   - Replace or modify **service.conf** next to the RazerAIService.exe by conf file provided for beta.

## License
This project is © 2025 Razer Inc. All rights reserved.