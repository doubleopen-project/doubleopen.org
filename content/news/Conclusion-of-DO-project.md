+++ 
date = "2022-04-25T10:17:00+03:00" 
title = "Conclusion of the Double Open project" 
draft = false 
description = "The Double Open project officially concluded in June 2021" 
+++

### **Some great achievements from Double Open**

- Creation of a new [meta-layer for Yocto](https://github.com/doubleopen-project/meta-doubleopen) for the creation of SPDX files. The creation of SPDX files is now being developed in Open Embedded and available to all Yocto users in future versions of Yocto.
- Fossology implemented API functionality based on Double Open needs.
- Double Open is using the [OSS Review Toolkit (ORT)](https://github.com/doubleopen-project/ort) Evaluator and Reporter at the end of the pipeline.
- Acting as an interoperable bridge between different open source projects for creating an end-to-end automated compliance pipeline.

### **Achieving project objectives**

As a research project, the Double Open project set itself and achieved the following research objectives:

1. getting image-specific package and file information (SBOM) out of Yocto into the SPDX format,
2. relevant package, license and copyright data in SPDX format are stored,
3. license compliance of a Yocto project is automatically determined with the Policy Engine using license data from Fossology,
4. an end-to-end repeatable process which produces a supporting artefact and/or alerts for further actions,
5. automatically building a notice file for a Yocto project using copyright data from Fossology, and
6. enabling CVE monitoring based on the SBOM.

Double Open also aimed to find a way to synchronize the licensing data between two separate Fossology instances. The project did not achieve this goal, but we still consider this an important functionality and will continue to explore it in the future.

Therefore, the project has been deemed completed and a great success by the steering group. We have moved to the next stage, a market pilot, where the Double Open approach is refined for continued production for multiple projects. At the same time, we are testing the viability of continuing Double Open as a business.

As the Project Manager, I would like to thank all our collaborators and staff for the considerable effort you have put in to the project. This is the end of the project phase but a mere introduction to the whole story that is Double Open. Please see our upcoming posts regarding the results of Double Open along with links to our published code. Also check out our [GitHub repository](https://github.com/doubleopen-project), which is updated with a faster interval than this website.

**Toni Päärni**  
_Project Manager_
