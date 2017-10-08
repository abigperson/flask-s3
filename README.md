flask-s3
========

Seamlessly serve the static assets of your Flask app from Amazon S3.

Fork
-----------

Forking this repo for several reasons:

- Using it in combination with Flask-Assets and want to retain the basic integration
- Encapsulate other areas of my app where I am using S3 (potentially)
- Leverage boto3 credential discovery to fully leverage IAM access control.
  (e.g. Local creds, AWS Lambda SDS creds, EC2 Metadata Service... all without configuration changes)

Installation
------------

Install Flask-S3 (forked version) via github:

    pip install git+https://github.com/abigperson/flask-s3

Documentation (original)
------------------------
The latest documentation for Flask-S3 can be found [here](https://flask-s3.readthedocs.io/en/latest/).
