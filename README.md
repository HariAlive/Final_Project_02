# Final_Project_02
Title: Designing an Automatic Data Collection and Storage System with AWS Lambda and Slack Integration for Server Availability Monitoring and Slack Notification

Goal:

To create an AWS Lambda function that will periodically fetch data from an API and store it in an Amazon RDS instance. The function should be triggered by an Amazon CloudWatch Event that occurs every 15 seconds.

Technologies used:

AWS Lambda, Amazon DynamoDB, Amazon CloudWatch, Amazon EventBridge, Slack API

Steps:

1.	Set up an AWS Lambda function: Create an AWS Lambda function that will periodically check the availability of servers.
2.	Configure Lambda to store data in Amazon DynamoDB.
3.	Configure a CloudWatch event trigger to schedule the Lambda function to run periodically.
4.	Integrating a Slack bot and incoming webhook for your Slack workspace. 
5.	Modify Lambda function to send data to Slack: Modify the Lambda function to send a notification to Slack when a server is unavailable. You can use the Slack API to send a message to your Slack workspace via the incoming webhook.
6.	Test and Deploy: Test the Lambda function and Slack integration to ensure that server availability data is being collected and stored in S3, and notifications are being sent to Slack when a server is unavailable.
7.	Monitor and Maintain: Monitor the system to ensure it is running smoothly and make any necessary adjustments as needed

Slack integration:
For integrating slack, the following steps were followed
1.	Create a new slack App
2.	Add basic functionality and install the App 
3.	Copy the webhook URL and integrate it with the lambda function
4.	Your setup is done and the slack Api will launch your project with specific channel for automated message receipt
5.	For this project we have setup the slack Api as to receive error messages if the given URL is not accessible. For testing we used a 403 forbidden error fetching URL https://www.sec.gov/Archives/edgar/dailyindex/xbrl/companyfacts.zip

