# brilliant-cafe
Brilliant-Cafe is where I am currently hosting my professional portfolio such as it is. This started with a project I created to implement Tetris in JavaScript. My GitHub repository for that project is [https://github.com/peterjirak/tetris-frontend](peterjirak/tetris-frontend). My implementation is fully working but it is not fully finished.

After getting the code working, I wanted to deploy it so other people could play my implementation of Tetris such as it is. So I deployed my Tetris implementation using AWS serverless static web content hosting. I own the domain [brilliant.cafe](https://www.brilliant.cafe), so I set up a [static website on Amazon S3](https://docs.aws.amazon.com/AmazonS3/latest/userguide/HostingWebsiteOnS3Setup.html). Next I used [CloudFront to serve my static website hosted on Amazon S3](https://repost.aws/knowledge-center/cloudfront-serve-static-website). While hosting a static website in S3 does not support SSL/TLS certificates and HTTPS, once one is using CloudFront to serve one's static website hosted on S3. So, after using CloudFront to serve my static website hosted on Amazon S3, I was then able to require HTTPS for communication between a user's web browser and my deployment in CloudFront.

This used the following AWS services:
 * Route 53
 * S3
 * 
 * CloudFront
 * Certificate Manager

Here are some documentation links on setting this up:
 * [Hosting a HTTPS website using AWS S3 and CloudFront posted on November 23, 2017 by Matt Burgess](https://medium.com/@itsmattburgess/hosting-a-https-website-using-aws-s3-and-cloudfront-ee6521df03b9#id_token=eyJhbGciOiJSUzI1NiIsImtpZCI6IjgyMjgzOGMxYzhiZjllZGNmMWY1MDUwNjYyZTU0YmNiMWFkYjViNWYiLCJ0eXAiOiJKV1QifQ.eyJpc3MiOiJodHRwczovL2FjY291bnRzLmdvb2dsZS5jb20iLCJuYmYiOjE2ODQ1MTk1NjEsImF1ZCI6IjIxNjI5NjAzNTgzNC1rMWs2cWUwNjBzMnRwMmEyamFtNGxqZGNtczAwc3R0Zy5hcHBzLmdvb2dsZXVzZXJjb250ZW50LmNvbSIsInN1YiI6IjExMDg2NDc5NDIwOTk1NDgyNTY3OSIsImVtYWlsIjoicGV0ZXIuamlyYWtAZ21haWwuY29tIiwiZW1haWxfdmVyaWZpZWQiOnRydWUsImF6cCI6IjIxNjI5NjAzNTgzNC1rMWs2cWUwNjBzMnRwMmEyamFtNGxqZGNtczAwc3R0Zy5hcHBzLmdvb2dsZXVzZXJjb250ZW50LmNvbSIsIm5hbWUiOiJQZXRlciBFbGRyaXRjaCIsInBpY3R1cmUiOiJodHRwczovL2xoMy5nb29nbGV1c2VyY29udGVudC5jb20vYS9BR05teXhZZFd1ZTV3N0c3WnktRWZOdkF2WV9BdGZaYVBzand0SXhYTzUxajNnPXM5Ni1jIiwiZ2l2ZW5fbmFtZSI6IlBldGVyIiwiZmFtaWx5X25hbWUiOiJFbGRyaXRjaCIsImlhdCI6MTY4NDUxOTg2MSwiZXhwIjoxNjg0NTIzNDYxLCJqdGkiOiIyZGM3ZmI4YTAwNzQ1OWU4N2QzMjZjOGIzYzNlZTI5OTZiNzVmOGI0In0.D46M8NlwHyQL1lvAoepwtJK8qIIkVS_Zrkm9NBfJoiMLbUJ6S-jUohZ9PZZnRiLt8EmkzJTaeYP23xyUa0poDjdOutijpVSZpjsP21APutnPYYA1uka8dCHFb0lNIIQ3BQEi1dfCVcCpvJctVnarwPgc01yG7vWLEGDWUSIJhAy4MQr0MfxBi2892EA_pkcNv7tYwAsc18ADEa7C0ycpyjWUbRX_5gVzBIjiXR7ISIdKE-8NSfj7EwTk4P2DQ2sd15nBukCQMLbmHzUX5H8lvT7dEZZwAL3PfhA-ZFIVZkTBz7m4-yKpK5Zi2sBS9uk3vG07ILdh8xfN2YQxMzCHsA)
 * [Tutorial: Configuring a static website on Amazon S3 | Amazon Documetation](https://docs.aws.amazon.com/AmazonS3/latest/userguide/HostingWebsiteOnS3Setup.html)
   * [How do I use CloudFront to serve a static website hosted on Amazon S3? | AWS re:Post](https://repost.aws/knowledge-center/cloudfront-serve-static-website)
   * [Requiring HTTPS for communication between viewers and CloudFront | Amazon Documetation](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/using-https-viewers-to-cloudfront.html)

I have deployed my most recent revisions to my implementation of Tetris. So now, you can [play Tetris](https://www.brilliant.cafe/games/tetris/index.html)

Note that it is fully working but not fully finished. Also it works in a computer's browser, but does not yet work on mobile.

My URL for the deployment of my most recent revisions of my Tetris imnplementation is: [https://www.brilliant.cafe/games/tetris/index.html](https://www.brilliant.cafe/games/tetris/index.html)

I wanted to deploy Tetris using the URL [https://www.brilliant.cafe/games/tetris/index.html](https://www.brilliant.cafe/games/tetris/index.html) which is where my Tetris implementation is hosted. I set up a basic about me page at the URL [brilliant.cafe](https://www.brilliant.cafe).

This repository is intended to track changes I may make to [brilliant.cafe](https://www.brilliant.cafe). Note that this repository has the path games/tetris, but that path is basically empty since I have that project in a different repository and so do not want to copy it into this repository. Note that git does provide some solutions for that like sub-repositories etc, but for now I just have the path there but nothing under it.
