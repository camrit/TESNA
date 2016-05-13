TESNA is short for TEchnical Social Network Analysis
 
The TESNA tool creates visualisations of the social networks and calculates metrics to show the changes of the networks over time. The T loop corresponds to the Technical Module of TESNA. The Technical module reads input about relations or dependencies between tasks. It gets the data by mining the software repository versioning systems such as CVS and SVN. It uses JUNG for the visualisation of networks and uses https://github.com/camrit/DSM-clusterer.git for clustering

A high level description of what it can do:
In short, the following steps describe the TESNA method:
1.	Exploring Potential Coordination Requirements (PCRs)
a)	Deciding the patterns that are applicable
b)	Analysing the social network and/or the software architecture using the TESNA tool
c)	Analysing the visualisations and metrics produced by TESNA for the particular pattern
d)	Identifying PCRs related to the patterns
e)	Optionally, exploratory interviews can also be conducted.
2.	Verifying the appearance of a PCR: Verification is through interviews or with the help of a workshop presentation
3.	Identifying the reasons contributing to the PCR: Interview data and/or a feedback from a work-shop presentation are used to discover the reasons behind the PCR
Please note that the last part (3rd point above) of identifying reasons for the PCR is an optional part of the method. The procedure may be slightly different, like replacing the interviews with direct obser-vation etc. The details of the method, including how the interviews are conducted and analysed are de-scribed in the following sections.

Also see: Amrit C, Hillegersberg J. TESNA: A Tool for Detecting Coordination Problems.

To RUN:
change Manifest File in tesna.jar

with:
Manifest-Version: 1.0

Main-Class: Main
Class-Path: colt.jar jung-1.7.6.jar sdtv.jar org-netbeans-lib-cvsclient.jar xml-apis.jar xercesIm l.jar xalan.jar log4j.jar jh.jar jcvsii.jar jCharts-0.7.5.jar javasvn.jar javasvn-cli.jar javasvn-javahl.jar jakarta-oro.jar j2ssh-core.jar j2ssh-common.jar ganymed.jar DependencyFinder.jar commons-collections-3.2.jar commons-logging.jar colt.jar activation.jar resources.jar

run from command line with:

java  -vmargs  -Xms256m -Xmx1024m  -jar  tesna.jar
