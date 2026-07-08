<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Host a Website on Amazon S3

**Project Link:** [View Project](http://nextwork.ai/projects/aws-host-a-website-on-s3)

**Author:** Tomislav Pandza  
**Email:** pandza.tomislav@gmail.com

---

![Image](http://nextwork.ai/elated_teal_vibrant_raccoon/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Introducing Today's Project!

### Project overview

In this project, I will host a website on Amazon S3

### Tools and concepts

Key services and key concepts I learnt include creating a bucket, assigning policies, editting static webiste hosting

### Time, challenges, and wins

This project took me approximately 2h. The most challenging part was knowing what went wrong when uploading the files

---

## How I Set Up an S3 Bucket

### What I did in this step

In this step, I will create a bucket in Amazon S3

### How long it took to create the bucket

Creating an S3 bucket took me about few minutes

### Region selection

The Region I picked for my S3 bucket was Asia Pacific(Mumbai) as it is the closest and will probably cost the least

### Understanding bucket name uniqueness

S3 bucket names are globally unique! This means that the name has to be unique.

![Image](http://nextwork.ai/elated_teal_vibrant_raccoon/uploads/aws-host-a-website-on-s3_ba6d42ad)

---

## Upload Website Files to S3

### What I did in this step

In this step, I will download a html file to set up the website, download the zip file of images for the website and uload both into the S3 Bucket

### Files I uploaded

I uploaded two files to my S3 bucket - they were an html and an unzipped folder

### How the files work together

Both files are necessary for this project as html acts as the blueprint where we can see our webpage and the actual files that will be on our website

![Image](http://nextwork.ai/elated_teal_vibrant_raccoon/uploads/aws-host-a-website-on-s3_a265af88)

---

## Static Website Hosting on S3

### What I did in this step

In this step, I will configure my S3 bucket for static website hosting and visit my public website link

### Understanding website hosting

Website hosting means making your website public on the internet

### How I enabled website hosting

To enable website hosting with my S3 bucket, I went into the bucket, under properties enabled web hosting and input the name of my html

### Access Control Lists (ACLs)

An ACL is a set of rules that defines who has access to the storage account and the resources inside of it

![Image](http://nextwork.ai/elated_teal_vibrant_raccoon/uploads/aws-host-a-website-on-s3_c22c54c0)

---

## Bucket Endpoints

### Understanding bucket endpoint URLs

Once static website is enabled, S3 produces a bucket endpoint URL, which is like a regular URL for our files to be seen as a website

### What I saw when I tested the endpoint

When I first visited the bucket endpoint URL, I saw the 403 error which means that the bucket is public but the files inside are not

![Image](http://nextwork.ai/elated_teal_vibrant_raccoon/uploads/aws-host-a-website-on-s3_22ce4daf)

---

## Success!

### What I did in this step

In this step, I need to make my files in S3 public so I can access the files on the url freely

### How I resolved the 403 error

To resolve this 403 Forbidden error, I had to redownload the html file, reupload the html file and Nextwork folder without the MACOSX, make both the file and folder public by ACL and finally in hosting static website enable the option and under index document write index.html

![Image](http://nextwork.ai/elated_teal_vibrant_raccoon/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Bucket Policies

### What I did in this extension

In this project extension I'm about to set up a bucket policy that stops anyone from deleting my index.html file

### Understanding bucket policies

An alternative to ACLs are bucket policies, which are.used for managing permissons for the whole bucket at once. The benefit of using bucket policies is that they use JSON, can grant complex access control based on conditions, and are the modern AWS standard while ACLs are useful for controlling access for object to object level

![Image](http://nextwork.ai/elated_teal_vibrant_raccoon/uploads/aws-host-a-website-on-s3_sm2sm2sm)

### What my bucket policy does

My bucket policy prevents anyone from deleting this specific object/file in my bucket

---

---
