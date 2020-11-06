# About this Repo

This repo is a starting-point for folks interested in getting involved in TL-Verilog-related projects (for h/w folks and s/w folks).

# Learning Resources for TL-Verilog

Numerous trainings, videos, papers, and posts can be found on the [Redwood EDA Publications](https://www.redwoodeda.com/publications) page.

The [Makerchip.com](https://www.makerchip.com) IDE contains tutorials for learning TL-Verilog.

TL-Verilog is an evolving language with evolving tools and infrastructure. Several important features are actively being explored and documentation for these is limited:
  - M4 macro preprocessing is being used to explore parameterization and code generation in TL-Verilog before proper TL-Verilog features are defined. [M4 docs](https://www.gnu.org/savannah-checkouts/gnu/m4/manual/m4-1.4.18/index.html) are available, but the particular use of M4 with TL-Verilog is considered transitional, and is currently undocumented.
  - Visualization features are under development at Redwood EDA and have been utilized in online workshops. Documentation is not yet available, but several projects are underway to benefit from these features. Ask me ([Steve Hoover](emailto:steve.hoover@redwoodeda.com)) about early access.

# Community

After you work through the available training material on your own and feel comfortable with TL-Verilog basics, feel free to ask me ([Steve Hoover](emailto:steve.hoover@redwoodeda.com)) for access to the TL-Verilog User's Slack group. You'll find other newcomers and experienced developers listening in who can help you learn more.

# Starter Projects

After you work through the available training material, and before you contribute to a "real" project, try some small-scale development of your own. Here are a few ideas:

  - Find an IP on [OpenCores](https://opencores.org/) and convert to TL-Verilog
  - Ramp up on [1st CLaaS](https://github.com/stevehoover/1st-CLaaS) and create a simple hardware kernel that can be executed from a web application. You'll find a few simple demo applications in this repository that you can reference as examples.


# Project Repos

Here are a few noteworthy TL-Verilog project repositories:
  - [1st ClaaS](https://github.com/stevehoover/1st-CLaaS): A framework for developing hardware accelerated web and cloud applications using cloud FPGAs.
  - RISC-V:
    - [MYTH Workshop](https://github.com/stevehoover/RISC-V_MYTH_Workshop): A workshop offered by Redwood EDA and VLSI System Design. The repo indexes a few [CPU cores developed by students of the workshop](https://github.com/stevehoover/RISC-V_MYTH_Workshop/blob/master/student_projects.md) which serve as a good reference for RISC-V using TL-Verilog.
    - [WARP-V](https://github.com/stevehoover/warp-v): A CPU core generator that makes heavy use of M4 macro preprocessing and the flexibility of TL-Verilog to support different ISAs, pipeline depths, etc.
  - [https://github.com/stevehoover/tlv_flow_lib](TL-Verilog FLow Library): A library of building-block components in TLV/M4 utilizing transaction flow (`$ANY`) to enable microarchitectures to be constructed quickly and easily.
  - [https://github.com/stevehoover/makerchip_examples](https://github.com/stevehoover/makerchip_examples): In addition to those examples that can be found inside the Makerchip IDE, these are a few more examples of TL-Verilog logic for Makerchip.


# TL-Verilog-Related Project Ideas

A number of open-source projects have been proposed that you might want to participate in.

## Community Platform

Just as GitHub builds a community of open-source developers and [Scratch](https://scratch.mit.edu/) fosters interest in software development in a younger audience, this project aims to build momentum for open-source hardware. Similar efforts include [OpenCores](http://opencores.org/) and [LibreCores](https://www.librecores.org/). This project could be a collaboration or integration with those platforms or a project of its own. Specifically, this project aims to integrate seamlessly with the Makerchip IDE.

Features would include:
  - Project/IP cataloging:
    - sharing
    - characterizing
    - searching
    - evaluating/scoring
  - User profiles with skill certification.
  - Discussion boards (probably external).

**Required skills**
 - full-stack web development

## TL-VHDL/TL-C/TL-Clash/etc.

TL-Verilog is a Verilog implementation of TL-X, and currently Verilog is the only target language for TL-X. This project would see through the vision of layering transaction-level support on other languages. TL-VHDL would help to broaden the reach of the technology. TL-C would connect transaction-level design with high-level synthesis. And, TL-Clash would explore the integration of transaction-level modeling with a stronger type system among other language benefits.

**Required skills**
  - Hardware modeling in TL-Verilog, VHDL, System-C, and/or [Clash](https://qbaylogic.com/).
  - Java

## Visualization

Makerchip will soon support "Visual Debug" (VIZ), a feature that enables custom visualization of circuit simulation, coded in JavaScript. This feature has many potential uses and is getting a lot of attention, even before public release within Makerchip.

### Visualization for basic digital logic instruction

VIZ can be used to illustrate basic logic functions and concepts like logic gates, K-maps, pipelines, etc. This project would develop these visualizations.

**Required skills**
  - JavaScript
  - Basic TL-Verilog

### Visualization of SweRV

The SweRV core is an RISC-V CPU core developed by Western digital. It is an interesting core for college course and is being highlighted in the [RVfpga course](https://www.imgtec.com/news/press-release/imagination-announces-the-first-risc-v-computer-architecture-course/) for one. Visualizing the operation of the core can greatly enhance the learning experience. This project aims to do so.

This project is underway in collaboration with [Manoj Sharma at IIT Delhi](https://www.ece.bvcoend.ac.in/site/home/index/319). Collaborators are welcomed.

**Required skills**
  - JavaScript
  - CPU microarchitecture
  - SystemVerilog

### ...

BaseJump STL and BlackParrot
TLV Flow Library
…
Curriculum material
Online tutorial components for Makerchip.

