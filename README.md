flask-s3
========

Seamlessly serve the static assets of your Flask app from Amazon S3.

Fork
-----------

Forking this repo for several reasons:

- Using it in combination with Flask-Assets and want to retain the basic integration
- I use CloudFront, which accesses S3 through an [Origin Access Identity](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/private-content-restricting-access-to-s3.html)
  and wanted to upload my files without a **public** ACL.
- Leverage boto3 credential discovery to fully leverage IAM access control.
  (e.g. Local creds, AWS Lambda SDS creds, EC2 Metadata Service... all without configuration changes)

Ultimately, I've simplified the code a bit for my specific use case... mostly assuming the S3 Bucket exists,
removing all credential discovery and all noodling with bucket/object ACL.

Installation
------------

Install Flask-S3 (forked version) via github:

    pip install git+ssh://git@github.com/abigperson/flask-s3.git#Egg=Flask-S3

Documentation (original)
------------------------
The latest documentation for Flask-S3 can be found [here](https://flask-s3.readthedocs.io/en/latest/).
