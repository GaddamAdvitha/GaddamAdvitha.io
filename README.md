Email Marketing Application Using AWS Lambda, SES, S3, and EventBridge
Overview

This project is an automated email marketing solution leveraging AWS services such as Lambda, Simple Email Service (SES), Simple Storage Service (S3), and EventBridge. The application sends personalized emails to a list of contacts stored in an S3 bucket, using an HTML email template also stored in S3. The Lambda function, triggered automatically via AWS EventBridge, processes the contact list and sends out the emails through SES.

The project is deployed and managed via GitHub, with the front end hosted on GitHub Pages.

Features

    Automated Email Sending: Sends personalized emails to contacts using AWS Lambda and SES.
    Event-Driven Execution: Utilizes AWS EventBridge to schedule and trigger the Lambda function automatically.
    HTML Email Templates: Customizable HTML templates for email formatting.
    S3 Integration: Stores the contact list and email template in an S3 bucket.
    SES Identity Management: Manages sender and recipient identities in AWS SES.
    Deployed on GitHub Pages: The project domain and front-end hosting are managed via GitHub Pages.

What I Did
1. Set Up GitHub Pages

    Domain Setup: I hosted the project's frontend on GitHub Pages, enabling a domain for easy access and management of the email template.

2. Created and Configured AWS S3 Buckets

    S3 Bucket: I created an S3 bucket named email-marketing-appli.
    Stored Files: Uploaded contacts.csv containing the email list and index.html with the HTML content of the email to the S3 bucket.
   
4. Developed the Lambda Function

    Lambda Function: I wrote a Python Lambda function that:
        Retrieves the contacts.csv and email_template.html from the S3 bucket.
        Parses the CSV file to personalize the email template for each contact.
        Sends the personalized emails using AWS SES.
    Error Handling: The function includes error handling to manage issues like missing files or unverified email addresses.
ChatGPT

Got it! Here's the README tailored to reflect what you've done in the project:
Email Marketing Application Using AWS Lambda, SES, S3, and EventBridge
Overview

This project is an automated email marketing solution built using AWS services like Lambda, SES, S3, and EventBridge. The application sends personalized emails to a list of contacts stored in an S3 bucket, using an HTML email template also stored in S3. The Lambda function is triggered automatically through AWS EventBridge. The front end is hosted on GitHub Pages, where I managed the project domain.
What I Did
1. Set Up GitHub Pages

    Domain Setup: I hosted the project's frontend on GitHub Pages, enabling a domain for easy access and management of the email template.

2. Created and Configured AWS S3 Buckets

    S3 Bucket: I created an S3 bucket named email-marketing-appli.
    Stored Files: Uploaded contacts.csv containing the email list and email_template.html with the HTML content of the email to the S3 bucket.

3. Developed the Lambda Function

    Lambda Function: I wrote a Python Lambda function that:
        Retrieves the contacts.csv and email_template.html from the S3 bucket.
        Parses the CSV file to personalize the email template for each contact.
        Sends the personalized emails using AWS SES.
    Error Handling: The function includes error handling to manage issues like missing files or unverified email addresses.

4. Configured AWS SES

    Verified Email Identities: Verified the email addresses in AWS SES to ensure that emails could be sent from the specified address and received by the recipients.

5. Scheduled Lambda Execution with EventBridge

    EventBridge Rule: Set up an AWS EventBridge rule to trigger the Lambda function at scheduled intervals, automating the email-sending process.

6. Tested the Workflow

    Manual Testing: Executed the Lambda function manually to ensure emails were sent successfully.
    Proof of Concept: Captured logs and screenshots showing successful email delivery to the specified email IDs in contacts.csv.

1. Email Template Hosted on GitHub Pages: ![image](https://github.com/user-attachments/assets/efe81d11-e935-44e3-95ce-acd0f1c84b20)

2. SES Verified Identities: ![image](https://github.com/user-attachments/assets/5856d881-0523-48ae-88b8-8409d4a377c0)

3. Successful Lambda Execution: ![image](https://github.com/user-attachments/assets/1cda56dd-127f-4559-87af-9fba95a3e926)

4. Emails Received: ![image](https://github.com/user-attachments/assets/f771ee18-51fa-4f04-b56a-c904281023e9)
