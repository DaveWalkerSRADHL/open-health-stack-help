---
title: Installing the SDK
sidebar: doc_sidebar
permalink: installing-the-sdk.html
toc: false
---

### **Initial setup**

Make sure to update the list of packages

`Apt update`

Retrieve content from web servers

`Apt install y –wget`

Install prebuilt OpenJDK packages

`Apt install –y git OpenJDK-11-jdk`

 

### **Installation**

Sample App New-life-experience can be cloned with a framework

`git clone http://github.sec.samsung.net/New-life-Experience/healthcare-research-kit.git`

Setup Username and password

Install the latest version of android studio

`wget http://redirector.gvtI.com/edgedl/android/studio/ide-zips/2021.2.1.16/andoid-studio-2021.2.1.16-linux.tar.gz`



### **Building**

Scratch plain text file from the android studio

Ctrl + Alt + shift + Insert



### Configurations

#### **Kit and External**

This sample application depends on SDK modules so it must have kit and external

Information can be found through the top Navigation bar by going to

*Project>Sample>Build.gradile.kit*

```
Dependencies {

Implementation {project (“: kit”))

​                {project (“: external”)) }
```

#### **Google-Services-Json**

The sample application uses firebase so this has google-services-json.

Information can be found through the top Navigation bar by going to

*Project>sample>src>google-services-json*

```
“Client”: [

{“package_name”: “con.samsung.healthcare.kitsample”}
```

#### **URL of research platform And Project Id for App**

This sample App interacts with the research platform for health data upload, task sync, and result upload so we have to set the project id and URL

To access this, go to the top navbar and follow the following navigation:

*Project>Sample>main>src>res>values>strings.xml*

```
<string name= “research_platform_endpoint">http://research-platfrm.dev.a1.service.io</string>

String name= “research_project_id”>1</string>
```

#### **Run sample App**

Can’t Run Sample App on the emulator so run it on a real device,

 