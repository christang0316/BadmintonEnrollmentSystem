# Badminton Court Enrollment System - LINE Bot

## Overview

This project is a **LINE Bot** designed to manage the reservation and enrollment system for the badminton courts at our campus. Since our campus has only four badminton courts, students often struggle to secure a court after classes due to the high demand. The goal of this bot is to create an efficient and fair system that allows students to easily enroll in available courts, track their turn, and enjoy their game without any hassle.

## Features

- **Real-Time Court Enrollment:** Students can enroll in any of the four courts through the LINE Bot by simply sending a message. The system will automatically manage their position in the queue.
- **Court Status Tracking:** Users can check how many people are currently waiting for a specific court, and the system will update in real-time as students enroll or leave.
- **Queue Management:** The system tracks who is currently playing on the court, and when their turn is over, the bot will notify the next person in the queue.
- **Admin Controls:** Certain users (like administrators) can manage the queue, clear enrollments, and call the next person in line for any court.

## Key Functionalities

- **Enroll to Play:** Users can enroll for any court (A, B, C, or D) by sending a simple command like `A+1`. The bot handles everything from adding the user to the queue to notifying them when it’s their turn to play.
- **View Court Status:** Users can check how many people are currently waiting for each court and see if any courts are available.
- **Cancel Enrollment:** If a user decides to cancel their enrollment, they can do so easily via the bot.
- **Call Next Player:** When a game is over, the bot can call the next player in the queue to take the court.

## Why This Project?

The idea behind this project was born out of necessity. Our campus only has four badminton courts, and with a high demand for them after class, it was becoming chaotic to organize games fairly. The manual method of signing up was inefficient and led to confusion and missed turns. By automating this process with a LINE Bot, students can focus on playing while the system handles the rest.

## Technology Stack

- **LINE Messaging API**: For interacting with users and managing conversations.
- **Google Apps Script**: Handles the backend logic, integrates with Google Sheets for real-time data tracking, and minimizes API call overhead.
- **Google Sheets**: Stores court enrollment data, user information, and queue management in a structured format.

## Installation & Setup

1. **Clone this repository** to your local machine.
2. **Set up a Google Apps Script project** to handle the backend logic (integrate with your Google Sheets).
3. **Configure the LINE Messaging API**:
   - Create a LINE Bot and obtain your `CHANNEL_ACCESS_TOKEN`.
   - Set up a Webhook URL that connects to your Google Apps Script.
4. **Modify the Google Sheets**:
   - Create a Google Sheet that will act as the database for managing enrollments, users, and courts.
5. **Deploy the Bot**:
   - Deploy your Google Apps Script to handle real-time interaction with users.
   - Ensure the bot is live and integrated with the LINE platform.

## Future Improvements

- **Automated Reminders:** Notify users a few minutes before their turn on the court.
- **Advanced Admin Controls:** Add more granular controls for admins, such as court-specific overrides and schedule management.
- **Multi-language Support:** Expand the bot to support multiple languages for a more inclusive user experience.

## Contributing

Feel free to fork this repository and submit pull requests with improvements. Contributions are welcome!

## License

This project is licensed under the MIT License.
