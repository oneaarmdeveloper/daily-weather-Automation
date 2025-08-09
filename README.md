

# Weather Notification Automation with n8n

## Overview
This project demonstrates an automated workflow built using **n8n** (free plan) to fetch weather data from the OpenWeatherMap API on a scheduled basis and send email notifications. It showcases my skills in workflow automation, API integration, and basic data handling, developed as part of my continuous learning journey as a 2nd-year Azubi (Fachinformatiker für Anwendungsentwicklung) in Regensburg.

## Features
- **Scheduled Data Fetch**: Triggers daily to retrieve weather data.
- **API Integration**: Uses HTTP Request to pull data from OpenWeatherMap.
- **Email Notification**: Sends weather updates via email.
- **Scalable Design**: Can be extended with custom scripts or additional nodes.

## Tech Stack
- **n8n**: Workflow automation tool.
- **HTTP Request**: Fetches data from OpenWeatherMap API.
- **Schedule Trigger**: Automates execution.
- **Send Email**: Delivers notifications.
- **Optional Skills**: Python (for data processing), SQL (for logging), HTML/CSS/JS (for potential dashboard), OSINT (for weather-related trend monitoring).

## Setup Instructions
1. **Prerequisites**:
   - Install n8n locally (via Docker or Node.js) or use the free n8n cloud plan (app.n8n.cloud).
   - Obtain an API key from [OpenWeatherMap](https://openweathermap.org/api).
   - Set up an email account with SMTP credentials (e.g., Gmail with App Password).
2. **Import Workflow**:
   - Download the `workflow.json` file from this repository.
   - In n8n, go to **Settings > Import Workflow** and upload the `.json` file.
3. **Configure Nodes**:
   - **HTTP Request Node**: Update the API endpoint (e.g., `https://api.openweathermap.org/data/2.5/weather?q={city}&appid={YOUR_API_KEY}`) with your API key and desired city.
   - **Send Email Node**: Enter your SMTP server details (host, port, username, password) and recipient email.
4. **Activate and Test**:
   - Set the workflow to **Active** and click **Execute Workflow** to test.
   - Check the **Logs** tab for execution details.

## Usage
- The workflow runs daily once active  (configurable via the Schedule Trigger) and emails the latest weather data (e.g., temperature, conditions) for the specified city.
- Example output in email: "Current weather in Regensburg: 22°C, Sunny."

## Screenshots
"C:\Users\kason\OneDrive\Documents\ShareX\Screenshots\2025-08\brave_J7FLx0AxXd.png"

## Future Improvements
- **Data Processing**: Add a Python node to parse and format weather data (e.g., convert Kelvin to Celsius).
- **Database Logging**: Store weather data in a SQL database for trend analysis.
- **OSINT Integration**: Use OSINT techniques to monitor weather-related social media trends.
- **Dashboard**: Build a simple HTML/CSS/JS dashboard to visualize data.

## Limitations (Free Plan)
- Execution is limited by n8n's free tier quota. Test within these constraints.
- Sensitive data (e.g., API keys, email credentials) has been removed from the `.json` file for security.

## About Me
I am a 2nd-year Azubi (FIAE) in Regensburg, continuously learning and exploring automation, coding (HTML, CSS, JS, SQL, Bash, Python), and cybersecurity . This project reflects my interest in applying these skills to real-world automation challenges, 
such as those relevant to Organisations and Companies

## License
This project is open-source under the MIT License. Feel free to use, modify, and contribute!

## Contact
- GitHub: [Your GitHub Username](https://github.com/oneaarmdeveloper)

