+++ 
date = "2022-07-14T10:17:00+03:00" 
title = "Nordic Institute For Interoperability Solutions (NIIS) Using Double Open " 
draft = false 
description = "NIIS Case Study"
+++

_“With the help of Double Open, our third-party open-source component usage is now compliant all the time, and we have significantly reduced both the time needed in open-source compliance and the related administrative headaches.”_  
    
_Petteri Kivimäki, CTO at NIIS_  

![](/images/Kivimaki.png)

## Background

NIIS is a non-profit association that develops open-source solutions for digital government infrastructure. X-Road® and Harmony eDelivery Access software are the current products of NIIS. Both X-Road® and Harmony eDelivery Access rely on a significant number of third-party open-source (“OS”) dependencies as any modern software does.  

NIIS requested our assistance in bringing their software license compliance up to date for an upcoming release. This was a one-shot review for both products for a specific release only, and we included a NOTICE file that NIIS could distribute with the release. We also ensured that NIIS would be able to meet the obligations of all licences and that there would be no incompatibility between the licenses inside the products.

## Challenge

NIIS used a compliance process, at the heart of which was the constant tendering process of one-shot license reviews from third parties. In addition, all NIIS products contain multiple third-party OS components, containing dozens of dependencies and hundreds of transitive dependencies. The products use different technologies and multiple package management systems. In addition, not all dependencies are managed using package management systems, but some dependencies are included in the source repositories.  

In addition to the high cost of the compliance process formerly used by NIIS, the risk of a release-phase review is particularly high because the audit findings can be costly in the form of late changes and delayed releases or even cancelled releases. NIIS needed to reform its OS compliance processes. With finite resources to devote to compliance, the solution should be largely automated. Improving the process would also mean that NIIS must establish best practice policies and increase compliance competence for all employees.  

## Solution

After running both the X-Road® and Harmony eDelivery Access codebases through the OSS Review Toolkit ("ORT"), we at Double Open assessed the suitability of the codebase for the implementation of continuous use of ORT. ORT is a fully open-source OS license compliance tool designed to assist with tasks typically performed during OS license compliance reviews. It does this by organising a highly customisable toolkit that abstracts the underlying services.  

To create a near-automated process, OS Policies were needed to allow NIIS to understand and stipulate how to deal with different types of licenses. A machine-readable version of the OS Policies was also created to enable ORT to make independent decisions based on the OS Policies. We utilised Double Open's license-classifications.yml, a public OS license categorisation database created by Double Open.  

In addition to implementing ORT for the projects, we trained NIIS employees on using ORT. Currently, ORT runs as part of the NIIS CI/CD pipeline so that NIIS employees can manually trigger ORT when needed.  

## Experiences and benefits

ORT is initially a pretty complex toolkit and implementing it into a CI/CD pipeline requires technical and legal expertise. ORT's documentation is somewhat incomplete and aimed at technical people, but after user training and initial configuration, the operation is straightforward. However, nothing is fully automated, at least for the time being, and manual work is still required. Still, the workload at NIIS has decreased considerably compared to doing OS license compliance as third-party one-shot reviews for every release from scratch. Scaling ORT and adding new projects after the initial configuration is not challenging.  

After the implementation project, we conclude that NIIS' OS compliance maturity has increased, and the ability to manage OS compliance independently has improved significantly. Once we had implemented ORT into NIIS' CI/CD pipeline, NIIS remained an ongoing support customer for Double Open, allowing NIIS to contact us on an ongoing basis in situations where they need assistance. These include technical issues related to the use of ORT and legal matters such as the categorisation of individual new licenses or reviewing specific components inside their products.

## Background on NIIS, the association

Nordic Institute for Interoperability Solutions (NIIS) is a non-profit association with the mission to ensure the development and strategic management of X-Road® and other cross-border solutions for digital government infrastructure. The republics of Estonia, Finland and Iceland are members of NIIS.  

NIIS is both a network and cooperation platform and executioner of IT developments in members’ common interests. The institute focuses on practical collaboration, sharing of experience and promoting innovation. The operating model of the institute is something unique in the world.

