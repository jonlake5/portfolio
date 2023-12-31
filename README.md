# Portfolio

This github repo serves as my portfoloio of projects, scripts, and other bits of information regarding my technical background, expreiences, and certifications.

# About

Hello, my name is Jonathan Lake. I am a cloud enginer (AWS and Azure) with software development experience. You can view my [resume](/Resume.md) to understand more of what I have worked on throughout my professional career.
I have experience working in different verticals including healthcare, finance, manufacturing, and transportation.
I am passionate about utilizing cloud services such as AWS and Azure to improve business operations and building solutions that will help customers succeed in solving their problems.

# Certifications

## AWS

![aws-certified-solutions-architect-professional 150x150](/images/aws-certified-solutions-architect-professional-150x150.png)
![aws-certified-solutions-architect-associate](/images/aws-certified-solutions-architect-associate-150x150.png)

## Azure

![azure-certified-administrator](/images/microsoft-certified-associate-badge.png)

# Projects

## Chatbot

Use case:
This client wanted to have a ChatBot functionality on their webpage. A small icon on the bottom right that when clicked would open a chatbot. The chatbot back end was developed with Amazon Lex.
It opened an embedded iframe that was hosted on S3 with CloudFront.
It had pre-programmed phrases to send to the chat bot, in addition to being able to type in any message desired.

Front End:

- HTML
- CSS
- JavaScript

Backend:

- Amazon Lex
- API Gateway

## Call Recording Search

Use case:

The hosted telephony system in-use only kept recorded calls for up to 1 year. The regulations of this organization required call recordings to be kept for 7 years.
I utilized the IP Telephony's ability to upload directly to Amazon S3. Upon upload, a lambda function was called to update the database with the metadata of the file.

On the front end, users that are permitted to log in and query the database were created in AWS Cognito. From this login they could search for and retrieve wav files of the recorded calls based on the call metadata stored in the database.

Backend:

- Python
- Lambda
- API Gateway
- RDS Aurora

Front End:

- Javascript
- HTML
- CSS
- Cognito for Authentication

[Git Repo](https://github.com/jonlake5/five9_call_archiving)

Solution Diagram:

![Solution Diagram](/images/call-recording.png)

# Programming examples

## AWS Identity Center User Management

Description: Once enabling AWS Identity Center to be federated to a 3rd party IDP (Azure AD in this example) there isn't any option to add users to groups or add new users if SCIM isn't implemented to populate the users from the IDP. These were created to easily allow users to be added to groups or to Identity Center.

[addUserToGroup.py](https://github.com/jonlake5/pbUtilities/blob/6196740f21df69b9ed6907d1472fbff1d0b448f0/addUserToGroup.py)

[addUserToIdentityCenter.py](https://github.com/jonlake5/pbUtilities/blob/6196740f21df69b9ed6907d1472fbff1d0b448f0/addUserToIdentityCenter.py)
