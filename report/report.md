---
numbering:
  heading_1: true
  heading_2: true
exports:
  - format: pdf
    template: lapreprint-typst
    output: exports/feickert-urssi-report-2025.pdf
    id: feickert-urssi-report-2025
downloads:
  - id: feickert-urssi-report-2025
    title: PDF export
---
# Matthew Feickert's 2025 URSSI Early-Career Fellowship Report

## Overview

As part of inaugural US Research Software Sustainability Institute (URSSI) Early-Career Fellow Matthew Feickert's fellowship research, he developed an open source course on creating reproducible software environments for scientific and AI/ML applications.
The project "[Reproducible Machine Learning Workflows for Scientists](https://urssi.us/blog/2025/04/25/urssi-welcomes-first-early-career-fellows/)" focused on using the open source tool [Pixi](https://pixi.sh/) to create fully reproducible research software environments with specialized hardware accelerator support.
In addition to performing research on creating robust reproducible hardware accelerated workflows with Pixi, Feickert organized and taught a pilot workshop at the University of Wisconsin&ndash;Madison, a tutorial at the 2025 SciPy conference, and a national-level workshop at the University of Wisconsin&ndash;Madison.

## Summary of Project

TBD

## Project Outcomes

The main deliverable of the project was to create permissively licensed open source educational material and executable examples for real scientific software applications with a focus on AI/ML.
The educational material was also scoped to be contributed as a lesson module to [The Carpentries Incubator](https://github.com/carpentries-incubator/proposals).
The workshop materials were proposed to [The Carpentries Incubator as a contribution](https://github.com/carpentries-incubator/proposals/issues/222) at the project onset, and all materials were developed under the `carpentries-incubator` GitHub organization at https://github.com/carpentries-incubator/reproducible-ml-workflows.
The produced material was piloted at an initial workshop for University of Wisconsin&ndash;Madison students and staff in June, 2025.
Feedback received on the pilot workshop's most critical points was incorporated into a condensed four hour tutorial taught at the SciPy 2025 conference with the lead developer of Pixi, Ruben Arts, and NVIDIA principal engineer, John Kirkham, who lead the technical work for the distribution of the CUDA software stack as conda packages.
Both of these events informed the content for the national-level workshop in August, 2025, with 44 participants from 11 universities, national laboratories, organizations, and companies across the United States.

:::{pull-quote}
This would have historically been considered too technically difficult to achieve for beginners.
:::

In all workshops, most participants and little to no experience with Pixi, and limited or no experience constructing software environments containing CUDA accelerated software packages.
As a result, the workshop participants had their effective first introduction to Pixi on the first day of the workshop.
Workshop participants were able to successfully deploy CUDA accelerated PyTorch machine learning workflows to remote GPUs on high-throughput computing (HPC) facilities by the last day of the workshop, using software environments that they had all individually constructed.
This represents a rapid technological adoption and deployment process that would have historically been considered too technically difficult to achieve for beginners.

<!--
### Workshop Survey Analysis

TBD
-->

### Workshops and Events

* [Reproducible Machine Learning Workflows for Scientists Workshop Pilot 2025](https://indico.global/event/14745/), Matthew Feickert. June 16-17, 2025.
* [SciPy 2025 tutorial on Reproducible Machine Learning Workflows for Scientists with Pixi](https://github.com/matthewfeickert-talks/reproducible-ml-for-scientists-with-pixi-scipy-2025), Matthew Feickert, Ruben Arts, John Kirkham. July 7, 2025.
* [Reproducible Machine Learning Workflows for Scientists Workshop 2025](https://indico.global/event/14982/), Matthew Feickert. August 12-14, 2025.

### Research Products and Publications

* Matthew Feickert, [Reproducible Machine Learning Workflows for Scientists](https://github.com/carpentries-incubator/reproducible-ml-workflows), 2025.
* Matthew Feickert, Ruben Arts, John Kirkham, _[Reproducible Machine Learning Workflows for Scientists with Pixi](https://inspirehep.net/literature/3071594)_, Proceedings of 24th International SciPy Conference — SciPy 2025, July, 2025. DOI: [10.25080/nwuf8465](https://doi.org/10.25080/nwuf8465)

### Contributions to Open Source Projects

* Addition of Pixi workflow templates to the University of Wisconsin&ndash;Madison's Center for High Throughput Computing[^1] [GPU Job Templates GitHub repository](https://github.com/CHTC/templates-GPUs).

### Future Opportunities and Collaborations

The Brookhaven National Laboratory [National Synchrotron Light Source II](https://www.bnl.gov/nsls2/) (NSLS-II) [Data Science and Systems Integration](https://www.bnl.gov/nsls2/datascience/) (DSSI) division sent staff to the August, 2025 national-level workshop.
Following the workshop, the DSSI has invited Feickert to BNL in 2026 to give a guest workshop for NSLS-II scientists and staff, as they are looking to modernize their beamline software application deployments.

## Project Review

### Expected Impact

The project proposal's expected impact on the Scientific Software Community was focused on the long-term impact of the training and education imparted at the workshop to the research communities of the workshop participants.
From the post-workshop survey and from the 3 month long-term follow-up survey there is evidence that Pixi as a technology is easy to learn and is beneficial enough for researchers that it has changed their normal scientific software workflows habits, becoming a common tool in their regular work.
The workshop and material had a particular focus on CUDA accelerated workflows for applications on GPUs.
While this was a popular topic in the workshop and was noted by participants as an area of interest for participating, few participants had existing software projects that were actively making use of CUDA or GPUs for scientific tasks where hardware acceleration would be beneficial, e.g. machine learning.
While the reasons for this are not well understood, a hypothesis is that while the hardware and hardware acceleration technologies are important and useful, to gain access to them and use them effectively at traditional academic institutions requires multiple steps and levels of permissions, which can act as a deterrent to rapid experimentation.
While the workshop materials provide instruction and examples at each step of this procedure, and use of Pixi and CUDA conda packages significantly lowers the  complexity of the software management, the computing platforms used may have a large impact on adoption of demonstrated workflows in normal research.
As shown in @computing_comparison, deploying fully reproducible software environments to a computing facility for use generally requires researchers to use at least one additional computing technology beyond Pixi, with each additional technology potentially requiring multiple supporting files or actions to use.
Improvements in the levels of interfacing between computing systems and researchers may have a positive effect on the widespread adoption and impact of fully reproducible hardware accelerated software environments.

:::{table} Comparison of common computing facility management solutions for scientific research and the number of distinct technologies required to use fully reproducible software environments with them. The use of `*` indicates a potential or optional dependency. Note that HTCondor systems with shared file systems are uncommon.
:label: computing_comparison
:align: center

| Computing resource management system | Shared file system |  Technologies required |
| --- | --- | --- |
| High-throughput computing  | No  | Pixi, Linux containers, HTCondor       |
| High-throughput computing  | Yes | Pixi, HTCondor                         |
| High-performance computing | Yes | Pixi, Slurm                            |
| Commercial cloud services  | Yes | Pixi, Slurm*, cloud specific software* |

:::

### Evaluation Metrics and Deliverables

The project evaluation metrics for success are reported in @evaluation_metrics.
The total number of participants across all workshops is reported from the in-person attendance of the June, 2025 pilot workshop (29 participants), the SciPy 2025 tutorial (56 participants), and the August, 2025 national-level workshop (44 participants).
Additionally, as not all national-level workshop participants brought their own research projects, the reported percentage (42/44 participants) includes those that executed examples workflows.
Under these conditions, all participants in the national-level workshop succeeded in executing CUDA accelerated ML workflows except for two, who had been delayed by technical difficulties earlier in the workshop.
During the duration of the Fellowship project, [The Carpentries Lab](https://carpentries-lab.org/) was reviewing lesson submissions [by invitation only](https://github.com/carpentries-lab/reviews/blob/80deafff58555e8eae2944f7ee0506d7d737b48d/README.md#what-is-the-process-for-submitting-a-lesson-to-the-carpentries-lab).
This, along with additional criteria discussed in @section_additional_funding, made it not possible to submit to The Carpentries Lab review process.
The workshop materials will instead be submitted to the [Journal of Open Source Education](https://jose.theoj.org/) (JOSE).

:::{table} Summary of project success evaluation metrics as defined in the Fellowship proposal.
:label: evaluation_metrics
:align: center

| Evaluation metric | Target | Delivered | Metric achieved |
| --- | --- | --- | --- |
| Total number of participants across all workshops | 50 participants | 129 participants | Yes |
| Percentage of participants who were able to successfully reproduce their own scientific and AI/ML research workflows using the information they learned by the end of the national-level workshop | 90% | ~95% | Yes |
| Acceptance of the workshop educational materials into The Carpentries Incubator and The Carpentries Lab curriculum | The Carpentries Lab | The Carpentries Incubator | No |

:::

Of the twelve milestone and deliverables established in the Fellowship proposal, all were met or delivered, with the exception of:
* The deliverable of a second pilot workshop at University of Wisconsin&ndash;Madison based on development time constraints.
* The deliverable of submission of the workshop material for peer review to The Carpentries Lab given the previously mentioned restrictions.

(section_additional_funding)=
### Potential Impact of Additional Funding

In the event in which additional research funding would have been available to extend the Fellowship project, the project would have supported additional more targeted workshops.
The registration for the August, 2025 national-level workshop reached its room capacity in under one week of registration being opened, and there were requests for additional registration slots to be opened indicating interest and demand for the material.
There was also a limited number of lodging stipend awards that were available for participants to apply for to offset the costs associated with travel to the workshop location in Madison, Wisconsin.
Additional funding would have allowed for follow up workshops and additional lodging stipend awards to make the in-person workshop training accessible to more scientific communities.

In addition, feedback in the post-workshop survey and discussion with The Carpentries Incubator community, indicates that the scope of technologies covered in the existing workshop material may be too much for some researchers to be able to fully understand and apply in a workshop that lasts less than one week.
It has been recommended by The Carpentries Incubator that the current material be split into three successive "lessons"[^2] focusing on: Pixi, deployment technologies with Linux containers, and machine learning workflows at HTC and HPC facilities.
Additional funding support would allow for the redesign of the current material into individual lessons that could be more easily taught by additional instructors, which is [a requirement for peer review](https://github.com/carpentries-lab/reviews/blob/80deafff58555e8eae2944f7ee0506d7d737b48d/README.md#essential) of lesson submissions to The Carpentries Lab.
This would also allow for multiple, more targeted workshops to be taught that might attract different researchers, or for more technical workshops that use the succession of lesson development to require higher levels of prerequisite skills.

## Acknowledgements

This work was supported by the US Research Software Sustainability Institute (URSSI) via grant G-2022-19347 from the Sloan Foundation.

[^1]: The development home of HTCondor.
[^2]: The Carpentries Incubator lessons map roughly to individual workshops.
