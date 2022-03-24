## How to create bucket ?

1. give the bucket name (don't use space or uppercase)
2. select the region
3. Object ownership choose -> ACLs enabled or disabled
4. Block public access
5. Bucket versioning - disable or enable 
6. Tag - name - value 
7. Default encryption - server side encryption - enable or disable 
8. object locked - enable or disable 

then **create bucket**.
test-at-night bucket name.


What is ACL? why should we disable it ? 

After creating Bucket, there are some features. 
1.objects
2.properties
3.permissions
4.Metrics
5.Management
6.Access points 

Objects feature

1. Create folder 
2. go to folder, upload images or files.
3. After upload a image, we go to properties of image, copy the object url 
4. Hit the browser with url and it shows access denied
5. go to objects actions -> share with a presigned url for 10 minutes or hour. upto you.
6. copy the linke and hit the browser. 


The basics of S3
1. object based file storage 
2. size - 0 to 5 TB
3. unlimited storage
4. Files are stored in Buckets.
5. universal namespace. name must be unique globally
6. when upload a file s3, sender receiver **HTTP 200 code** if upload was successful.
7. S3 is object based. 
Object have:
1. key
2. value
3. versioning (version id)
4. Metadata (Data about data )
5. access control list.

S3 data consistency
-----------------------
1. if you write a file and read it immediately, you will able to view the data
2. if we update existing file or image or anyting, we can view latest updated data or file. 
3. if we delete the latest version, then it will show older version.


S3 features
------------
1. tiered storage available.
2. lifecycle management 
3. versionning
4. encrytion
5. MFA delete
6. secure your data using access control list and bucket policies 

S3 Storage classes
-----------------
1. S3 Standard
2. S3 - IA
3. S3 One Zone - IA
4. S3 - intelligent Tiering
5. S3 Glacier
6. S3 Glacier Deep Archieve

What are different tiers?

S3 Standard 
==============
most expensive
1. General purpose storage
2. used for frequently accessed data.
3. first 50 TB / Month - $0.023 per GB, Next 450 TB /Month - $0.022 per GB, Over 500 TB / Month - $0.021 per GB

S3 Intelligent-Tiering 
--------------------------
Best tier (recommended)
Automatic cost savings for data with unknown or changing access patterns.
frequent access tier, first 50 TB / Month - $0.023 per GB
infrequent access tier, all storage /Month -$0.0125 per GB
Monitoring and Automation, All storgae /Month - $0.0025 per 1000 objects.

S3 Standard 
--------------
Infrequent access - For long lived but infrequently accessed data that needs ms access.
All storage /Month - $0.0125 per GB

S3 One Zone
-------------------
Infrequent access - $0.01 per GB

S3 Glacier
-------------
long-term backup and archieves with retrieval option from 1 min to 12 hours - $0.004 per GB
S3 Glacier Deep Archieve 
------------------------
- For long-term data archiving that is accessed once or twice in a year can be restored within 12 hours.
price - all storage / month - $0.00099 per GB

S3 Billing 
---------------
1. storage
2. Requests
3. Storage management pricing 
4. Data transfer pricing 
5. Transfer acceleration
6. Cross region replication pricing 

S3 security and encryption
--------------------------------
1. All newly created buckets are **private**
Encryption in transit is achieved by
1. SSL/TLS - client side encryption

Server-side encryption
------------------------
S3 Encryption Key type
--------------------------------
1. S3 managed keys - SSE-S3 - An encryption key that Amazon S3 creates, manages, and uses for you
2. AWS key management service, SSE-KMS - An encryption key protected by AWS Key Management Service (AWS KMS)
3. SSE-C

S3 - Versioning 
------------------------
1. backup tool.
2. stored all versions of objects.
3. versioning can't be disabled, only suspended.
4. integrates with **Lifecycle rules**

Lifecycle Management
---------------------------

1. automate moving your objects between the different object tiers.
2. can be used in conjunction with versioning.

Sharing S3 buckets Across Accounts
--------------------------------------
3 ways.
1. Using Bucket policies & IAM programmatic access only.
2. Using Bucket ACLs & IAM(individual objects). Programmatic access only.
3. Cross-Account IAM roles. programmatic and console access.
 
 Cross Region Replication
 -----------------------------
 1. cross region replication need versioning enabled.

S3 Transfer Acceleration
----------------------------
1. S3 Transfer Acceleration utilises the CloudFront Edge network to accelerate your uploads to S3.
2. without direct uploading to S3, we can use a object url to upload edge location.
3. Edge location later transfer that file to S3. 
4. 
 


Read S3 FAQs.
