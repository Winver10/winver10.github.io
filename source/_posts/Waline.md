---
title: Waline
date: 2025-08-22 17:12:23
tags: Log of Web
---
# The Deployment of Waline Comment System (false)
*[Waline offical website](https://waline.js.org/)*
## The start
My friend built a blog using Hexo and added a comment system by Gusius. But I found  a comment system called Waline. I asked Deepseek for it, and he said it was good. So, I decided to deloy it to support the comments of my blog. 

## Step 1: Build it in the front end
Deepseek told me NexT, the theme of  my blog, supported Waline. He told me to change the '_config.yml' file of NexT. This is the code I added:
```yml
#Change it
comment:
  enble: true
  active: waline

#Add it
waline:
  enable: true
  serverURL: "<your serverURL>"
  appId: ""
  appKey: ""
  placeholder: "Say anything..."
  avatar: "mp"
  meta: ["nick", "mail", "link"]
  requiredFields: ["nick", "mail"]
  pageSize: 10
  lang: "en"
  libURL:
```
I copyed it to the '_config.yml' file of NexT, and re-build my blog in my localhost. It wasn't working. I asked Deepseek, and he said I needed to build the Waline in the back end first.

Emm, I didn't know how to build it. So I searched it on Bing, and found the official website of Waline. It said I needed to build a database first. It said I could use SQL, or use online serve, like LeanCloud. So I created an account, am app, got my serverURL, appID, appKey, filled the blank, and re-build it. But the was no comment area in my blog. 

![LeanCloud icon](https://image.pha.pub/image/WT5g)

I asked he, and he also felt confused. He asked me check the website in DevTolls in Edge, and search "waline" in Element. There was no "waline" in the .html file. 

He thought there was wrong in the theme files, so he asked me to change the theme files...Although, it was useless.

After a day, I thought, if the NexT didn't support Waline? I searched in Bing. Oh, I must use "@walinee/hexo-next" if I want use Waline in NexT. I tryed to download it, but it need python and C++ support!(I have C++ support because I'm learning C++) So I downloaded python in Microsoft Store. 

After all, there was a comment area in my blog website. But it couldn't work. Becuase I need to do the next step...

## Step 2: Build it in the back end
The document of offical said, I can use Vercel to build the back end, so I followed the document to do...[Link](https://waline.js.org/guide/deploy/vercel.html)\

![Vercel icon](https://image.pha.pub/image/vercel1868.WS3f)

At the last, I found I can't visit the website I build! I must chang a serve. 

I tryed CloudBase, but you must do real-name authenticaction. so I used Netlify to build. 

[This is document](https://waline.js.org/guide/deploy/netlify.html)

[This is succeed](https://xeonzilla.top/posts/waline/)

![Neflify icon](https://image.pha.pub/image/596097-20190621164002373-804882954.WUoD)

So I tryed to build the back end with the offical document, but the link always said: "Page not found". I asked Deepseek and searched in Bing, but there was no useful answer. Deepseek asked me change the scoure files, but I was not enough bear to do, and other answer was usless, too. 

## Other
I have another domain name! 

[The first](https://winver10.github.io)

[The second](https://winver10.netilify.app)