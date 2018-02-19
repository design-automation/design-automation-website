---
layout: dexen
title: Overview
---

# Overview

Dexen is an execution environment for running computationally demanding jobs on distributed computing resources. These include cloud based infrastructures such as Amazon EC2.

Dexen consists of a number of components that run on networked computers in the cloud. The three main components are: a server computer that is the core of the system and manages all communication; one or more node computers that have workers that execute the actual tasks defined by the job; and one database that is used to store all data associated with the running job.

{% include fig.html file="dexen.png" caption="The Dexen architecture." %}

Dexen allows end users to run computationally demanding jobs on distributed computing resources. These jobs can have complex dependencies, including arbitrary resources and other existing software systems. For example, jobs can be executed that rely on APIs and resources provided by third-part 3D modelling or simulation software.

Within Dexen, a job consists of a set of tasks that get triggered when data objects become available. The end user can develop a set of tasks and uploaded them to the server. The system will schedule and execute the tasks on a set of workers in parallel, with all data input and output automatically being stored in the database. The user is then able to view the data in the database, for example in order to download results that have been evolved.

Dexen has an inbuilt flexibility and robustness due to the fact that the tasks only communicate via data. This allows the system to automatically discover which tasks to execute at any time. Each task can be executed multiple times and can create, modify, and delete data objects. Such data objects may contain any type of data – from simple types to arbitrary blobs of data, such as 3D models of design variants saved as files.

This flexibility makes Dexen ideal for running optimisation jobs. For example, in order to run an evolutionary optimization algorithm, the end-user can define and upload the tasks for the evolutionary process, including development, evaluation, and feedback. These tasks will then be executed by as an when data becomes available in the database: the development task when new genotypes are added to the database, the evaluation task when unevaluated phenotypes are added to the database, and the feedback task when the population has grown enough to allow selection and reproduction to be performed.

{% include fig.html file="optimisation.png" caption="Example of a Pareto graph showing a population of building designs evolved using Dexen. (The example is based on the Interlace in Singapore.)" %}

Creating tasks still requires the user to write code. This is challenging for end-users with limited programming skills. To address this, a tool has been created to partially automate the creation of these various procedures. For more information, see the Eddex site.
