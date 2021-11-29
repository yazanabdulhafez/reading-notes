# Amazon S3

## What is Amazon S3?

* Amazon Simple Storage Service.
* (Amazon S3) is an object storage service.

## How Amazon S3 works

Its a object storage service store the data in Buckets and to do this we need to do the following:

1. create a bucket and specify a bucket name and AWS Region
2. upload the data to that bucket

### S3 features

1. we can use S3 Versioning (multiple versions of Bucket)
2. Buckets and the objects they are private (accessed when user authenticated)

### Topics in S3

* Buckets:its is a container for the objects stored in Amazon S3
* Objects: its the fundamental entities that stored in S3
* Keys: unique identifier for an object and every single object have only one key
* S3 Versioning:we use it to keep multiple variants of an object in the same bucket
* Version ID: Amazon S3 generates an ID for every object added to the Bucket
* Bucket policy: it used to grant access permissions to our bucket and the objects in it
* Access control lists (ACLs): its an access control mechanism
* Regions:we can choose the geographical AWS Region where Amazon S3 will store the buckets that we create.

## Amazon S3 data consistency model

Amazon S3 provides strong read-after-write consistency for PUT and DELETE requests of objects for all Buckets in all regions.

## Related services

1. Amazon Elastic Compute Cloud (Amazon EC2)
2. Amazon EMR
3. AWS Snow Family
4. AWS Transfer Family

## Accessing Amazon S3

we can access Amazon S3 by many ways:

1. AWS Management Console
2. AWS Command Line Interface
3. AWS SDKs
4. Amazon S3 REST API

## Paying for Amazon S3

* Pricing for Amazon S3 is designed so the storage requirements of the applications not need to plan for it. also Amazon S3 make you pay just when you use something with no hidden fees and not higher charges.

## PCI DSS compliance

Payment Card Industry (PCI)
Data Security Standard (DSS).

## Provision backend storage

* To start provisioning storage resources in the backend, go to your project directory and execute the command:**amplify add storage**

* After complete the setup you can push your changes to the cloud, execute the command:**amplify push**

## Install Amplify Libraries

* Add these libraries into the dependencies block:

1. implementation 'com.amplifyframework:aws-storage-s3:1.30.0'
2. implementation 'com.amplifyframework:aws-auth-cognito:1.30.0'

* aws-auth-cognito is used to provide authentication for Amazon S3 then click sync now.

## Initialize Amplify Storage

To initialize the Amplify Auth and Storage categories we call Amplify.addPlugin() method.

## Uploading data to your bucket

To upload to S3 from a data object, specify the key and the data object to be uploaded.

## Resources used in this reading

1. [What is Amazon S3?](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html)
2. [STORAGE](https://docs.amplify.aws/lib/storage/getting-started/q/platform/android/)
