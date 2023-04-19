---
layout: default
---

## [Cloud Resume Challenge](https://cloudresumechallenge.dev/docs/the-challenge/aws/)

[Cloud Resume](https://www.jc-resume.xyz/)

---

[PendingUsername](https://github.com/PendingUsername): My Github with various projects, including my cloud resume. 

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

The Cloud Resume Challenge is a project created by Forrest Brazeal. This challenge is a great opportunity for individuals to enhance their skills and knowledge on AWS services, particularly on serverless computing. In this blog post, we will discuss the different tasks that one needs to accomplish to complete the Cloud Resume Challenge.

Step 1: Certification
> The first requirement for the Cloud Resume Challenge is to have an AWS Cloud Practitioner certification on your resume. This certification serves as an introductory course to AWS Cloud, which helps you understand the basics of cloud computing. I also took the Solutions Architect exam. It can be taken online for $100 USD, and there are exam prep resources available on Udemy. I recommend using the Udemy course by Stephan Maarek. Link to the course -> [Udemy Course](https://www.udemy.com/share/106WtA3@_RiQLhVwYmyeFFkFwb0fSmBa5YSOv_MmpoiV40vPi8znRpovdV_bI34Y1nmZZ7igPg==/)

Step2: HTML
> The second requirement is to create your resume using HTML. This means that your resume should not be in a Word document or PDF. You can use any text editor or Integrated Development Environment (IDE) to write your resume in HTML. There are several online resources that can help you learn HTML, such as W3Schools, MDN Web Docs, and Codecademy. I used an HTML5 template, editing it to meet my needs. WebDev has never been easier. 

Step 3: CSS
> Styling your resume with CSS is the third requirement of the Cloud Resume Challenge. This means that your resume should not only be in raw HTML but should also have a visually appealing design. You can use CSS to customize the font, color, layout, and other design elements of your resume. There are several online resources that can help you learn CSS, such as W3Schools, MDN Web Docs, and Codecademy.

Step 4: Static Website
> The fourth requirement is to deploy your HTML and CSS resume as a static website using Amazon S3. A static website is a type of website that only contains HTML, CSS, and JavaScript files and does not require any server-side processing. Amazon S3 is a storage service that allows you to host static websites at a low cost. There are several tutorials available online that can help you deploy your website using Amazon S3. Simply create a S3 bucket for your site and make the contents public. This video does a great job explaining the process and taught me a ton. [S3 + CloudFront](https://www.youtube.com/watch?v=mls8tiiI3uc&t=580s)

Step 5: HTTPS
> The fifth requirement is to use HTTPS for your S3 website URL. HTTPS is a secure protocol that encrypts the data transmitted between the website and the user's browser. To use HTTPS, you need to use Amazon CloudFront, a content delivery network (CDN) service that can distribute your website's content to users worldwide. There are several tutorials available online that can help you enable HTTPS for your S3 website using [CloudFront](https://www.youtube.com/watch?v=mls8tiiI3uc&t=580s).

Step 6: DNS
> The sixth requirement is to point a custom DNS domain name to the CloudFront distribution so that your resume can be accessed at a custom URL like my-c00l-resume-website.com. You can use Amazon Route 53 or any other DNS provider for this. Route 53 is a domain name system (DNS) service that allows you to register and manage domain names. There are several tutorials available online that can help you set up your custom DNS domain name using [Route 53](https://www.youtube.com/watch?v=mls8tiiI3uc&t=580s).

Step 7: Javascript
> The seventh requirement is to include a visitor counter on your website that displays how many people have accessed your site. To achieve this, you need to write a bit of JavaScript code that counts the number of visitors and displays it on the website. Create and index.js file, then call the script in your index.html. There are several tutorials available online that can help you add a visitor counter using JavaScript. Mine looked something like this: 

//counter
const counter = document.querySelector(".counter-number");
async function updateCounter() {
    let response = await fetch("lambda-url");
    let data = await response.json();
    counter.innerHTML = `Views: ${data}`;
}

updateCounter();

Step 8: Database
> The eighth requirement is to store the visitor counter data in a database. For this challenge, it is suggested that you use Amazon DynamoDB, a fully managed NoSQL database service that can store and retrieve any amount of data. There are several tutorials available online that can help you set up and use DynamoDB for this challenge. Simply create a database 

Step 9: API
> The ninth requirement is to create an API that accepts requests from your web app and communicates with the database. For this challenge, it is suggested that you use Amazon API Gateway and AWS Lambda. Make sure that the function is allowed to read and write to the database. This can be configured in the CORS settings. Here is my Lambda function:

Step 10: Python
> To complete the Cloud Resume Challenge, you will need to write code in the AWS Lambda function. While you could use more Javascript, it would be better for our purposes to explore Python, a common language used in back-end programs and scripts, and its boto3 library for AWS. If you are not familiar with Python, there are many free tutorials available online to get started.

Step 11: Tests
> It is important to include tests for your Python code to ensure it functions correctly. This helps catch any bugs or errors before deployment, which can save you time and headaches later. There are many resources available online to help you write good Python tests. Some important aspects of testing include covering edge cases, verifying expected behavior, and maintaining code coverage.

Step 12: Infrastructure as Code
> Manually configuring your API resources - the DynamoDB table, the API Gateway, and the Lambda function - by clicking around in the AWS console can be time-consuming and error-prone. Instead, it is better to define them in an AWS Serverless Application Model (SAM) template and deploy them using the AWS SAM CLI. This is called "infrastructure as code" (IaC) and can save you time in the long run. SAM is a great tool for AWS serverless APIs, but if you prefer to use Terraform, it is a more broadly applicable and commonly-used IaC tool in the industry.

Step 13: Source Control
> It is essential to use source control to manage your codebase effectively. By creating a GitHub repository for your backend code, you can track changes, collaborate with others, and ensure that you always have access to your code. Avoid updating your back-end API or your front-end website by making calls from your laptop; instead, use source control to update them automatically whenever you make a change to the code.

Step 14: CI/CD (Back end)
> Continuous integration and deployment (CI/CD) is an essential part of modern software development. To set up CI/CD for the back-end of your Cloud Resume Challenge, you can use GitHub Actions. Whenever you push an update to your Serverless Application Model template or Python code, your Python tests should get run. If the tests pass, the SAM application should get packaged and deployed to AWS.

Step 15: CI/CD (Front end)
> Create a second GitHub repository for your website code. Then, create GitHub Actions such that when you push new website code, the S3 bucket automatically gets updated. You may also need to invalidate your CloudFront cache in the code. It is crucial not to commit AWS credentials to source control, as bad actors could find them and use them against you.

Step 16: Blog Post
> Created this blog post to discuss what I learned.

In conclusion, the Cloud Resume Challenge is an excellent opportunity to gain experience in cloud technologies and showcase your skills to potential employers. By following these steps, you can complete the challenge and create a cloud-hosted resume website using various AWS services and best practices. Don't forget to focus on Python, testing, infrastructure as code, source control, and CI/CD for both the back-end and front-end.
