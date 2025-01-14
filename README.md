Facial Recognition App on AWS
This project is a facial recognition system built using AWS services as Amazon Rekognition, AWS Lambda, Amazon S3, DynamoDB, and API Gateway, along with a React front-end. The application consists of two main flows:
<img src="https://github.com/user-attachments/assets/f837549a-d673-4fc3-bdd3-a8d84601cf95" width="800"/>
Registration Flow: Employee images are uploaded to an S3 bucket, triggering a Lambda function to process the image using Rekognition, which indexes the face and stores the information in DynamoDB.

Authentication Flow: Visitors or employees can upload an image for recognition via the React front-end, which triggers an API Gateway. The image is processed by a Lambda function using Rekognition to match the face with those indexed in DynamoDB.
