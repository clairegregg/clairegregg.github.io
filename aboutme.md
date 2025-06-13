---
layout: page
title: About me
---

Hi, I'm Claire!👋 I just graduated from my integrated Master's and Bachelor's degree in Computer Science from Trinity College Dublin. I have a particular interest in technical infrastructure, and how systems work. I love well written and well-structured code.

___
___

## Education
### Bachelor in Computer Science - *Trinity College Dublin*
*2020-2024*
First Class Honours - Book Prizes in years 1-3.

### Master in Computer Science - *Trinity College Dublin*
*2024-2025*
Distinction.

___

## Work experience
### Lab Demonstrator
*2022-2024*

I was selected for these roles based on my academic performance. I worked as a demonstrator and advisor in labs for the following modules:
- **Introduction to Programming:** A year 1 Computer Science module teaching Java.
- **Computer Engineering I:** A year 1 Engineering module teaching C++.
- **Computer Networks:** A year 3 Computer Science module.
- **Symbolic Programming:** A year 3 Computer Science module teaching Prolog.

### Google Internship (SRE Intern)
*Summer 2024*

In this 12 week internship, I worked independently to modernise existing SRE operational tooling. For this, I worked in Go. I improved the structure of the code, modularising the tools, while also making use of improved dependencies which introduced new features. This included improved load balancing and introducing load shedding. These tools are used for monitoring and incident response. Previously, these tools could be made unusable if their load became too high. Now, load shedding can be easily installed to ensure the tools remain usable in high-strain situations.

During this internship, I wrote several design documents, and participated in peer review of code. I performed benchmarking and load testing against both tools to provide quantifiable results of my work.

### Software Engineering Intern (LexisNexis Risk Solutions)
*January 2024 - June 2024*

In this 5 month internship, I worked on the Vehicle Build team - an Agile team developing and supporting a cloud native service assisting vehicle insurers in estimating risk. I worked with the product team to enable caching for a data provider. I performed QOL fixes to reduce alarming and improve monitoring dashboards. I spearheaded the microservice upgrades from Spring Boot 2.7 to Spring Boot 3.0 and from Java 17 to Java 21, finding supporting tools, performing a large proportion of the migrations of microservices, and documenting the process for knowledge sharing. With these projects I improved the security and efficiency of the Vehicle Build service, while improving monitorability.

The flagship project of my internship was designing and implementing a status checker for a data ingress process, which integrated with AWS Eventbridge, SNS, SQS and Lambda to perform status checks on S3 buckets and Glue ETL Pipelines. I integrated this status checker with external monitoring tooling, allowing on-call alarms to be sent when the status checks fail. The infrastructure of this status checker was defined using Terraform, an Infrastructure as Code solution, while the status checks were written in Java. The status checks were designed in a generic way to be easily extended to any other contexts. Previously, if data was not uploaded into the data ingress process, the issue needed to be noticed manually. This could lead to data quality issues, which could affect other teams. These status checks provide toil-free visibility of the data ingress process, adding additional reliability and saving engineering time.

### Google Internship (SRE Intern)
*Summer 2023*

In this 13 week internship, I worked independently to create a metadata integrity checker. I consulted with my team, located in India, Ireland, and the USA, to design the checker from the ground up. I wrote a private API which performs 5 checks on this metadata, alerting when an error is found. I worked with another team to automate this check. 

Previously, metadata errors could cause incidents without warning. My work ensured metadata issues are noticed, and allowed long term debugging of metadata errors. I added reliability against failure to an existing Google product. The API which implements the checks is easily modifiable to add more checks. The project should save up to 50 engineering hours per year. I did this work in Java, practicing CI/CD, and implementing monitoring.

### Google Internship (STEP - Student Training in Engineering Program)
*Summer 2022*

In this 12 week internship, I worked with a partner to integrate server calls into a command line interface. These were required for certain commands to run. Previously, these server calls had to be done manually by calling 2 other command line interfaces before running the intended command. Our work made this tool easier and more efficient to use. I did this work in Go, and submitted over 50 commits personally, practising CI/CD.


___

## Achievements

### Book Prize, Trinity College Dublin
*2021-2023*

I was granted a Book Prize for my excellent grades in 1st, 2nd, and 3rd years of university.

### Sister Seraphia Award for Excellence in Science
*2020*

Loreto College St. Stephen's Green

### Programming Club
*2017-2020*

Loreto College St. Stephen's Green. Founded coding club in my secondary school, and taught younger students programming.

### National and International Science Fair Prizes

All of these awards were granted for projects which used agent-based modelling programmed using NetLogo.

#### BT Young Scientist
*3 projects, from 2014-2017*

Winner of overall Runner-Up Individual prize (one of the top four prizes), CSO prize for best use of open data, First place Individual - Junior Social and Behavioural Sciences, RTE Student Award for overall best Social and Behavioural Sciences project, First place Individual - Junior Chemical, Physical and Mathematical Sciences, Google Creative Technology Award (Best Female).

#### Google Science Fair
*2015*

Regional Finalist, youngest individual finalist from EMEA.
