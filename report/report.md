---
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
Both of these events informed the content for the national-level workshop in August, 2025, with 43 participants from 11 universities, national laboratories, organizations, and companies across the United States.

:::{pull-quote}
This would have historically been considered too technically difficult to achieve for beginners.
:::

In all workshops, most participants and little to no experience with Pixi, and limited or no experience constructing software environments containing CUDA accelerated software packages.
As a result, the workshop participants had their effective first introduction to Pixi on the first day of the workshop.
Workshop participants were able to successfully deploy CUDA accelerated PyTorch machine learning workflows to remote GPUs on high-throughput computing (HPC) facilities by the last day of the workshop, using software environments that they had all individually constructed.
This represents a rapid technological adoption and deployment process that would have historically been considered too technically difficult to achieve for beginners.

### Workshop Survey Analysis

TBD

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

## Acknowledgements

This work was supported by the US Research Software Sustainability Institute (URSSI) via grant G-2022-19347 from the Sloan Foundation.

[^1]: The development home of HTCondor.
