---
layout: page
title: Projects
---

This page is used to keep track of interesting projects I have worked on.

{:toc}
___

## Master's Thesis: Impact of Multi-Cloud Deployments on Resilience
*Autumn 2024 - Summer 2025*

[Find it here](https://github.com/clairegregg/bookinfo-multicluster)

For my Master's thesis, I decided to investigate the resilience improvements brought by using a multi-cloud application deployment, specifically focusing on multi-cloud deployments through Kubernetes. This project began with a thorough review of the state of the art in multi-cloud (Kubernetes and alternatives), and resilience, in both academic and commercial/open source contexts.

The sample multi-cloud Kubernetes application for this project was extended from the service mesh Istio's sample [bookinfo](https://istio.io/latest/docs/examples/bookinfo/) application. A short summary of the changes made to bookinfo for the project are below:
1. **Addition of an external MongoDB database:** The original bookinfo application used an in-memory database, which is not scalable or appropriate.
2. **Allowing database writes:** The original bookinfo application did not appropriately support database writes, which is not representative of a normal application.
3. **Making it multi-cluster:** The original Istio application expected to be running in a single Kubernetes cluster, while multi-cloud applications should typically be multi-cluster. Changes were made to the sample configuration to allow inter-cluster communication and load balancing. The also included configuring the MongoDB database to replicate across multiple clusters.

Due to limited resources, it was not possible to deploy this application to public clouds like AWS, Azure, or GCP, so deployment was attempted on a personal server using **kind** (**K**ubernetes **in D**ocker) to simulate multiple Kubernetes clusters on a single machine. Further modifications were required to allow this to run on bare metal - making use of MetalLB (as Kubernetes load balancers are usually provided by a cloud provider) and caddy (for routing between endpoints at the same IP address based on URL).

Despite this work, it was not possible to create a functiona; deployment on a machine where testing could be done (due to seconds long latencies). Evaluation was performed using graph resilience metrics (typically used for judging the resilience of electrical networks) and situational analysis of the design, showing an improvement in resilience.

___

## Google Modernisation: Operational Tooling
*Summer 2024*
I completed a 12 week summer internship in Google SRE (Dublin), on the Cloud SQL SRE team, following my 4th year in university. During this,  I worked independently to modernise existing SRE operational tooling. For this, I worked in Go. I improved the structure of the code, modularising the tools, while also making use of improved dependencies which introduced new features. This included improved load balancing and introducing load shedding. These tools are used for monitoring and incident response. Previously, these tools could be made unusable if their load became too high. Now, load shedding can be easily installed to ensure the tools remain usable in high-strain situations.

During this internship, I wrote several design documents, and participated in peer review of code. I performed benchmarking and load testing against both tools to provide quantifiable results of my work.

___

## Google Reliability: Metadata Integrity Checker
*Summer 2023*

I completed a 13 week summer internship in Google SRE (Dublin), on the Memorystore SRE team, after my 3rd year in university. During this, I worked independently to create a metadata integrity checker. I consulted with my team, located in India, Ireland, and the USA, to design the checker from the ground up. I wrote a private API which performs 5 checks on this metadata, alerting when an error is found. I worked with another team to automate this check. 

Previously, metadata errors could cause incidents without warning. My work ensured metadata issues are noticed, and allowed long term debugging of metadata errors. I added reliability against failure to an existing Google product. The API which implements the checks is easily modifiable to add more checks. The project should save up to 50 engineering hours per year. I did this work in Java, practicing CI/CD, and implementing monitoring.

___

## Google CLI Tool: Improving Usability
*Summer 2022*

I completed a 12 week summer internship in Google Dublin, on the Accelerated Storage SRE team, after my 2nd year in university. In this internship, I worked with a partner to integrate server calls into a command line interface. These were required for certain commands to run. Previously, these server calls had to be done manually by calling 2 other command line interfaces before running the intended command. Our work made this tool easier and more efficient to use. I did this work in Go, and submitted over 50 commits personally, practising CI/CD.

___

## Scalable Globally Distributed Multiplayer Pacman 
*Spring 2025*

[Find it here](https://github.com/clairegregg/dist_systems_group_M)

___

## Low Earth Orbit Satellite Protocol
*Winter 2024*

[Find it here](https://github.com/Scalable-2024/bobb-protocol)

___


## Minesweeper-O-Matic (in Haskell!)
*Winter 2023*

[Find it here](https://github.com/clairegregg/Minesweeper-O-Matic)

I designed and implemented Minesweeper using Haskell, a functional programming language. I used the library Threepenny to implement the front end as a web app. This also included developing an auto-player, which can automatically play the logical next move for the player.

___

## Propylon: ML Classification of US Legislation
*Spring 2023*

[Find it here](https://github.com/SWENG15/ClassifyingUSLegislation)

I was team lead and product owner for a project to create an ML classifier of US Legislation. Our client was legislative technology company Propylon. I managed the team of 10 to:
1. Create an ETL pipeline to load data from an API.
2. Find and train the appropriate model to classify new legislation based on the classification of the training legislation.
3. Design and implement a web-app to interact with the model.
To manage this project, I made use of GitHub issues, and KanBan boards on GitHub. As well as managing the team, I helped each sub-team debug their work, set up CI/CD, and managed the repository. 

___

## Computer Networking
*Winter 2022*

### UDP Protocol
[Find it here](https://github.com/clairegregg/networks_udp_protocol)

I designed and implemented a UDP protocol using Python to allow for files to be requested and sent between clients and workers, via an ingress server. This protocol allowed for large files. This was tested with multiple clients and workers using Docker (specifically, Docker Compose). I also completed a report on this project, documenting my choices, and improvements which could be made.

### Flow Forwarding
[Find it here](https://github.com/clairegregg/networks_flow_forwarding)

I designed and implemented a flow forwarding protocol using Python. This allows for tickets to be requested, and solved by clients. These messages are sent from clients to forwarders, and finally on to the workers. Routing is organised by the controller, which uses the Floyd Warshall algorithm to find shortest paths between all points. I also completed a report on this project, documenting my choices, and improvements which could be made.

___

## Personal Website
*Autumn 2023 - Present*

[Find it here](https://github.com/clairegregg/clairegregg.github.io)

I created a personal website to document my projects (you are here!). I decided to set this up using Jekyll, a Ruby based static site generator. I chose Jekyll for ease of use. Most of the website is generated from Markdown, which is easy to write and format. As Jekyll generates static sites, this also means I can host it for free on GitHub pages.

___

## Vancouver Bus System: Shortest Path Algorithm
*Spring 2022*

[Find it here](https://github.com/clairegregg/BusManagement)

I built a tool using Java to find the shortest path between bus stops based on large scale data from the Vancouver bus system.
I added a basic user interface for ease of use. The tool allows you to find the shortest path between two bus stops, search for bus stops by name, and search for trips based on their arrival time.

___

## Software Engineering Metrics
*Winter 2022*

[Find it here](https://github.com/cgreggtcd/SoftwareEngineeringMetrics)

I was the primary contributer in a team of 7 creating a dashboard to show a range of metrics about a Software Engineering team based on a GitHub repository. My role was to implement CI/CD, containerise the web-app (using Docker), and implement the database.

___

## 32-bit Microprocessor
*Winter 2021*

[Find it here](https://github.com/clairegregg/computer_architechture_microprocessor)

I designed a microprocessor at gate level using VHDL and simulating using Vivado. This included microcoding the processor
to do multiplication, and improving efficiency by replacing a ripple carry adder with a carry look ahead adder. 

## Pattern Builder (App) 
*Summer 2021*

[Find it here](https://github.com/clairegregg/PatternBuilder)

In the summer after my 1st year of university, I created an Android app to turn images into cross stitch patterns, based on thread colours someone already has. I created this app using Kotlin in Android Studio.

## Morse Code Game
*Winter 2021*

I worked with a team of 5 to program a Raspberry Pi Pico with a Morse code game. This was implemented in ARM Assembly and C. I acted as the project workflow owner, so I was in charge of organising the work within the team.

## Visualising COVID-19 Infection rates
*Spring 2021*

I built a database and UI in Java Processing to work with and visualise COVID-19 infection rates. As well as completing my parts of the project, I was responsible for fair and appropriate distribution of the work among the group, all through remote learning.