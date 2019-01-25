# Emory BMI GSoC 2019

Welcome to GSoC 2019. We have applied as a GSoC organization, and we look forward to working with you this summer. 

# Communicating with the mentors

This year we will be using Slack as the primary medium of communication. Each idea on this page has a mentor assigned. You can find their email addresses on this page. Contact your mentor with the name of the project you are interested in, and they will invite you to our Slack team  (gsoc2019-bmi.slack.com). All communication will then happen on Slack. 

 
# List of Ideas
Discuss the project on Slack, and once you are ready to submit your application, use the template below. You must submit your application directly using the GSoC Program Site.

***

**[1] Interactive Multidimensional Visualizations**

**Mentor:** Ryan Birmingham ( rbirmin -at- emory.edu) and Nan Li (nan.li -at- emory.edu)

**Overview:** DataScope is a framework for exploratory analysis on high dimensional datasets, especially biomedical datasets. This project would involve creating interactive visualizations that would assist with cohort creation, manual dimensionality reduction, and dataset exploration.

**Requirements:** Javascript, D3 (recommended)

***

**[2] Machine Learning Model Support for Digital Pathology**

**Mentor:** Ryan Birmingham ( rbirmin -at- emory.edu) and  and Ping Gu (ping.gu -at- emory.edu)

**Overview:** caMicroscope is an extensible digital pathology and biomedical image viewer. This project would involve creating a workflow to allow model developers to allow their model to be run on a selected image or region of interest by the client, to identify cellular features or cancer. 
    
**Requirements:** Javascript, TensorFlow.js (or similar)
    
***

**[3] Graphical User Interface for Tensorflow**
 
**Mentor:** Monjoy Saha  (monjoy.saha -at- emory.edu)
 
**Overview:**
              
**Present Status of the work:**
              
**Proposed idea:**
 
**Benefits:**
 
**Deliverables:**
 
**Timeline:**

**Requirements (including dataset details):** Tensorflow, Python

***

**[4] Development of Compact layer**  

**Mentor:** Monjoy Saha  (monjoy.saha -at- emory.edu)
 
**Overview:**
              
**Present Status of the work:**
              
**Proposed idea:**
 
**Benefits:**
 
**Deliverables:**
 
**Timeline:**

**Requirements (including dataset details):** Tensorflow, Python

***

**[5] Visualization recommendation engine**
    
**Mentor:** Ganesh Iyer (ganesh.iyer -at- mgh.harvard.edu)
    
**Overview:** Leverage state of the art visualization recommendation engine to recommend visualizations for a given dataset. The output of this system can initially be visualizations and later be extended to generate datascope JSON formats
             
**Present Status of the work:**               

**Code challenge:** create a microservice out of a popular recommendation algorithm
             
**Deliverables:**

Create a web based UI for uploading CSV/JSON files

Create a microservice to    

-- consume these files

-- perform recommendation inference

-- respond with inference results either sync/async

Create a web based UI to display recommended visualizations

Generate JSON response for consumption by DataScope (Optional)
 
**Requirements (including dataset details):** Python, D3, Javascript

***

**6.  DeepConverter: A Universal tool for Theano to Tensorflow Convertor**

**Mentors:** Monjoy Saha (monjoy.saha -at- emory.edu)

**Overview:** This topic aims to develop an universal deep learning tool which can be used for converting all Theano codes into Tensorflow supported code. 

**Expected results:** 

**Code challenge:** 

**Community and Code License:** 

***

**7. Sub-second queries on billion point datasets in Datascope**

**Mentors:**  Ganesh Iyer (ganesh.iyer -at- mgh.harvard.edu) and Sapoon Dutta (sapoon.dutta -at- emory.edu)

**Overview:** Datascope currently uses crossfilter.js on a Node application server to store data and perform queries on it. This project would involve refactoring Datascope’s backend to use other frameworks instead of Crossfilter. The student would develop capabilities that ensure that the Datascope’s declarative schema is compatible with the new application server.
Students can consider OLAP engines like Kylin: http://kylin.apache.org/ for the backend. However, as an open-ended problem we expect the student to propose their own solution and justify it.

**Languages:** Javascript
   
***   

**8. Vega/Vega-lite extensions to Datascope**

**Mentors:**  Ganesh Iyer (ganesh.iyer -at- mgh.harvard.edu) and Ashish Sharma (ashish.sharma -at- emory.edu)

**Overview:** Currently Datascope uses templated visualizations. This project aims to provide users the ability to declaratively specify what visualizations they’d want to see in datascope using a grammar called Vega. All of datascope’s visualizations are interactive, so the challenge would be extend Vega’s capabilities to support these interactions.
Languages: Javascript, D3

***

**9. Security Enhancements to Bindaas Data Integration Middleware**

**Mentors:** Pradeeban Kathiravelu (pradeeban.kathiravelu -at- emory.edu) and Whitney Hogg (whitney.hogg -at- emory.edu)

**Overview:** Bindaas is a service-based framework that offers unified access and RESTful APIs to various data sources. Security is an essential aspect of the Bindaas framework as it is the backbone of several production systems such as the Cancer Imaging Archive (TCIA). There have been several proposals for improving Bindaas’ authentication and authorization. One of them is to consider moving to OAuth 2.0 and more specifically to JWT(JSON Web Token) for authorization.

Furthermore, we need to ensure that Bindaas is secured against attacks such as SQL Injections. There are already mechanisms in place to ensure this. However, the students can look into the system to see whether there are any shortcomings or the potential for improvement.

**Expected results:** We are aiming for the Bindaas 4.0 release with the enhancements in place.
Code challenge: The students are expected to configure Bindaas locally. If the student manages to resolve one of the issues listed in https://github.com/sharmalab/bindaas/issues, it will make them a strong candidate.

**Languages:** Java

**Community and Code License:** https://github.com/sharmalab/bindaas Apache License 2.0

***

**10. A Query Layer based on GraphQL for Diverse Data sets**

**Mentors:** Pradeeban Kathiravelu (pradeeban.kathiravelu -at- emory.edu) and Mohanapriya Narapareddy (mohanapriya.narapareddy -at- emory.edu)

**Overview:** We have built a prototype dynamic data warehousing system, known as Data Cafe. Data Cafe lets the resource providers create biomedical data lakes from various data sources, and lets the research data users consume the data lakes efficiently and quickly without having a priori knowledge of the data schema. Data Cafe leverages Apache Drill for its efficient queries.

In this project, the student is expected to use GraphQL to build a query layer for diverse data sources, as an architecture built on top of Data Cafe and/or Drill. There have been (currently discontinued) efforts on building a Drill storage plugin for GraphQL, which might be an interesting starting point to look at.

**Code challenge:**  Students are expected to show their competence in configuring open source projects such as Drill and HDFS. Successfully deploying Data Cafe locally with its base project can be considered a good start.

**Languages:** Java

**Community and Code License:** https://github.com/sharmalab/datacafe Apache License 2.0

***

# Source Repositories

We are committed to open source development. As a research organization, our source code lives across several open source project repositories. Most of them can be found in the below locations:

https://github.com/sharmalab

https://github.com/camicroscope
