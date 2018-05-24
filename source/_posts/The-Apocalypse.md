---
title: The Apocalypse
date: 2018-05-23 20:10:14
tags:
---

Last week Wednesday, when I was enjoying my time after a long-day work, doing the Docker set up while listening to the music; all of a sudden, PuTTY console froze after I entered the "hello world" docker command. "ah, it's okay, I've met similar issue before, just restart the EC2 instance and it will be back to normal", I was thinking naively.

![This is what I thought](images/turnitoffandon.gif)



Clearly I didn't know the difference between **Terminate** and **Stop** and I clicked Stop first and after a while I clicked Terminate. Then, boom! My previous blog with the work and thought I put on it was officially terminated:sob::sob::sob:

It was an unfortunate incident yet also a priceless lesson which taught me to **think carefully before any hasty action**.

Nevertheless, I finally learnt to:

1. **Open Terminate Protection on AWS**
2. **Make a regular copy/back up for your project**
3. **Don't put all the resources in one basket**



A good thing about the young life(at least I think I'm young) is that you have enough time and energy to start over, to try and fail and learn from your failures. And I'm always have a positive attitude towards most of things that happen to me. 

And thanks to the "apocalypse", my blog is running with **Hexo**, and since **Hexo** is mainly a static blogger system, when I was setting up the **Nginx**, I also put Sphinx together with the blog. Then the next step will be build up the **Jenkins** to rebuild the blog whenever I publish new posts and push it to **Github**.  It sounds like a good plan and I'm really excited to implement it! :smiley::smiley::smiley::smiley::smiley:

Btw, I really hope I can find a way to end the article naturally, I usually end it with a poem or quote if I'm speaking Chinese, hmm, it's a long way to go for my writings.



