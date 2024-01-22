# Static-website-in-S3-accessed-with-Route53-DNS
![image](https://github.com/shaikshaz/Static-website-in-S3-accessed-with-Route53-DNS/assets/154241222/17429d3b-7084-4b9c-ac79-aba406a25d56)
SITUATION: I need to run my static website with the DNS name and store it on S3 bucket in AWS console.

TASK: The static website hosted on s3 should be routed through route53 in the aws console and the website domain should route through amazon rout 53 for DNS management.

ACTION: 
To host the static website on S3 first we need to create a S3 bucket on console “Create Bucket”, select a region.
-Configure bucket for static website Hosting set the bucket properties to have access to static website. E.g index.html
-Make s3 bucket public by giving the access through bucket policy.
- Upload static website files to the bucket once created.
- static website files are now stored in an S3 bucket and can be accessed via the S3 bucket URL.
ROUTE 53 configuration:
-The main purpose of rout53 is to provide DNS access to our static website to display the output page.
-Create a hosted zone create a name server like shazia.com and update the name server.
-Add a record set give an alias name and choose the bucket created as target so that when we run the DNS it should do to our S3 bucket content.
-In the backend the DNS gets registered and takes few minutes to update with our S3 bucket content.
-Once the resolution is done we can access out website with custom domain name .

RESULT: Static website is successfully hosted on Amazon S3, and its domain is routed through Amazon Route 53 for DNS management. We can now access our website using custom domain name.



