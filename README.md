# C++ Coding Challenge

Hello and welcome to the C++ coding challenge! This challenge is designed to test your knowledge of C++ and your ability to write efficient, clean, and easy to read code.

> [!IMPORTANT]
> If you have any questions or need clarification, please don't hesitate to reach out to us at [roland@teton.ai](mailto:roland@teton.ai).

## Objective 🎯

Develop a multi-process application in C++ that captures video frames from a stream, processes them in parallel through different algorithms, and then aggregates the results in a central process for output.

### Process 1: Capture Frames

The first process should handle the video input and capture frames from the (preferably) live video stream. It needs to provide the frames to the other processes for further processing using an IPC mechanism.

### Process 2 & 3: Image Processing

Implement two different processing each with its own image processing algorithm. A couple of examples for the processing algorithms are:

1. **Optical Flow**: Implement an optical flow algorithm to detect motion in the video stream.
1. **Circle Detection**: Implement a circle detection algorithm to detect circles in the video stream.

### Process 4: Aggregation and Visualization

The last process should aggregate the results from the other processes and display the results. It should receive both the original frame and the processed frames from the other processes and display them side by side.

Make sure the frames are synchronized such that both of the processed frames are displayed with the original frame they were processed from.

You are allowed to drop frames if the processing is too slow, but all 3 frames should always be synchronized when displayed.

> [!TIP]
> If you are unfamiliar with image processing algorithms, a good place to start is [OpenCV](https://opencv.org/).

## Requirements 📋

To complete this challenge, we ask that you use C++ for your implementation. You are free to use any standard library functions, and you may also use any third-party libraries if you wish.

* **Minimum C++ version:** C++11
* **Approximate time to complete:** 4 hours
* **Video**: Preferably a webcam for live video input (alternatively, you can use a video file).
* **Target**: Your solution must compile and run on an Ubuntu 22.04 system (at least).
* **3rd party libraries**: You may use any third-party libraries you wish, but please provide instructions on how to install them (can be a link to their docs) if relevant.

## Bonus Points ⭐

These are not required, but we think these could be interesting additions to your solution:

1. Add functionality to dynamically switch processing algorithms on/off during runtime based on user input.
1. Pass some information between the processing algorithms (e.g. the area of the detected circle in one process is passed to another process which applies some algorithm on this area only).
1. Add a GUI to the application for easier interaction.

## Deliverables 📦

Please provide the following:

1. A link to a public Git repository with your solution.
1. A README file with instructions on how to compile and run your solution.
1. A brief explanation of your design choices and any assumptions you made.
1. At the interview, be prepared to showcase your solution live and explain your thought process.

**Simply send us an email with the link to your solution at [roland@teton.ai](mailto:roland@teton.ai) when you're ready to submit.**
