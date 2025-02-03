# NBA Game Day Notifications / Sports Alerts System

### Project Overview
This project is an alert system that sends real-time NBA game day score notifications to subscribed users via SMS/Email. It leverages Amazon SNS, AWS Lambda and Python, Amazon EvenBridge and NBA APIs to provide sports fans with up-to-date game information. The project demonstrates cloud computing principles and efficient notification mechanisms.

 ### Features
- Fetches live NBA game scores using an external API.
- Sends formatted score updates to subscribers via SMS/Email using Amazon SNS.
- Scheduled automation for regular updates using Amazon EventBridge.
- Designed with security in mind, following the principle of least privilege for IAM roles.
  
### Prerequisites
- Free account with subscription and API Key at <a href="https://sportsdata.io/">here</a>
- Personal AWS account with basic understanding of AWS and Python

### Technical Architecture
![image](https://github.com/user-attachments/assets/ff6f0e81-c188-4981-9403-c3e0bc777158)

## Technologies
- **Cloud Provider**: AWS
- **Core Services**: SNS, Lambda, EventBridge
- **External API**: NBA Game API (SportsData.io)
- **Programming Language**: Python 3.x
- **IAM Security**:
 - `Least privilege policies for Lambda, SNS, and EventBridge.`
 
## Project Structure

```plaintext
game-day-notifications/
├── src/
│   ├── gd_notifications.py          # Main Lambda function code
├── policies/
│   ├── gb_sns_policy.json           # SNS publishing permissions
│   ├── gd_eventbridge_policy.json   # EventBridge to Lambda permissions
│   └── gd_lambda_policy.json        # Lambda execution role permissions
├── .gitignore
└── README.md                        # Project documentation

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
## Clone the repository
```bash
git clone https://github.com/aminatanimashaun31/gameday-notifications.git
```
## Create an SNS Topic
1. Open the AWS Management Console.
2. Navigate to the SNS service.
3. Click Create Topic and select Standard as the topic type.
4. Name the topic (e.g., gd_topic) and note the ARN.
5. Click Create Topic.
 ![image](https://github.com/user-attachments/assets/3c27cc14-fe24-4971-b897-f1d2b8176a3b)

## Add Subscriptions to the SNS Topic
1. After creating the topic, click on the topic name from the list.
2. Navigate to the Subscriptions tab and click Create subscription.
3. Select a Protocol:
- **For Email:**
  - Choose Email.
  - Enter a valid email address.

- **For SMS (phone number):**
  - Choose SMS.
  - Enter a valid phone number in international format (e.g., +1234567890).
4. Click Create Subscription.
5. If you added an Email subscription:
- Check the inbox of the provided email address.
- Confirm the subscription by clicking the confirmation link in the email.
6. For SMS, the subscription will be immediately active after creation.



4. Run the application
```bash
python src/weather_dashboard.py
```
![image](https://github.com/user-attachments/assets/873b198d-ec2f-4a48-a095-be94d2fd0c68)
### **Weather Dashboard: AWS S3 Bucket Overview**
The following screenshot shows the configured S3 bucket (`weather-data-aminat`) that stores the weather data collected during this project.
![image](https://github.com/user-attachments/assets/b442d41e-3cf0-4e7d-bbd2-9e91b6444877)

![image](https://github.com/user-attachments/assets/0ab83386-1bfd-4d0a-a2d1-1ec0e3f6915a)

