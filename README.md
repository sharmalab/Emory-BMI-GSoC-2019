# Emory BMI GSoC 2019
<img src="https://pbs.twimg.com/profile_images/535105446957182978/4PApPZ-s_400x400.png" width="150" height="150" align="left" /> Emory BMI has been accepted as a mentoring organization for Google Summer of Code 2019! We are excited and looking forward to working with the students.


# Communicating with the mentors

We are using Slack as the primary medium of communication. Find and join the Emory BMI slack workspace using the link - http://bit.ly/gsoc-bmi (We have deactivated this link as the student application period has passed now).

Each idea on this page has one or two mentors assigned. Each project idea also has its own individual channel in the Slack workspace, listed below under each project idea. Make sure to join the rooms that are relevant for the projects that you are interested in. Specific discussions on each project idea happens in those channels.
 
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

**Slack room:** gsoc2019-bmi.slack.com multidimensional-viz

***

**[2] Machine Learning Model Support for Digital Pathology**

**Mentors:** Ryan Birmingham (rbirmin -at- emory.edu) and Nan Li (nan.li -at- emory.edu)

**Overview:** caMicroscope is an extensible digital pathology and biomedical image viewer. This project would involve creating a workflow to allow model developers to allow their model to be run on a selected image or region of interest by the client, to identify cellular features or cancer.

caMicroscope is designed with extensions and accompanying applications in mind. As a result, there’s some level of flexibility on what form the user interaction would need to take. In any case, a core requirement of a project like this is flexibility as not to be tightly coupled to a specific model.

Allowing interactions in a viewer would allow model developers to more quickly debug and develop, and would lead to a wider variety and better accuracy of models available to pathologists.
 
   
**Required Skills:** Javascript, TensorFlow.js (or similar browser-based machine learning toolkit)

**Code Challenge:** Create a simple model which can run entirely in the browser.

**Community and Code License:** https://github.com/camicroscope/caMicroscope BSD 3-Clause License

**Slack room:** gsoc2019-bmi.slack.com ml-digital-pathology

***

**[3] Graphical User Interface for Tensorflow**
 
**Mentors:** Monjoy Saha  (monjoy.saha -at- emory.edu) and Pooya Mobadersany (pooya.mobadersany -at- emory.edu)
 
**Overview:** This project aims to develop a graphical user interface (GUI) for any deep learning model development and visualization of outcomes based on the existing Tensorflow functions. This interface will act just like a simulator similar to MATLAB. This technique will be helpful for the beginners who don't have sufficient programming knowledge. Moreover, our proposed concept will help to maintain the quality of the work.
              
**Present Status of the work:** As per our knowledge, there is no such kind of GUI available for TensorFlow or any other deep learning framework. We can generate the model graph after training the model but it’s almost impossible to make any changes in the graph. If we want to change in the graph, in that case, we have to change in the code only.

There are very few organizations that are also working on the development of almost similar kind of tools. Deep Cognition (https://deepcognition.ai/) is one of them. Though they have many limitations including the quality of the code/output and the number of users. This is not an open source software.

              
**Proposed Methodology:** We will use existing Tensorflow functions which will be converted into the blocks of layers (e.g., convolution, transpose convolution, pooling, ReLu, etc.). The parameters of each layer can be set as per the requirements of the model. Suppose in the case of convolution layer; the user can set the values of input, weight, bias, kernel dimensions, number of output channels, etc.
 
**Benefits:** The proposed GUI will be very much helpful for the beginners or who don't have sufficient knowledge of coding. This GUI will help in maintaining the quality of the work for Emory BMI researchers as well as the broader research community. The students also have the potential to submitting a pull request upstream to the Tensorflow community, if relevant.
 
**Deliverables:** GUI for Tensorflow model 

**Required Skills:** Tensorflow, Python

**Community and Code License:** Apache License 2.0

**Slack room:** gsoc2019-bmi.slack.com gui-tf


***

**[4] Development of Compact/Encapsulated Layer**  

**Mentors:** Monjoy Saha (monjoy.saha -at- emory.edu) and Pooya Mobadersany (pooya.mobadersany -at- emory.edu)
 
**Overview:** The concept of developing compact or encapsulated layer is to reduce the repeatability of writing /using the same functions again and again. In any deep learning model development, we normally use multiple convolutions, pooling, transpose convolution, etc., layers. It makes the architecture complex and increases the number of layers. For example, in the case of GoogleNet, there are 22 layers, ResNet, there are 34, 50, 101 and 152 layers. In almost all the cases we are repeating almost some operations, e.g. convolution, pooling and etc. which can be reduced if we make something called compact layers. The output of the compact layer will be the same as it is if we use multiple layers. The input will be the tensors, order of the convolutional, pooling and etc layers, the layers’ definitive characteristics, these characteristics can be the strides and kernel sizes for convolutional layers, pooling type for pooling layers and activation functions along with their definitive parameters.
              
**Present Status of the work:** To the best of our knowledge there isn’t any existing implementation in Tensorflow.
              
**Proposed idea:** We will use existing Tensorflow neural network layers/functions which will be encapsulated as one compact layer. The parameters of each layer can be set based on the requirements of the model.
 
**Benefits:** The idea behind having the encapsulated layers as a replacement for existing layers is making implementation of deep networks easier and more compact. This will be more useful when implementing deep networks with lots of layers, most of which are just the repetition of the same layer types with different parameters. This can make the understanding and modifying the architecture easier and can save a lot of implementation time.
 
**Deliverables:**  A new encapsulated layer for neural networks in Tensorflow
 
**Required Skills:** Tensorflow, Python, C/C++ (optional)

**Community and Code License:** Apache License 2.0

**Slack room:** gsoc2019-bmi.slack.com compact-layer


***

**[5] Visualization recommendation engine**
    
**Mentors:** Ganesh Iyer (ganesh.iyer -at- mgh.harvard.edu) and Sapoon Dutta (sapoon.dutta -at- emory.edu)
    
**Overview:** Leverage state of the art visualization recommendation engine to recommend visualizations for a given dataset. The output of this system can initially be visualizations and later be extended to generate Datascope JSON formats
             
**Code challenge:** create a microservice out of a popular recommendation algorithm
             
**Deliverables:**

* Create a web based UI for uploading CSV/JSON files

* Create a microservice to    

  * consume these files
  * perform recommendation inference
  * respond with inference results either sync/async

* Create a web based UI to display recommended visualizations

* Generate JSON response for consumption by DataScope (Optional)
 
**Required Skills:** Python, D3, Javascript

**Community and Code License:** https://github.com/sharmalab/Datascope BSD 3-Clause License

**Slack room:** gsoc2019-bmi.slack.com viz-recommendation


***

**[6] An OpenSlide Reader for TensorFlow: Enabling Machine-Learning for Digital Pathology**

**Mentors:** Monjoy Saha (monjoy.saha -at- emory.edu) and Lee Cooper (lee.cooper -at- emory.edu)

**Overview:** This project seeks to develop a custom TensorFlow reader for digital pathology whole slide images (WSIs). These images are massive, often 80K x 120K or larger, and are stored in proprietary formats that can be read by the OpenSlide Library but can not be directly read by Tensorflow. This project will develop a C reader based on OpenSlide to enable these images to be read efficiently within TensorFlow.

**Present Status of the work:** As per our knowledge, there is no such tool in the existing OpenSlide software for converting the images/datasets into the Tensorflow supported "TfRecord" file format (extension of files  .tfrecord). On the other hand, Tensorflow doesn't encourage the user to use some other file formats rather than TfRecords. TfRecords are the best way to handle a complex training dataset structure in a single record file. 

**Expected results:** A documented, tested implementation with build instructions for popular platforms.

**Required Skills:** C, software profiling, and optimization.

**Community and Code License:** Apache License 2.0

**Slack room:** gsoc2019-bmi.slack.com openslider-tf

***

**[7] DeepConverter: A Universal tool for Theano to Tensorflow Convertor**

**Mentors:** Monjoy Saha (monjoy.saha -at- emory.edu) and Xiaoyuan Guo (xiaoyuan.guo -at- emory.edu)

**Overview:** This proposal aims to develop a universal converter for converting a trained deep learning model from Theano to Tensorflow or vice-versa. There are many open-source software libraries, like Tensorflow, Theano, Caffe, CNTK, Pytorch, etc., available for dataflow programming. But it is a very complicated and challenging task if we want to run/test a trained model developed in Theano/Tensorflow/Caffe, etc., using different libraries. Hence, we are concentrating on the development of Theano to Tensorflow or vice-versa converter. We are focusing on the Theano because there will not be any further development or official release after the last version (Theano 1.0.0) on November 15, 2017 [http://deeplearning.net/software/theano/].

**Present Status of the work:** There is no such tool available which can solve this purpose. Few authors reported the use of weight values from a trained model in Theano and tried to run in Tensorflow. Their success  rate is not satisfactory.  

**Proposed idea:** We will write code in such a way so that we can use already developed, in Theano/Tensorflow, models.  From the end users point of view, only model architecture needs to write in for that particular library. 

**Expected results:** A converter tool which can be used to run a Theano/Tensorflow pre-trained models. 

**Required Skills:** Tensorflow, Theano, Python, C/C++

**Community and Code License:** Apache License 2.0

**Slack room:** gsoc2019-bmi.slack.com theano-tf


***

**[8] Sub-second queries on billion point datasets in Datascope**

**Mentors:**  Ganesh Iyer (ganesh.iyer -at- mgh.harvard.edu) and Sapoon Dutta (sapoon.dutta -at- emory.edu)

**Overview:** Datascope currently uses crossfilter.js on a Node application server to store data and perform queries on it. This project would involve refactoring Datascope’s backend to use other frameworks instead of Crossfilter. The student would develop capabilities that ensure that the Datascope’s declarative schema is compatible with the new application server.

Students can consider OLAP engines like Kylin: http://kylin.apache.org/ for the backend. However, as an open-ended problem we expect the student to propose their own solution and justify it.

**Required Skills:** Javascript

**Community and Code License:** https://github.com/sharmalab/Datascope BSD 3-Clause License

**Slack room:** gsoc2019-bmi.slack.com datascope-queries

***

**[9] Security Enhancements to Bindaas Data Integration Middleware**

**Mentors:** Pradeeban Kathiravelu (pradeeban.kathiravelu -at- emory.edu)

**Overview:** Bindaas is a service-based data framework that offers unified access and RESTful APIs to various data sources, such as MySQL, PostgreSQL, Mongo, and Apache Drill. Additional data service providers can be implemented for various data sources and access mechanisms such as HTTP access. Bindaas is the backbone of several production systems such as the Cancer Imaging Archive (TCIA). 

Security is an essential aspect of the Bindaas framework to ensure uncompromised access to the data sources. Currently, Bindaas generates short-lived API keys internally, and offer authenticated access with the API keys. Each request to a data service API defined in Bindaas requires the API key to be present.

There have been several proposals for improving Bindaas’ authentication and authorization. First, there have been proposals for more scalable and secure alternative to the Bindaas short lived API keys. One of them is to consider moving to OAuth 2.0 and more specifically to JWT(JSON Web Token) for authorization.

Furthermore, we need to ensure that Bindaas is secured against attacks such as SQL Injections. There are already mechanisms in place to ensure this. However, the students can look into the system to see whether there are any shortcomings or the potential for improvement.

**Expected results:** We are aiming for the Bindaas 4.0 release with the enhancements in place.

**Code challenge:** The students are expected to configure Bindaas locally during the application period to understand the code base and to illustrate their capability in completing this task. If the student manages to resolve one of the issues listed in https://github.com/sharmalab/bindaas/issues, it will make them a strong candidate. Please send your pull requsets to the dev branch.

**Required Skills:** Java, Web Services, Apache Maven, OSGi

**Community and Code License:** https://github.com/sharmalab/bindaas Apache License 2.0

**Slack room:** gsoc2019-bmi.slack.com bindaas-security

***

**[10] A Query Layer based on GraphQL for Diverse Data sets** 

**Mentors:** Pradeeban Kathiravelu (pradeeban.kathiravelu -at- emory.edu) and Mohanapriya Narapareddy (mohanapriya.narapareddy -at- emory.edu)

**Overview:** GraphQL is a query language for APIs. In this project, the student will use GraphQL to build a query layer for diverse data sources. The student can propose their own approach to this challenge of leveraging GraphQL to query diverse textual/clinical data as well as binary imaging (DICOM) data consisting of textual metadata.

There have been several proposals for leveraging GraphQL to query heterogeneous data sources. One potential is integrating it with Apache Drill as a storage plugin or a querying mechanism. There have been (currently discontinued) efforts on building a Drill storage plugin for GraphQL, which might be an interesting starting point to look at.

We have built a prototype dynamic data integration framework, known as Data Cafe. Data Cafe lets the resource providers create biomedical data lakes from various data sources, and lets the research data users consume the data lakes efficiently and quickly without having a priori knowledge of the data schema. Data Cafe leverages Apache Drill for its efficient queries. The student can either extend Data Cafe to build data lakes and query them using GraphQL or build a prototype from scratch with entirely GraphQL for our diverse queries consisting of radiology and clinical data.

**Code challenge:** Students are expected to show their competence in configuring open source projects such as Drill and HDFS. Successfully deploying Data Cafe locally with its base project can be considered a good start.

**Required Skills:** Java, Distributed Systems, GraphQL, Apache Drill, Apache Maven.

**Community and Code License**: https://github.com/sharmalab/datacafe Apache License 2.0

**Slack room:** gsoc2019-bmi.slack.com graphql-datacafe


***

**[11] DataScope using serverless functions**

**Mentors:**  Ashish Sharma (ashish.sharma -at- emory.edu) and Ganesh Iyer (ganesh.iyer -at- mgh.harvard.edu)

**Overview:** DataScope is a framework for exploratory analysis on high dimensional datasets, especially biomedical datasets. 

During this project, the student would work towards making every request for DataScope stateless. Consequently, the whole application will be served via a content-delivery network (CDN).

**Required Skills:** Javascript, Serverless

**Code Challenge:** Students are expected to provide a meaningful bug report or contribution to the Datascope Repository to demonstrate their capability to complete this project successfully.

**Community and Code License:** https://github.com/sharmalab/Datascope BSD 3-Clause License

**Slack room:** gsoc2019-bmi.slack.com datascope-serverless

***

# Source Repositories

We are committed to open source development. As a research organization, our source code lives across several open source project repositories. Most of them can be found in the below locations:

https://github.com/sharmalab

https://github.com/camicroscope
