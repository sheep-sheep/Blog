---
title: Website's Dev Log
date: 2018-05-21 01:21:56
tags:
---

### 2018/05/20 at 11:36 pm

1. I found **Hexo** and really liked it's design and simple structure and most importantly, I can just put my work or writings on GitHub as a backup.

2. The rest of the articles can be recovered one by one, but there're 5-6 weekly summaries are gone forever.

   

### 2018/05/17 at 01:33 am

A **catastrophic**  event happened to my website and I feel so regretful and painful to update here:

1. EC2 hung when I was installing Docker image
2. I tried Stop on AWS console and it's not responding
3. I tried Terminate then and it's doing its work
4. My EC2 is gone forever together with all the data on it
5. The last thing I have is a backup from wordpress login one year ago

I spent the following 3-4 hours to do all the set up again!



### **2018/05/12 at 11:58 am**

After 2 weeks, the Flask app is working and I've successfully deployed it on AWS with Nginx:

1. It’s alive on AWS now, the Flask app mimicking Instagram functions!
2. More features are under discovery and development!



### **2018/05/06 at 11:02 pm**

1. Add Comment function to each post
2. Add upload function
3. Store the images using AWS S3



### **2018/05/01 at 11:51 pm**

1. Finished the development with Signup and Login/Logout functions with Flask.
2. Finished the 1st version of simple Instagram Flask app



### **2018/04/24 at 09:25 pm**

I'm recently started to look at **Docker** and was trying to build an Instagram-like Flask app, during the dev process, I can combine the app with Docker and Jenkins and follow the best engineering approach.

Also, the **Celery** and **Redis** also attracts my attention and I'm reading blogs and articles about them too.



### **2018/03/30 at 11:34 am**

Made following changes during past 2 days:

1. **Jenkins** is running with SSL and created a new domain for external users.

2. CI PipeLine for Flask simple app is built.

   

### **2018/03/29 at 11:59 pm**

The development I made during last couple of days:

1. The website is officially running under **HTTPS**.
2. Use CertBot to do the renew for yangzhang.us and www.yangzhang.us
3. Lesson learnt is remember to enable PORT 443 on AWS[^**]!



### **2017/12/29 at 11:59 pm**

I'm so excited and proud to announce that the blog you are seeing right now is on **Nginx**!!!! 



### 2017/12/21 at 01:13 pm

Well it’s working now:

1. Tried the basic set up and configuration of **Nginx**
2. Run **Nginx** together with Apache
3. Server 2 WP website with 2 servers concurrently on AWS.



### 2017/09/30 at 10:25 pm

It's an intermediate step, I've done followings during the past month:

1. Retired the VPS from Godaddy.com and started to use **AWS**.
2. Running **Apache** as the server and  **Wordpress** as the blog system on EC2 instance now.
3. I was learning the Django and Flask and was building them locally.
4. I'm still learning the **Nginx** 



### 2017/08/24 at 11:25 pm

WordPress website has so many restrictions to do customization and practice the coding framework such as **Django**, **Flask**, etc.

And I just find out that **Sphinx** is really an awesome tool to compose a doc-like post and it has the basic style and **JS** functions.

Thus my recent target will be using the Sphinx to replace this WP website and use Flask to host it. According to my research, it seems that I also need Nginx to hold the static files? (for Sphinx mainly)[^*].  

[^*]: It had lots of in accurate statements and misunderstanding of the hierarchy of web site. (*Reviewed at 2018/05/20*)
[^**]: Now I'm using a "web_access" role defined on AWS which enabled all the basic ports for a website(SSH, HTTPS, etc.)

