# AWSProject1
Neat diagram of project architechture of the project 

![Architecture Diagram](new.drawio.png)

OVERVIEW
This project demonstrates the integration of AWS Polly, a service that converts text into lifelike speech. The project is designed to [create audio versions of textual content].

FEATURE
*Text-to-Speech Conversion: Converts input text files to audio using AWS Polly.
*S3 Integration: Stores input text files and output audio files in AWS S3.
*Automated Workflow: AWS Lambda automates the process upon file upload.
*Multiple Voice Options: Supports various voices.

ARCHITECTURE

*S3 Bucket: Receives text files and stores the output audio files.
*AWS Lambda: Triggers AWS Polly to convert text to speech.
*AWS Polly: Processes text files and generates audio files.

SET UP AWS RESOURCES

*S3 Bucket: Create an S3 bucket to store input and output files.
*IAM Role: Set up an IAM role with permissions for Polly, S3, and Lambda.
*AWS Lambda: Deploy the Lambda function to process S3 events.
*Python script: write a python code contains json to interact with the polly and test in lambd environment

CONFIGURATION
AWS Configuration:

*Add your S3 bucket name, region, and other configurations in the environment variables.
*Configure Polly's voice settings in the Lambda function.
*Environment Variables:

Set up environment variables in AWS Lambda for the S3 bucket and Polly configurations.

ROADMAP
*Add support for more languages.
*Implement real-time conversion.
*Integrate with a web interface for user uploads.

ACKNOWLEDGEMENT
*AWS Polly for the amazing text-to-speech service.
*AWS lambda
*IAM Role
