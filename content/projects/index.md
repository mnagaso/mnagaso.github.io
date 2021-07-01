---
title: Projects
---


# My former and current projects


## I/O optimization and designing/developing a workflow toward a full-wave inversion calculation on Exascale HPC machines.
This is a project (part of my postdoc works) for code optimization towards a use on Exascale High Performance Computers or supercomputers.  
The I/O is one of the significant bottleneck for achieving a scalable computation (the ratio between the number of processors and the computation time is enoughly close to a linear),
because the limitation of file I/O bandwidth blocks the other computing processes.
For avoid this waiting time, I implemented an advanced way of using multi-processors, i.e. preparing some I/O dedicated nodes (we call this I/O server) then the computing process may do only their computation while actual I/O processes are done on only the I/O servers, which realize an asynchronous I/O.

## Full wave inversion and development of pre/post processing tool for massive amount of seismic observation data.
This is the project (part of my postdoc works) to realize a seismic tomography using Spectral Element Method and Full wave inversion for studying the subsurface structure of Japanese islands.
I am developing an Gui application for downloading, pre/post-processing, configurating a set of files/scripts for running a full wave inversion and shipping the massive seismic observation data to HPC and computation clusters.
![img](/images/img_for_cheese.png)
![img](/images/ppff.png)

## Network clustering application
Implementation of hierarchical network clustering code, based on Map equation (Rosvall 2008, 2010, 2011) and Modularity (Clauset 2004).  
The search algorithm may be selected from Louvain method (Blondel 2008) or Modified Louvain method (Rosvall 2010).  
For the calculation of transition probability, the users may select Standard teleportation, Recorded link teleportation or Unrecorded link teleportation (Lambiotte 2012).  
Convergence calculation is done by Arnoldi method or Power method.  

Keywords: Map equation, Modularity, Louvain method, Page rank
![img](/images/clustering.png)
 
## The numerical computation library for estimation of subject times
Python library for calculating the subject time (i.e. temporal position indicating the degree of progress in a disease) written in C++ and wrapped by swig.  
In the calculation routine of this library, nonlinear mixed effect modeling was implemented for calculating averaged curves of multiple bio-markers (i.e. fixed effects) and random parts which depends on each subject.  
Golden search algorithm was also implemented during the routine.  
This code was developed as a part of research project by Dr. Keita Tokuda, a project researcher at The University of Tokyo Hospital.  
Keywords: Maximum likelihood estimation, Nonlinear mixed effect model, Golden search
<!-- ![img](/images/sreft.png) -->

## Improvement of multi-label classification using C2AE and fine-tuning with Transformer-lm
In order to improve the accuracy of multi-label classification task with Canonical Correlated AutoEncoder (C2AE) for limited amount of input texts, we applied the method of "Improving Language Understanding by Generative Pre-Training" so called (finetune-transformer-lm).  
Keywords: Natural language processing, Deep Learning, multi-label classification, Transformer, Language model, C2AE

## Generation of semantic networks with review texts of popular products and generation of learning model for creating a new hit product
This is a part of another research project on "computational creativity" by Dr. Akihito Sudo, a researcher/research manager at The University of Shizuoka.  
First, we generates two semantic networks, one is generated from reviews texts written for a hit product and another is from reviews for multiple products in the category which the target product belongs to.  
By using these semantic networks and difference between them as a data set, we are trying to generate learning model to generate keywords for the next hit products.  
Keywords: Natural language processing, word2vec, Semantic network, Machine learning, SMOTE

## Web scraping scripts
This is a set of scraping scripts developed for gathering review texts from Amazon.com/co.jp for generating semantic networks concerning the above project.  
A python library "Scrapy" was used as the engine of scraping spiders.  
Keywords: Web Scraping
