# CloudFront: Optimizing Web Performance with Amazon CloudFront and S3 Integration

## Overview
In this project, I learned to use Amazon CloudFront to accelerate content delivery and reduce latency for web applications by configuring an Amazon S3 bucket as the origin and setting up a CloudFront distribution, enabling faster delivery of static content through a global network of edge locations.

## Steps

1. **Prepare the Content**
   - I first downloaded a sample photo and saved it to a folder on my computer.
   - Within the AWS management console, I searched for the S3 service and opened the console.
   - Once in the S3 console, I clicked _Create bucket_.


   ![Create A Bucket](Create-a-bucket.png)


   - When creating a bucket, I had to pick a unique S3 bucket name that has never been used before. In the image below, you'll see _jeaninebucket_. However, I had to go back and change it to _jeaninethebucket_ since the first name was already taken.


   ![Bucket Name](bucket-name.png)


   - I then set the permission settings for my bucket. I made slight changes to the default settings. First, enabled ACLs under _Object Ownership_, then deselected the check box next to "Block all public access" under _Blcok Public Access settings for this bucket_, and, last, I disabled Bucket Versioning, Default encryption, and advanced settings.


![Enable ACLs](acls-enabled.png)
![Make Public](make-public-acknowlege.png)
![Disable Additional Features](disable-additional-features.png)


   - The only thing left to do in this step was to click the orange _Create bucket_ button at the very bottom of the page.


![Create Bucket Button](create-bucket-button.png)

3. ****
   - 

4. ****
   - 

4.****
   - 

## Resources
- [Use an Amazon CloudFront distribution to serve a static website](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/getting-started-cloudfront-overview.html)
