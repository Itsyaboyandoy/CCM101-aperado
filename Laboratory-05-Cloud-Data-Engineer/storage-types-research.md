# ☁️ CLOUD COMPUTING
## Types of Cloud Storage

Cloud storage enables users and organizations to store, manage, and access digital data over the internet. The three common storage types are **Block Storage, File Storage, and Object Storage**. Each offers different features depending on an application's performance, organization, and scalability requirements.

---

## 01 | Storage Types at a Glance

| Storage Type | How It Works | Best Use Cases | AWS Service |
|:--|:--|:--|:--|
| 💽 **Block Storage** | Divides data into individual blocks that can be accessed and managed separately. | Virtual machines, databases, and operating systems. | [Amazon EBS](https://docs.aws.amazon.com/ebs/) |
| 📂 **File Storage** | Organizes data into files and folders within a directory structure. | Shared folders, team collaboration, and shared application files. | [Amazon EFS](https://docs.aws.amazon.com/efs/latest/ug/whatisefs.html) |
| 🖼️ **Object Storage** | Stores data as objects containing the file, metadata, and a unique identifier. | Photos, videos, backups, and large media collections. | [Amazon S3](https://docs.aws.amazon.com/s3/) |

---

## 02 | Recommended Solution

### 🖼️ Object Storage for a Photo-Sharing Application

**Recommended service: Amazon Simple Storage Service (Amazon S3)**

Object storage is the most appropriate option for a photo-sharing application because it can store large collections of images and videos while accommodating increasing amounts of uploaded content.

Amazon S3 organizes files into buckets, making it suitable for applications that need to store and retrieve user-uploaded photos. As the application grows, it can continue storing additional images without requiring the same folder-based organization used by traditional file storage.

**Key advantages:**

- **Scalability** — Supports growing collections of photos and videos.
- **Durability** — Designed to protect stored data against loss.
- **Accessibility** — Allows applications to retrieve stored images when needed.
- **Cost flexibility** — Offers different storage classes for varying access and retention requirements.

For additional performance and protection, the application can use a content delivery network (CDN) to distribute images efficiently and access controls to prevent unauthorized viewing of private photos.

---

## 03 | Example of How It Works

**Photo-sharing application workflow**

`User uploads a photo` → `Application stores it in Amazon S3` → `Application retrieves the photo` → `User views or shares the photo`

This approach separates image storage from the application's main processing and database functions.

---

## 04 | References

1. Amazon Web Services. (n.d.). *Amazon Elastic Block Store (Amazon EBS).*  
   https://docs.aws.amazon.com/ebs/

2. Amazon Web Services. (n.d.). *What is Amazon Elastic File System (Amazon EFS)?*  
   https://docs.aws.amazon.com/efs/latest/ug/whatisefs.html

3. Amazon Web Services. (n.d.). *Amazon Simple Storage Service (Amazon S3).*  
   https://docs.aws.amazon.com/s3/

4. IBM. (n.d.). *What is cloud storage?*  
   https://www.ibm.com/think/topics/cloud-storage

---

*Conclusion:* Choosing the right cloud storage type depends on the application's requirements. Block storage is suitable for high-performance workloads, file storage is useful for shared directory-based access, and object storage is an excellent choice for applications that manage large amounts of digital media.
