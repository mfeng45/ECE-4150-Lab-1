# Serverless Photo Gallery Application

This repository contains the code and instructions to create a serverless Photo Gallery application using AWS Lambda, API Gateway, S3, DynamoDB, and Cognito.

## Overview

The application utilizes the following AWS services:

- **S3**: For static website hosting and storing photos.
- **API Gateway**: To expose endpoints for backend services.
- **Lambda**: To handle backend business logic.
- **Cognito**: For user pool management and authentication.
- **DynamoDB**: For storing records of photos.

## Setup Instructions

Follow the steps below to set up the Photo Gallery application in your AWS account.

### 1. Create S3 Buckets

- **Static Website Hosting**: Create an S3 bucket to host the web interface (HTML and JS) of the application.
- **Photo Storage**: Create another S3 bucket to store photos uploaded by users.

### 2. Create DynamoDB Table

- Create a DynamoDB table to store metadata and records of photos.

### 3. Create Cognito User Pool

- Set up a Cognito User Pool to manage user registration and authentication.

### 4. Create IAM Roles

- Create IAM roles with the necessary permissions to access the S3 buckets, DynamoDB table, and other AWS resources.

### 5. Review and Update Python Files

- Review `login.py`, `signup.py`, and `confirmemail.py`.
- Update the `<USER_POOL_ID>` and `<CLIENT_ID>` placeholders with your Cognito User Pool ID and Client ID.

### 6. Create Lambda Functions

- Write and deploy the Lambda functions to handle the backend logic.

### 7. Create API Gateway

- Create a new API in API Gateway and integrate it with the Lambda functions.

### 8. Update Website Script

- In the `process.js` file, update the `<API_URL>` with your API Gateway URL and `<PHOTOGALLERY_S3_BUCKET_NAME>` with your S3 bucket name for storing photos.

### 9. Deploy the Static Website

- Upload the web interface files to the S3 bucket configured for static website hosting.

### 10. Access the Photo Gallery Application

- Open the URL of the static website in a browser.

## Usage Instructions

1. **Sign Up**: 
   - Navigate to the signup page and create a new user account.

2. **Confirm Email**:
   - Confirm the user's email address.

3. **Login**:
   - Log in using the created user account.

4. **Add Photos**:
   - Go to the add photos page and upload new photos.

5. **Browse and Search Photos**:
   - Browse and search for photos within the application.

## License

This project belongs to Georgia Institute of Technology
