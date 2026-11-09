
---
layout: default
title: "DSC 180A — Causal Discovery"
---

# DSC 180A — Methodology Assignment 4


**Name:** Uzair Gheewala  
**UCSD Email:** ugheewala@ucsd.edu  
**Section:** D04 — Learning and Using Causal Relationships from Multi-modality Data  
**Domain Mentor:** Professor Biwei Huang

## Quarter 2 Project Reflections

**1. What is the most interesting topic covered in your domain this quarter?**

While my efforts in the domain itself have largely been focused on looking at problem areas in the field of causal discovery, the most interesting topic would be that which we ended up moving forward with which is this attempt to enable clear and effectie diagnoses into said issues and ultimately resolutions of them through the development of a fully system-agnostic, end-to-end auditing system. The field is already moving into more general, autonomous reasoning systems, like Causal-Copilot, and with that comes ambiguity, especially because of the introduction of the use of LLMs in key decision-making parts of the pipeline. 

A causal relationship may be supported by an algorithm under certain assumptions, by repeated statistical tests, or by an LLM's understanding of the domain. These are not equivalent forms of justification, even if they ultimately produce the same directed edge in a causal graph. This leads us to ask: To what extent can context that is initially implicit or semantic be represented explicitly as entities, relations, assumptions, constraints, and evidence? If the operationally relevant parts of that context can be externalized, more of the reasoning process might become independently inspectable, reproducible, and verifiable. This is ultimately the thesis that is driving the development of my Q1 project which is the Crucis auditing system, designed to do exactly that.

**2. Describe a potential investigation you would like to pursue for your Quarter 2 Project.**

The Q1 project should end with a viable end to end audiitng system that's able to run every major causal discovery system out there on our range of benchmark datasets and is able to fuly derive the traces of origination of every edge and direction from the pipeline, as opposed to simply inspecting the final graph. The findings yielded from that investigation would prompt the pursuit and development of a causal discovey system that's able to satisfy all of the requirements of said auditor and then ideally excel at them, and by proxy achieve superior strength in the relevant metrics. 

One possible direction is an extension to Causal-Copilot in which each proposed causal relationship is accompanied by a structured record of how it was derived. Such a record might distinguish the statistical algorithm that proposed an edge, the assumptions under which it was inferred, its empirical stability, relevant domain knowledge, and any subsequent LLM or human modifications. By also then tracking how associated metrics like directed-F1 changes at each of these stages we'd iteratively understand where exactly the system makes mistakes that'd ultimately allow us to uncover the desired improvements.

**3. What is a potential change you'd make to the approach taken in your current Quarter 1 Project?**

The nature of the Q1 project is such that it needs a lot of runs ona  lot of datasets on a lot of systems as well which burns through availble capital quickly. Q2 will similarly need many tests so definign the sample sets of these larger datasets beforehand and taking a batch-based approach where we rerun tests after some set batch of improvements and clearly delineating hen a batch is completed would help optimize our capital utilization in relation to observed improvements.

**4. What other techniques would you be interested in using in your project?**

I am more so interested in typed intermediate representations, and explicit modeling of assumptions and evidence. These could potentially be used to separate statistical support, domain knowledge, and user-specified constraints without collapsing them into a single confidence score. Some level of generic intermediate, pipeline-stage-agnostic representations would be invaluable in better deciphering why a given stage of a pipeline is bulletproof versus being responsible for flaky F1 performances.