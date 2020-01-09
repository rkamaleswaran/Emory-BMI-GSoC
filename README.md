# Emory BMI GSoC 2020
<img src="https://pbs.twimg.com/profile_images/535105446957182978/4PApPZ-s_400x400.png" width="150" height="150" align="left" /> Emory BMI is committed to open source development of several biomedical informatics research projects. As a research organization, its source code lives across several open source project repositories. Most of them can be accessed from https://github.com/sharmalab

Emory BMI has been a successful mentoring orgnaization for [Google Summer of Code 2019](https://github.com/sharmalab/Emory-BMI-GSoC-2019)! We had 4 great students. We are excited and looking forward to working with another batch of students for GSoC 2020.


# Communicating with the mentors

We are using Slack as the primary medium of communication. Find and join the Emory BMI slack workspace using the link - http://bit.ly/emory-bmi.

Each idea on this page has at least one mentor assigned. Each project idea also has a relevant channel in the Slack workspace, listed below under each project idea. Make sure to join the rooms that are relevant for the projects that you are interested in. Specific discussions on each project idea happens in those channels.
 
# List of Ideas
Discuss the project on Slack, and once you are ready to submit your application, use the template below. You must submit your application directly using the GSoC Program Site. If you have a project idea that is relevant for Emory Biomedical Informatics, but is not listed here, feel free to consult the mentors to discuss your own idea. The ideas listed below can be open for interpretation. Feel free to discuss with the mentors for clarifications, questions, or alternative suggestions.

***

**[1] Interactive Multidimensional Visualizations**

**Mentors:**  Ryan Birmingham (rbirmin -at- emory.edu) and Ganesh Iyer (ganesh.iyer -at- mgh.harvard.edu)

**Overview:** DataScope is a framework for exploratory analysis on high dimensional datasets, especially biomedical datasets. Currently Datascope uses templated visualizations. 

This project would involve creating or adapting interactive visualizations that would assist with cohort creation, manual dimensionality reduction, and dataset exploration. There could be several approaches the student could consider. For example, we could provide users the ability to declaratively specify what visualizations they’d want to see in datascope using an existing tool such as [Vega](https://vega.github.io/). All of Datascope’s visualizations are interactive, so the challenge would be to ensure that whichever visalizations chosen are smoothly integrated with interactivity.

Adding multidimensional interactive visualizations would allow users to explore the relationship between two or more variables, and to create cohorts based upon combinations of interest.

**Current Status:** Currently, DataScope has interactive visualizations, but only of a single variable each, and has some multidimensional visualizations, but they are noninteractive.

**Required Skills:** Javascript, D3 (recommended)

**Code Challenge:** Either from scratch or an existing toolkit, make a simple univariate interactive visualization. Alternatively, a meaningful bug report or contribution to the Datascope Repository.

**Community and Code License:** https://github.com/sharmalab/Datascope BSD 3-Clause License

**Slack room:** gsoc-emory-bmi.slack.com multidimensional-viz

***

**[2] Extensions to Bindaas Data Integration Middleware**

**Mentors:** Pradeeban Kathiravelu (pradeeban.kathiravelu -at- emory.edu) and Tushar Aggarwal (tushar1997 -at- gmail.com)

**Overview:** Bindaas is a service-based data framework that offers unified access and RESTful APIs to various data sources, such as MySQL, PostgreSQL, Mongo, and Apache Drill. Additional data service providers can be implemented for various data sources and access mechanisms such as HTTP access. Bindaas is the backbone of several production systems such as the Cancer Imaging Archive (TCIA).

There have been several proposals to improve Bindaas’ usability. There are several tasks to follow up.

First, more data source providers. Namely, we should extend Bindaas for cloud file systems and storages such as S3, by incorporating with the cloud CLIs.

Second, currently Bindaas limits its API to REST. We also propose to have more interfaces to Bindaas such as GraphQL query language interfaces, in addition to its RESTful interfaces.


**Expected results:** We are aiming for the Bindaas 4.5 release with the enhancements in place.

**Code challenge:** The students are expected to configure Bindaas locally during the application period to understand the code base and to illustrate their capability in completing this task. If the student manages to resolve one of the issues listed in https://github.com/sharmalab/bindaas/issues, it will make them a strong candidate.
   
**Required Skills:** Java, Web Services, Apache Maven, OSGi, GraphQL, Cloud Computing

**Community and Code License:**  https://github.com/sharmalab/bindaas Apache License 2.0

**Slack room:** gsoc-emory-bmi.slack.com bindaas

***

**[3] Performance Enhancements to Bindaas Data Integration Middleware**
 
**Mentors:**  Pradeeban Kathiravelu (pradeeban.kathiravelu -at- emory.edu) and Mohanapriya Narapareddy (mohanapriya.narapareddy -at- emory.edu)

**Overview:** Bindaas is a service-based data framework that offers unified access and RESTful APIs to various data sources, such as MySQL, PostgreSQL, Mongo, and Apache Drill. Additional data service providers can be implemented for various data sources and access mechanisms such as HTTP access. Bindaas is the backbone of several production systems such as the Cancer Imaging Archive (TCIA).

Performance is an essential aspect of the Bindaas framework. Therefore, there have been several proposals for improving Bindaas’ performance. This project aims to improve the performance of Bindaas by addressing some of those proposals.

First, better serialization of Bindaas internal representation with Protobuf, Kryo, or other efficient serialization and deserialization approaches.

Second, the SQLite-based audit logs have some performance and scalability limitation. The tight-coupling with SQLite should be removed, and replaced with a generic interface. Then, also implement persistence based on other data stores as alternatives. Consider Mongo and In-Memory Data Grids such as Infinispan and Hazelcast.

Third, Bindaas currently does not optimize its database queries. We should be able to reach better outputs than the database APIs themselves through query optimization.

**Expected results:** We are aiming for the Bindaas 4.5 release with the enhancements in place.

**Code challenge:** The students are expected to configure Bindaas locally during the application period to understand the code base and to illustrate their capability in completing this task. If the student manages to resolve one of the issues listed in https://github.com/sharmalab/bindaas/issues, it will make them a strong candidate.

**Required Skills:** Java, Web Services, Apache Maven, OSGi

**Community and Code License:** https://github.com/sharmalab/bindaas Apache License 2.0

**Slack room:** gsoc-emory-bmi.slack.com bindaas


***

**[4] TensorFlow-GUI: Graphical User Interface for Tensorflow**

**Mentors:**  Monjoy Saha (monjoy.saha -at- emory.edu)

**Overview:** This project aims to develop a graphical user interface (GUI) for any deep learning model development and visualization of outcomes based on the existing Tensorflow functions. This interface will act just like a simulator similar to MATLAB. This technique will be helpful for the beginners who don't have sufficient programming knowledge. Moreover, our proposed concept will help to maintain the quality of the work.
              
**Present Status of the work:** Preliminary work has been done and a TensorFlow-GUI has been implemented as part of GSoC 2019 project with Emory BMI organization. The GSoC 2020 student is expected to extend or utilize the work from the previous year.

There are very few organizations that are also working on the development of almost similar kind of tools. [Deep Cognition](https://deepcognition.ai/) is one of them. Though they have many limitations including the quality of the code/output and the number of users. This is not an open source software.
              
**Proposed Methodology:** We will use existing Tensorflow functions which will be converted into the blocks of layers (e.g., convolution, transpose convolution, pooling, ReLu, etc.). The parameters of each layer can be set as per the requirements of the model. Suppose in the case of convolution layer; the user can set the values of input, weight, bias, kernel dimensions, number of output channels, etc.
 
**Benefits:** The proposed GUI will be very much helpful for the beginners or who don't have sufficient knowledge of coding. This GUI will help in maintaining the quality of the work for Emory BMI researchers as well as the broader research community. The students also have the potential to submitting a pull request upstream to the Tensorflow community, if relevant.
 

**Deliverables:** GUI for Tensorflow model 

**Required Skills:** Tensorflow, Python

**Community and Code License:** https://github.com/sharmalab/tensorflow-gui GNU General Public License v3.0

**Slack room:** gsoc-emory-bmi.slack.com gui-tf

***

**[5] Sub-second queries on billion point datasets in Datascope**

**Mentors:**  Ganesh Iyer (ganesh.iyer -at- mgh.harvard.edu) and Sapoon Dutta (sapoon.dutta -at- emory.edu)

**Overview:** Datascope currently uses crossfilter.js on a Node application server to store data and perform queries on it. This project would involve refactoring Datascope’s backend to use other frameworks instead of Crossfilter. The student would develop capabilities that ensure that the Datascope’s declarative schema is compatible with the new application server.

Students can consider OLAP engines like [Kylin](http://kylin.apache.org) for the backend. However, as an open-ended problem we expect the student to propose their own solution and justify it.

**Required Skills:** Javascript

**Community and Code License:** https://github.com/sharmalab/Datascope BSD 3-Clause License

**Slack room:** gsoc-emory-bmi.slack.com datascope-queries

***


**[6] DataScope using serverless functions**

**Mentors:**  Ashish Sharma (ashish.sharma -at- emory.edu) and Ganesh Iyer (ganesh.iyer -at- mgh.harvard.edu)

**Overview:** DataScope is a framework for exploratory analysis on high dimensional datasets, especially biomedical datasets. 

During this project, the student would work towards making every request for DataScope stateless. Consequently, the whole application will be served via a content-delivery network (CDN).

**Required Skills:** Javascript, Serverless

**Code Challenge:** Students are expected to provide a meaningful bug report or contribution to the Datascope Repository to demonstrate their capability to complete this project successfully.

**Community and Code License:** https://github.com/sharmalab/Datascope BSD 3-Clause License

**Slack room:** gsoc-emory-bmi.slack.com datascope-serverless

***
