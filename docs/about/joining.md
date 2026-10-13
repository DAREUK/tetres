---
icon: lucide/user-round-group
title: Joining TETREs
---

# Joining TETREs

This will eventually be a formal guide to joining TETREs, or for setting up a new federation following the TETREs model.

In the meantime if you are interested in getting involved (and helping to develop this document!) please open an [issue on GitHub](https://github.com/DAREUK/tetres/issues).

## Document outline

!!! info "This is a speculative draft outline"

    Everything is up for discussion, and can be changed.
    All feedback is welcome!

### Scope

This will define the scope of the document.
Most likely it will cover the technical requirements to enable TREs to run federated analysis applications.
Details of the applications and how to configure them will most likely be out of scope, but may be covered in other documents.

### Terminology

Several terms will be used throughout the document, such as "federation".
The terms used will be defined here or in a relevant external glossary.

### 1. Prerequisites: Agreement to join the federation

A federation is an agreement between a group of organisations to work together.
TETREs will evaluate tools for managing a federation, but will not mandate them.
Ultimately new and existing members must mutually agree to work with each other regardless of the technologies or platforms in use.

Details of how to reach this agreement are outside the scope of TETREs.

### 2. Central shared services

TETREs will have a set of centrally managed services.

These central services _may_ include:

- Registry services holding the definitive list of organisations in the federation and the services each node is running
- Central oversight of networking between TREs
- Authentication, Authorisation and Accounting Infrastructure
- Key and/or certificate management

The requirements for these and other shared services will be defined in this document.

### 3. Technology choices for connecting TREs

This will document the vendor agnostic requirements for a system such as an encrypted mesh network for connecting TREs together.
It will also describe the chosen open-source implementation(s) and configuration(s) for TETREs.

### 4. Requirements for each node

Every TRE node connecting to TETREs will need to configure their systems to communicate with other TREs and shared services, following the choices in the previous sections.

This will likely be a combination of:

- Configuration of an organisation's network perimeter, for example firewall rules
- Deployment of components inside the organisation's network boundary to allow restricted communication between a TRE and external services
- There may be reporting/auditing services that each node must run

### 5. Standards for running federated applications

As TETREs develops we will see if there are any standards that can be defined for running federated applications.
It is entirely possible that this is not feasible due to the wide variety of analysis workloads that will be run in TREs.
