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



S3 Billing 
---------------
1. storage
2. Requests
3. Storage management pricing 
4. Data transfer pricing 
5. Transfer acceleration
6. Cross region replication pricing 

Read S3 FAQs.
