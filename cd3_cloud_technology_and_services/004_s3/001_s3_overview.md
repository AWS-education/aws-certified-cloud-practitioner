**Amazon S3**

- S3 - is a cloud-based object storage service

---

**Amazon S3 - Buckets**

- Amazon S3 allows people to store objects (files) in "buckets" (directories);
- Buckets are defined at the region level;
- Buckets assigned to a specific region;
- Naming:
  - Shared Global Namespace - have a globally unique name (accross all regions all accounts);
  - Account Regional Namespace - allows for "reuse" of the same bucket name accross regions;
- Naming constraints:
  - No uppercase, No underscore;
  - Not an IP;
  - Must start with the lowercase letter or number;
  - Must NOT start with the prefix `xn--`;
  - Must NOT end with the suffix `-s3alias`;

---

**Amazon S3 - Objects**

- Objects (files) have a Key;
- The `key` is the FULL path:
  - `s3://my-bucket/my_file.txt`;
  - `s3://my-bucket/my_folder/another_folder/my_file.txt`;
- The key is composed of _prefix_ + _object name_;
- There's no concent of "directories" within buckets;
  (although the UI will trick you to think otherwise)
- Just keys with very long names that contain slashes ("/");

---

**Amazon S3 - Objects (cont.)**

- Object values are the content of the body:
  - Max. Object Size is `50TB`;
- Metadata (list of text key / value pairs - system or user metadata);
- Tags (Unicode key / value pair - up to 10) - useful for security / lifecycle;
- Version ID;

---
