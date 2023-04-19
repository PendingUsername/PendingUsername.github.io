---
layout: default
---

## Cloud Resume Challenge(https://cloudresumechallenge.dev/docs/the-challenge/aws/)

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

------------------

## The Challenge

The Cloud Resume Challenge is a project created by Forrest Brazeal, an AWS Serverless Hero. This challenge is a great opportunity for individuals to enhance their skills and knowledge on AWS services, particularly on serverless computing. In this blog post, we will discuss the different tasks that one needs to accomplish to complete the Cloud Resume Challenge.

Certification
The first requirement for the Cloud Resume Challenge is to have an AWS Cloud Practitioner certification on your resume. This certification serves as an introductory course to AWS Cloud, which helps you understand the basics of cloud computing. It can be taken online for $100 USD, and there are exam prep resources available on A Cloud Guru.

HTML
The second requirement is to create your resume using HTML. This means that your resume should not be in a Word document or PDF. You can use any text editor or Integrated Development Environment (IDE) to write your resume in HTML. There are several online resources that can help you learn HTML, such as W3Schools, MDN Web Docs, and Codecademy.

CSS
Styling your resume with CSS is the third requirement of the Cloud Resume Challenge. This means that your resume should not only be in raw HTML but should also have a visually appealing design. You can use CSS to customize the font, color, layout, and other design elements of your resume. There are several online resources that can help you learn CSS, such as W3Schools, MDN Web Docs, and Codecademy.

Static Website
The fourth requirement is to deploy your HTML and CSS resume as a static website using Amazon S3. A static website is a type of website that only contains HTML, CSS, and JavaScript files and does not require any server-side processing. Amazon S3 is a storage service that allows you to host static websites at a low cost. There are several tutorials available online that can help you deploy your website using Amazon S3.

HTTPS
The fifth requirement is to use HTTPS for your S3 website URL. HTTPS is a secure protocol that encrypts the data transmitted between the website and the user's browser. To use HTTPS, you need to use Amazon CloudFront, a content delivery network (CDN) service that can distribute your website's content to users worldwide. There are several tutorials available online that can help you enable HTTPS for your S3 website using CloudFront.

DNS
The sixth requirement is to point a custom DNS domain name to the CloudFront distribution so that your resume can be accessed at a custom URL like my-c00l-resume-website.com. You can use Amazon Route 53 or any other DNS provider for this. Route 53 is a domain name system (DNS) service that allows you to register and manage domain names. There are several tutorials available online that can help you set up your custom DNS domain name using Route 53.

Javascript
The seventh requirement is to include a visitor counter on your website that displays how many people have accessed your site. To achieve this, you need to write a bit of JavaScript code that counts the number of visitors and displays it on the website. There are several tutorials available online that can help you add a visitor counter using JavaScript.

Database
The eighth requirement is to store the visitor counter data in a database. For this challenge, it is suggested that you use Amazon DynamoDB, a fully managed NoSQL database service that can store and retrieve any amount of data. There are several tutorials available online that can help you set up and use DynamoDB for this challenge.

API
The ninth requirement is to create an API that accepts requests from your web app and communicates with the database. For this challenge, it is suggested that you use Amazon API Gateway and AWS Lambda. Amazon
