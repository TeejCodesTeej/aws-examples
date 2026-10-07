# Introduction to S3

What is Object Storage (Object-based Storage)?
Object Storage is a data storage architecture that manages data as objects as opposed to other storage architectures.

* Unlimited Storage
* Don't need to think about the underlying infrastructure
* The S3 Conole provides a way for you to upload and access your data

## Important Concepts

### S3 Object

Object contain the data that you upload. They're like files.

The object may consist of:

- `key` this is the name of the object
- `value` this is the data itself. Made up of a sequence of bytes.
- `version id` this is the version of the object if versioning is enabled. 
    - Versioning does cost money
- `Metadata` additional info attached to the object

### S3 Bucket

Buckets hold objects.  Can have folders for grouping.
S3 is a universal namespace so all buckets need to have a unique name.
You can store an individual object from 0 bytes to 5TB in size

# S3 Follow-along

