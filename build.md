# This manual describe configuration of FHIR.EE website

## Requirements
- The all resources should be acessible over *https*.
- Web content should be available as static files.
- All content should be managed over GithHub.
- Temporary artefacts should accesible over build.fhir.ee
- User shoud have the way to configure redirects through Github.

## Site map
### URLs
- https://fhir.ee - Official artefacts
- htttps://build.fhir.ee - Build artifacts, such as results of CI builds

### build.fhir.ee
Contains build artefacts. Initially it is builds of Implementation Guides.
- htttps://build.fhir.ee/ig - the root for latest build of IG, For example: 
  - htttps://build.fhir.ee/ig/ee-base - The latest build of Estonian Base Implementation Guide
  - htttps://build.fhir.ee/ig/mpi - The latest build of Master Patient Inde (MPI) Implementation Guide

### fhir.ee
Contains offcial artefacts and web site
- \ (root) - The content of current project startting from directory "root"
- \ImplementationGuide - the root for latest official of IG, For example: 
  - htttps://fhir.ee/ImplementationGuide/ee-base - The official version of Estonian Base Implementation Guide
  - htttps://fhir.ee/ImplementationGuide/mpi - The official version of Master Patient Inde (MPI) Implementation Guide
- redirects - The ability to specify Ngnix instructions to rewrite location of the different resources (mostly terminology). It includes:
  - CodeSystem
  - ValueSet
  - NamingSystem

### www.fhir.ee
Redirects to fhir.ee.
  
