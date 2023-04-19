---
layout: default
---

## Cloud Resume Challenge 

[Cloud Resume](https://www.jc-resume.xyz/)

---

[PendingUsername](https://github.com/PendingUsername) My Github with various projects, including my cloud resume. 

Technologies Used
------------------
S3:
> Amazon S3 is used to store the static content of the website, including HTML, CSS, JavaScript, and image files. The S3 bucket also serves as the origin for AWS CloudFront.

AWS CloudFront:
> AWS CloudFront is used as a content delivery network (CDN) to improve the site's performance and speed. CloudFront caches and delivers content from the S3 bucket to the user's browser.

Certificate Manager:
> AWS Certificate Manager (ACM) is used to provision and manage SSL/TLS certificates for the website. ACM makes it easy to obtain and manage SSL certificates to secure website traffic.

AWS Lambda:
> AWS Lambda is used to implement serverless functions that perform various tasks, such as sending emails, processing contact form submissions, and performing database queries.

DynamoDB:
> DynamoDB is used to store data associated with the website, such as user information and contact form submissions. The data is accessed and manipulated using AWS Lambda functions.

GitHub Actions:
> GitHub Actions is used for continuous integration and deployment of the website. The site is automatically built and deployed to S3 and CloudFront when new changes are pushed to the master branch.

Python and Java:
> Python and Java are the primary programming languages used to develop the site's functionality. Python is used for serverless functions, while Java is used for the backend API.

CSS and HTML:
> CSS and HTML are used for the site's styling and structure, respectively. The site uses modern CSS techniques and responsive design to ensure the site looks great on all devices.

Route 53:
> Amazon Route 53 is used for DNS management for the website. It ensures that the website is accessible using a custom domain name.

