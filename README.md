# 30 Days DevOps Challenge - Weather Dashboard
 
 Day 1: Building a weather data collection system using AWS S3 and OpenWeather API

## Weather Data Collection System - DevOps Day 1 Challenge
### Project Overview
This project is a Weather Data Collection System that demonstrates core DevOps principles by combining:

 - **External API Integration** (OpenWeather API)
- **Cloud Storage** (AWS S3)
- **Infrastructure as Code**
- **Version Control** (Git)
- **Python Development**
- **Error Handling**
- **Environment Management**
### Features
- Fetches real-time weather data for multiple cities
- Displays temperature (°F), humidity, and weather conditions
- Automatically stores weather data in AWS S3
- Supports multiple cities tracking
- Timestamps all data for historical tracking
### Technical Architecture
![image](https://github.com/user-attachments/assets/c61285e7-c86d-4761-864c-539e2aecb944)
## Technologies
 - **Language**: Python 3.x
- **Cloud Provider**: AWS (S3)
- **External API**: OpenWeather API
- **Dependencies**: 
  - `boto3` (AWS SDK)
  - `python-dotenv`
  - `requests`
 
## Project Structure

```plaintext
weather-dashboard/
    src/
        __init__.py
        weather_dashboard.py
    tests/
    data/
    .env
    .gitignore
    requirements.txt

```
## What I Learned

- AWS S3 bucket creation and management
- Environment variable management for secure API keys
- Python best practices for API integration
- Git workflow for project development**
- Error handling in distributed systems
- Cloud resource management
## Future Enhancements
- Add weather forecasting
- Implement data visualization
- Add more cities
- Create automated testing
- Set up CI/CD pipeline
## How to navigate all of it as a beginner
### Prerequisites
Before you can work on the project, you need to have certain things setup on your local machine. This includes but not limited to the following:
- **VS code Editor** you can see documentation <a href="https://code.visualstudio.com/download" target="_blank">here</a>
- **AWS CLI** Installed you can see documentation <a href="https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html" target="_blank">here</a>

Next, you configure your AWS CLI with the ACCESS KEY ID and ACCESS SECRET KEY gotten from your AWS console IAM USER by doing:
```bash
aws configure
```
## Setup Instructions
1. Clone the repository
```bash
git clone https://github.com/aminatanimashaun31/weather-dashboard.git
```
2. Install dependencies
```bash
pip install -r requirements.txt
```
3. Configure environment variables (.env):
```bash
OPENWEATHER_API_KEY=your_api_key
AWS_BUCKET_NAME=your_bucket_name
```
4. Run the application
```bash
python src/weather_dashboard.py
```
![image](https://github.com/user-attachments/assets/873b198d-ec2f-4a48-a095-be94d2fd0c68)
### **Weather Dashboard: AWS S3 Bucket Overview**
The following screenshot shows the configured S3 bucket (`weather-data-aminat`) that stores the weather data collected during this project.
![image](https://github.com/user-attachments/assets/b442d41e-3cf0-4e7d-bbd2-9e91b6444877)

![image](https://github.com/user-attachments/assets/0ab83386-1bfd-4d0a-a2d1-1ec0e3f6915a)

