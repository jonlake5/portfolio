# Portfolio
This github repo serves as my portfoloio of projects, scripts, and other bits of information regarding my technical background, expreiences, and certifications.

# About
Hello, my name is Jonathan Lake. I am a cloud enginer with software development experience. I 

# Certifications
## AWS
![aws-certified-solutions-architect-professional 150x150](https://github.com/jonlake5/portfolio/assets/5898917/813047ac-2122-4b25-b15c-49b334777f75) ![aws-certified-solutions-architect-associate](https://github.com/jonlake5/portfolio/assets/5898917/6536846d-ea6a-48f6-aa1a-da87598cf64a)
![](/images/aws-certified-solutions-architect-professional-150x150.png)
# Projects

## Chatbot


## Call Recording Search
Use case:

The hosted telephony system in-use only kept recorded calls for up to 1 year. The regulations of this organization required call recordings to be kept for 7 years.
I utilized the IP Telephony's ability to upload directly to Amazon S3. Upon upload, a lambda function was called to update the database with the metadata of the file.

On the front end, users that are permitted to log in and query the database were created in AWS Cognito. From this login they could search for and retrieve wav files of the recorded calls based on the call metadata stored in the database. 

Backend:
* Python
* Lambda
* API Gateway
* RDS Aurora

Front End: 
* Javascript
* HTML
* CSS
* Cognito for Authentication

Solution Diagram
[Solution Diagram](/images/call-recording.png)