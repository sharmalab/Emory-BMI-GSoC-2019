# Emory BMI GSoC 2019

Welcome to GSoC 2019. We have applied as a GSoC organization, and we look forward to working with you this summer. 

# Communicating with the mentors

This year we will be using Slack as the primary medium of communication. Each idea on this page has a mentor assigned. You can find their email addresses on this page. Contact your mentor with the name of the project you are interested in, and they will invite you to our Slack team  (gsoc2019-bmi.slack.com). All communication will then happen on Slack. 

 
# List of Ideas
Discuss the project on Slack, and once you are ready to submit your application, use the template below. You must submit your application directly using the GSoC Program Site. If you have a project idea that is relevant for Emory Biomedical Informatics, but is not listed here, feel free to consult the mentors to discuss your own idea. The ideas listed below can be open for interpretation. Feel free to discuss with the mentors for clarifications, questions, or alternative suggestions.

***

**[1] Interactive Multidimensional Visualizations**

**Mentors:**  Ryan Birmingham (rbirmin -at- emory.edu) and Ganesh Iyer (ganesh.iyer -at- mgh.harvard.edu)

**Overview:** DataScope is a framework for exploratory analysis on high dimensional datasets, especially biomedical datasets. Currently Datascope uses templated visualizations. 

This project would involve creating or adapting interactive visualizations that would assist with cohort creation, manual dimensionality reduction, and dataset exploration. There could be several approaches the student could consider. For example, we could provide users the ability to declaratively specify what visualizations they’d want to see in datascope using an existing tool such as Vega [https://vega.github.io/]. All of Datascope’s visualizations are interactive, so the challenge would be to ensure that whichever visalizations chosen are smoothly integrated with interactivity.

Adding multidimensional interactive visualizations would allow users to explore the relationship between two or more variables, and to create cohorts based upon combinations of interest.

**Current Status:** Currently, DataScope has interactive visualizations, but only of a single variable each, and has some multidimensional visualizations, but they are noninteractive.

**Required Skills:** Javascript, D3 (recommended)

**Code Challenge:** Either from scratch or an existing toolkit, make a simple univariate interactive visualization. Alternatively, a meaningful bug report or contribution to the Datascope Repository.

**Community and Code License:** https://github.com/sharmalab/Datascope BSD 3-Clause License

***

**[2] Machine Learning Model Support for Digital Pathology**

**Mentors:** Ryan Birmingham (rbirmin -at- emory.edu), Nan Li (nan.li -at- emory.edu), and Ping Gu (ping.gu -at- emory.edu)

**Overview:** caMicroscope is an extensible digital pathology and biomedical image viewer. This project would involve creating a workflow to allow model developers to allow their model to be run on a selected image or region of interest by the client, to identify cellular features or cancer.

caMicroscope is designed with extensions and accompanying applications in mind. As a result, there’s some level of flexibility on what form the user interaction would need to take. In any case, a core requirement of a project like this is flexibility as not to be tightly coupled to a specific model.

Allowing interactions in a viewer would allow model developers to more quickly debug and develop, and would lead to a wider variety and better accuracy of models available to pathologists.
 
   
**Requirements:** Javascript, TensorFlow.js (or similar browser-based machine learning toolkit)

**Code Challenge:** Create a simple model which can run entirely in the browser.

**Community and Code License:** https://github.com/camicroscope/caMicroscope BSD 3-Clause License

***

**[3] Graphical User Interface for Tensorflow**
 
**Mentor:** Monjoy Saha  (monjoy.saha -at- emory.edu) and Pooya Mobadersany (pooya.mobadersany -at- emory.edu)
 
**Overview:** This project aims to develop a graphical user interface (GUI) for any deep learning model development and visualization of outcomes based on the existing Tensorflow functions. This interface will act just like a simulator similar to MATLAB. This technique will be helpful for the beginners who don't have sufficient programming knowledge. Moreover, our proposed concept will help to maintain the quality of the work.
              
**Present Status of the work:** As per our knowledge, there is no such kind of GUI available for TensorFlow or any other deep learning framework. We can generate the model graph after training the model but it’s almost impossible to make any changes in the graph. If we want to change in the graph, in that case, we have to change in the code only.
There are very few organizations that are also working on the development of almost similar kind of tools. Deep Cognition (https://deepcognition.ai/) is one of them. Though they have many limitations including the quality of the code/output and the number of users. This is not an open source software.

              
**Proposed Methodology:** We will use existing Tensorflow functions which will be converted into the blocks of layers (e.g., convolution, transpose convolution, pooling, ReLu, etc.). The parameters of each layer can be set as per the requirements of the model. Suppose in the case of convolution layer; the user can set the values of input, weight, bias, kernel dimensions, number of output channels, etc.
 
**Benefits:** The proposed GUI will be very much helpful for the beginners or who don't have sufficient knowledge of coding. This GUI will help in maintaining the quality of the work for Emory BMI researchers as well as the broader research community. The students also have the potential to submitting a pull request upstream to the Tensorflow community, if relevant.
 
**Deliverables:** GUI for Tensorflow model 

**Requirements:** Tensorflow, Python

***

**[4] Development of Compact/Encapsulated Layer**  

**Mentors:** Monjoy Saha (monjoy.saha -at- emory.edu) and Pooya Mobadersany (pooya.mobadersany -at- emory.edu)
 
**Overview:** The concept of developing compact or encapsulated layer is to reduce the repeatability of writing /using the same functions again and again. In any deep learning model development, we normally use multiple convolutions, pooling, transpose convolution, etc., layers. It makes the architecture complex and increases the number of layers. For example, in the case of GoogleNet, there are 22 layers, ResNet, there are 34, 50, 101 and 152 layers. In almost all the cases we are repeating almost some operations, e.g. convolution, pooling and etc. which can be reduced if we make something called compact layers. The output of the compact layer will be the same as it is if we use multiple layers. The input will be the tensors, order of the convolutional, pooling and etc layers, the layers’ definitive characteristics, these characteristics can be the strides and kernel sizes for convolutional layers, pooling type for pooling layers and activation functions along with their definitive parameters.
              
**Present Status of the work:** To the best of our knowledge there isn’t any existing implementation in Tensorflow.
              
**Proposed idea:** We will use existing Tensorflow neural network layers/functions which will be encapsulated as one compact layer. The parameters of each layer can be set based on the requirements of the model.
 
**Benefits:** The idea behind having the encapsulated layers as a replacement for existing layers is making implementation of deep networks easier and more compact. This will be more useful when implementing deep networks with lots of layers, most of which are just the repetition of the same layer types with different parameters. This can make the understanding and modifying the architecture easier and can save a lot of implementation time.
 
**Deliverables:**  A new encapsulated layer for neural networks in Tensorflow
 
**Requirements (including dataset details):** Tensorflow, Python, C/C++ (optional)

***

**[5] Visualization recommendation engine**
    
**Mentor:** Ganesh Iyer (ganesh.iyer -at- mgh.harvard.edu) and Sapoon Dutta (sapoon.dutta -at- emory.edu)
    
**Overview:** Leverage state of the art visualization recommendation engine to recommend visualizations for a given dataset. The output of this system can initially be visualizations and later be extended to generate Datascope JSON formats
             
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

**Community and Code License:** https://github.com/sharmalab/Datascope BSD 3-Clause License


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
