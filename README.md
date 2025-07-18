# Stopwatch-clock-application
Stopwatch & Clock Application (IST)

A simple C++ console application that functions both as a stopwatch and a real-time clock. The current time is displayed in Indian Standard Time (IST), and the stopwatch allows users to start, stop, and reset the elapsed time.

Features

⏰ Current IST Clock: Displays the real-time Indian Standard Time (UTC +5:30).
⏱ Stopwatch Functionality:
Start stopwatch
Stop stopwatch
Reset stopwatch
📋 Menu-driven interface: Easy-to-use numbered menu.
⏳ Accurate time tracking using C++11 chrono and thread.

Technologies Used

C++11
<chrono> for time measurement
<ctime> for current time
<thread> for adding delays

Stopwatch Logic:
Uses steady_clock::now() to get high-resolution time points.
Tracks elapsed time using duration<double> and stores cumulative result.
Controlled via boolean running flag to determine start/stop states.

Notes

The application delays by 5 seconds after each loop (this_thread::sleep_for(milliseconds(5000))) for a cleaner output.
The program runs in a loop until the user selects option 5 (Exit).
Works in IST even if the computer is set to another timezone.
