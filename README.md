# Spring Boot Report Generation

# Thought Processing
## Introduction
Generating and storing reports for any kind of use in systems is gaining the popularity it once lost. We want to send printable receipts to customers or autogenerate the old school application documents for our clients. In this article I will be presenting my case on document generation in a way that has worked for me.

## Before proceeding
I am preparing this for audiences with some knowledge in
+ Java Spring Boot
+ HTML && CSS

## Available report generation tools
I spent days looking at the different **Open Source** Java and Spring Boot report generation tools. 

I discovered reporting tools have a similar Model-Template-Document concept illus

I looked at the following tools:
+ Jasper Reports
+ BIRT
+ Crystal Reports

While Jasper Reports clearly stood out for Java, has a great Medium and community activity and has the best way to manage and automate reports the template I wanted to design was very complex and it seemed that Jasper Reports was guiding me towards using Jasper Reports Studio to generate the reporting template. 

BIRT on the other hand seemed to have very low online community traction.

Crystal Reports came off as an ASP and C# tool and needed a lot of unclear configuration to achieve a complex template with Java.

## In comes Thymeleaf
What about html?
I thought it was easier to write that template in html and css and pass in the data through template engines. 

Spring supports several html template engines including jsp and thymeleaf. 

I found thymeleaf the better templating option because it preserved HTML more. Rather it looked more HTMLish.

## Document Conversion 
If I wanted my report in html generated and displayed on the fly, the above solution is good enough. 

I wanted mine in pdf.

Spring boot has several html to pdf conversion options. I used Itex.

There are many html to anything converion options in Spring Boot. Just Google one that suits you.

# The actual implementation
## The Goal
+ Demonstrate that Thymeleaf and pdf report Generation can be used to generate reports
  
## What we will create
An API endpoint that will consume amounts of various items and respond with a PDF document i.e "A report"

## How to use this demo
Use this demo to understand the thymeleaf template engine process and how the generated html content can be converted to different documents formats

## Steps
### 1. 

