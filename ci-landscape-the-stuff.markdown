---
author:
- Mike Renfro\inst{1,2}
institute:
  - \inst{1}Tennessee Tech University
  - \inst{2}Campus Champions Leadership Team
title: "The Cyberinfrastructure Landscape: Systems, Providers, Technologies"
date: 2024-06-25
aspectratio: 169
theme: Cookeville
colorlinks: true
linkcolor: white
filecolor: white
citecolor: blue
urlcolor: blue
section-titles: false
toc: false
---

### Who am I? (Who are any of us, really?)

::: {.columns align=center}
::: {.column width=50%}
#### Back in the day
- ME student at a medium-sized public STEM-ish university who should have studied more instead of helping people do things in computer labs.
- Sysadmin/CAD/FEA co-op student at Oak Ridge National Lab before SGI Irix got its cameo in "Jurassic Park" ("It's a Unix system: I know this!").
:::

::: {.column width=50%}
![Some skinny nerd, 1990]

[Some skinny nerd, 1990]: figures/mike-1990.jpg { width=100% }
:::
:::

::: notes
x
:::

### Who am I? (Who are any of us, really?)

::: {.columns align=center}
::: {.column width=70%}
#### Now
- Three ME degrees from the now-R2 university (1995, 1998, 2018)
- Mostly-solo practitioner of all things RCD at the same university (2000--2017, 2017--)
- Perpetually online member of multiple RCD organizations (2018--)
- Member of Campus Champions Leadership Team (2022--)
- Compulsive advice-giver
:::

::: {.column width=30%}
![Same nerd, not remotely skinny, 2023]

[Same nerd, not remotely skinny, 2023]: figures/mike-2023.jpg { width=100% }
:::
:::

::: notes
x
:::

# Computational and/or Storage Resources

## National Science Foundation

### ACCESS Allocations Portal

::: {.columns align=top}
::: {.column width=80%}

![](figures/access-allocations-home.png){ width=80% }

https://allocations.access-ci.org/

:::
::: {.column width=20%}
[![](figures/qr-access-allocations-home.png)](https://allocations.access-ci.org/)
:::
:::

### ACCESS Resource Catalog

::: {.columns align=top}
::: {.column width=80%}

![](figures/access-resource-catalog.png)

:::
::: {.column width=20%}
[![](figures/qr-access-resource-catalog.png)](https://allocations.access-ci.org/resources/)
:::
:::

### Stampede3 at Texas Advanced Computing Center (TACC)

::: {.columns align=top}
::: {.column width=80%}

- 20 Intel Sapphire Rapids nodes each with 4 Intel GPUs, 128 GB HBM
- 560 Intel Sapphire Rapids nodes (no GPUs), 128 GB HBM
- 1060 Intel Skylake nodes, 192 GB RAM
- 224 Intel Ice Lake nodes, 256 GB RAM
- 10 PB VAST (`$SCRATCH`) + 1 TB Lustre (`$WORK`)
- 100 Gb Omni-Path networking
- Intended for:
  - parallel applications scalable to 10,000+ cores
  - general purpose computing
  - throughput computing

:::
::: {.column width=20%}
[![](figures/qr-stampede3.png)](https://docs.tacc.utexas.edu/hpc/stampede3/)
:::
:::

::: notes
x
:::

### Delta at National Center for Supercomputing Applications (NCSA)

::: {.columns align=top}
::: {.column width=80%}

- All using AMD 7763 CPUs
- 132 nodes with 128 cores and 256 GB RAM
- 100 nodes with 64 cores, 256 GB RAM, and 4 NVIDIA A40 CPUs
- 100 nodes with 64 cores, 256 GB RAM, and 4 NVIDIA A100 GPUs
- 6 nodes with 128 cores, 2048 GB RAM, and 8 NVIDIA A100 GPUs
- 1 node with 128 cores, 2048 GB RAM, and 8 AMD MI100 GPUs
- 6 PB Lustre for `$HOME` and `$SCRATCH`
- 200 Gb HPE/Cray Slingshot networking

:::
::: {.column width=20%}
[![](figures/qr-delta.png)](https://docs.ncsa.illinois.edu/systems/delta/)
:::
:::

::: notes
x
:::

### Bridges-2 at Pittsburgh Supercomputing Center (PSC)

::: {.columns align=top}
::: {.column width=80%}

- 488 nodes with 128 AMD 7742 cores and 256 GB RAM
- 16 nodes with 128 AMD 7742 cores and 512 GB RAM
- 4 nodes with 96 Intel Cascade Lake cores and 4096 GB RAM
- 24 nodes with 40 Intel Cascade Lake cores, 512 GB RAM, and 8 NVIDIA V100 GPUs (32 GB)
- 9 nodes with 40 Intel Cascade Lake cores, 192 GB RAM, and 8 NVIDIA V100 GPUs (16 GB)
- 1 node with 48 Intel Skylake cores, 1536 GB RAM, and 16 NVIDIA V100 GPUs (32 GB)
- 15 PB Lustre for `$PROJECT`
- 200 Gb Infiniband networking

:::
::: {.column width=20%}
[![](figures/qr-bridges-2.png)](https://www.psc.edu/resources/bridges-2/)
:::
:::

::: notes
x
:::

### ACES at Texas A&M University

::: {.columns align=top}
::: {.column width=80%}

- 130 nodes, 11888 cores
- Mostly Intel Sapphire Rapids, some Intel Ice Lake, Intel Cascade Lake, and AMD Rome
- Tons of mostly-composable accelerators:
  - GPUs: NVIDIA H100 and A30, Intel (coming soon)
  - FPGAs: Bittware Agilex, Intel D5005
  - Coprocessors: NextSilicon
  - Optane memory modules
- Non-composable accelerators:
  - Graphcore IPUs: GC200, Bow-2000
  - NEC Vector Engine: Type 20B-P
- 2.3 PB Lustre
- 200 Gb Infiniband networking

:::
::: {.column width=20%}
[![](figures/qr-aces.png)](https://hprc.tamu.edu/kb/Quick-Start/ACES/)
:::
:::

::: notes
x
:::

### Jetstream2 at Indiana University

::: {.columns align=top}
::: {.column width=80%}

- Hybrid-cloud platform for flexible, on-demand, programmable cyberinfrastructure tools
- Interactive virtual machine services
- Infrastructure and orchestration services for research and education
- AMD Milan CPUs (128 per node)
- 360 NVIDIA A100 GPUs
- 512--1024 GB RAM
- 100 Gb Ethernet

:::
::: {.column width=20%}
[![](figures/qr-jetstream2.png)](https://docs.jetstream-cloud.org/)
:::
:::

::: notes
x
:::

## Department of Energy

### Advanced Scientific Computing Research (ASCR)

::: {.columns align=top}
::: {.column width=80%}

![](figures/doe-ascr.png){ width=80% }

:::
::: {.column width=20%}
[![](figures/qr-ascr.png)]()
:::
:::

::: notes
x
:::

### Accessing ASCR Facilities

::: {.columns align=top}
::: {.column width=80%}

- [Innovative and Novel Computational Impact on Theory and Experiment (INCITE)](https://www.alcf.anl.gov/science/incite-allocation-program): multi-year awards for open science using majority of machine at Oak Ridge or Argonne
- [ASCR Leadership Computing Challenge (ALCC)](https://science.osti.gov/ascr/Facilities/Accessing-ASCR-Facilities/ALCC): 1-year awards for advancing DOE mission or broadening the community capable of using large computing resources at Oak Ridge, Argonne, or NERSC
- [Energy Research Computing Allocations Process (ERCAP)](http://www.nersc.gov/users/accounts/): 1-year awards for advancing DOE Office of Science and SBIR/STTR mission at NERSC
- Center Reserves: 1-year awards for advancing science and engineering fields at [Oak Ridge](https://www.olcf.ornl.gov/support/getting-started/olcf-director-discretion-project-application/), [Argonne](http://www.alcf.anl.gov/directors-discretionary-dd-program), or [NERSC](https://www.nersc.gov/users/accounts/allocations/first-allocation/)

:::
::: {.column width=20%}
[![](figures/qr-ascr-accessing.png)](https://science.osti.gov/ascr/Facilities/Accessing-ASCR-Facilities)
:::
:::

::: notes
x
:::

# Services/Consultancies

## MATCH Plus

### Multi-tier Assistance, Training & Computational Help (MATCH) Plus

::: {.columns align=top}
::: {.column width=80%}

MATCH Plus:

- takes requests from researchers with a support need,
- identifies a student and mentor that can provide that support,
- connects the researcher to the student and mentor with regular meetings and updates,
- for 5--10 student hours and 2--3 mentor hours per week for 3--6 months,
- at **no charge**.

:::
::: {.column width=20%}
[![](figures/qr-match.png)](https://support.access-ci.org/match/overview)
:::
:::

::: notes
x
:::

## MATCH Premier

### Multi-tier Assistance, Training & Computational Help (MATCH) Premier

::: {.columns align=top}
::: {.column width=80%}

MATCH Premier:

- takes requests from already-funded projects,
- identifies an expert consultant and arranges payment,
- for a 6--12 month period.

:::
::: {.column width=20%}
[![](figures/qr-match.png)](https://support.access-ci.org/match/overview)
:::
:::

::: notes
x
:::

## Engagement and Performance Operations Center (EPOC)

### Engagement and Performance Operations Center (EPOC)

::: {.columns align=top}
::: {.column width=80%}
> EPOC provides researchers with a holistic set of tools and services needed to debug performance issues and enable reliable and robust data transfers. By considering the full end-to-end data movement pipeline, EPOC is uniquely able to support collaborative science, allowing researchers to make the most effective use of shared data, computing, and storage resources to accelerate the discovery process.

-- https://epoc.global/
:::

::: {.column width=20%}
[![](figures/qr-epoc.png)](https://epoc.global/)
:::
:::

::: notes
x
:::

## Science Gateways

### Science Gateways

::: {.columns align=top}
::: {.column width=80%}

> [Science g]ateways are online interfaces that give researchers, educators, and students easy access to shared resources that are otherwise inaccessible or unaffordable for a large segment of the scientific community.
>
> ...
>
> The SGCI was founded to provide services and resources that advance the state of the art in science gateways, that help gateway creators use accepted practices in developing and operating gateways, and that catalyze the formation of a community that may be diverse in discipline but has a common need to advance science through gateways.

:::

::: {.column width=20%}
![](figures/sgx3.png)

![](figures/sgci.png)

[![](figures/qr-sg.png)](https://sciencegateways.org)
:::
:::

::: notes
x
:::

# Tools and Software

## OpenHPC

### OpenHPC

::: {.columns align=top}
::: {.column width=80%}
> OpenHPC is a Linux Foundation Collaborative Project whose mission is to provide a reference collection of open-source HPC software components and best practices, lowering barriers to deployment, advancement, and use of modern HPC methods and tools.
>
> OpenHPC components and best practices will enable and accelerate innovation and discoveries by broadening access to state-of-the-art, open-source HPC methods and tools in a consistent environment, supported by a collaborative, worldwide community of HPC users, developers, researchers, administrators, and vendors.

-- https://openhpc.community/about-us/

:::

::: {.column width=20%}
![](figures/ohpc_logo.png)

[![](figures/qr-openhpc.png)](https://openhpc.community/)
:::
:::

::: notes
x
:::

## Open XDMoD

### Open XDMoD

x

::: notes
x
:::

## Open OnDemand

### Open OnDemand

x

::: notes
x
:::

## ColdFront

### ColdFront

x

::: notes
x
:::

## Spack

### Spack

x

::: notes
x
:::
