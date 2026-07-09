# Video Calling Application

## Overview

This is a simple video calling application built in Java. It enables real-time video and audio communication between a client and a server over a network. The application uses Swing for the graphical user interface, OpenCV for video capture and processing, and the Java Sound API for audio streaming.

The project consists of two main components:
- **Client**: Connects to the server and handles video/audio sending and receiving.
- **Server**: Accepts connections from the client and manages the video/audio streams.

## Features

- Real-time video streaming using webcam.
- Audio communication via microphone and speakers.
- Simple GUI with local and remote video displays.
- Start/Stop call functionality.
- Cross-platform (Windows/Linux/Mac) with Java.

## Prerequisites

- Java Development Kit (JDK) 8 or higher.
- OpenCV 4.x for Java (download the JAR and native libraries from [OpenCV Releases](https://opencv.org/releases/)).
- NetBeans IDE (recommended for building) or Apache Ant.
- Webcam and microphone/speakers for video and audio.

## Installation

1. Clone or download the project to your local machine.
2. Download OpenCV for Java:
   - Go to [OpenCV Releases](https://opencv.org/releases/).
   - Download the version compatible with your system (e.g., opencv-4xx.jar).
   - Extract the native library (e.g., opencv_java4xx.dll for Windows, .so for Linux) and place it in a directory accessible via `java.library.path` or system PATH.
3. Place the OpenCV JAR file in the project classpath (e.g., create a `lib` folder and add it there).

## Build

### Using NetBeans
1. Open NetBeans IDE.
2. Open the project by selecting `File > Open Project` and navigating to the project directory.
3. Build the project using `Run > Build Project` or the build button.

### Using Ant
1. Ensure Apache Ant is installed.
2. Open a terminal in the project directory.
3. Run `ant` to build the project. The compiled classes will be in `build/classes`.

## Usage
1. **Start the Server**:
   - Run the Server class: `java -cp build/classes:lib/opencv-4xx.jar Server`
   - The server GUI will open, waiting for a client connection.

2. **Start the Client**:
   - Run the Client class: `java -cp build/classes:lib/opencv-4xx.jar Client`
   - The client GUI will open. Click "Start Call" to initiate the connection.

3. **During Call**:
   - Video from both sides will be displayed in the GUI.
   - Audio will be streamed in real-time.
   - Click "End Call" or "Stop Call" to terminate the session.

