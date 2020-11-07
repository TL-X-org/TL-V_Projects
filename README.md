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
  - [TL-Verilog FLow Library](https://github.com/stevehoover/tlv_flow_lib): A library of building-block components in TLV/M4 utilizing transaction flow (`$ANY`) to enable microarchitectures to be constructed quickly and easily.
  - [Makerchip Examples](https://github.com/stevehoover/makerchip_examples): In addition to those examples that can be found inside the Makerchip IDE, these are a few more examples of TL-Verilog logic for Makerchip.


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
  - JavaScript and VIZ
  - Basic TL-Verilog

### Visualization of SweRV

The SweRV core is an open-source SystemVerilog RISC-V CPU core developed by Western digital. It is an interesting core for college course and is being highlighted in the [RVfpga course](https://www.imgtec.com/news/press-release/imagination-announces-the-first-risc-v-computer-architecture-course/) for one. Visualizing the operation of the core can greatly enhance the learning experience. This project aims to do so.

This project is underway in collaboration with [Manoj Sharma at IIT Delhi](https://www.ece.bvcoend.ac.in/site/home/index/319). Collaborators are welcomed.

**Required skills**
  - JavaScript and VIZ
  - CPU microarchitecture
  - SystemVerilog

### Visualization for BaseJump STL

[BaseJump STL](https://gitlab.com/black-parrot/basejump_stl) is a library of SystemVerilog components used in the design of [Black Parrot](https://pdfs.semanticscholar.org/f4e8/fc065db9fadcb6b800718bd1f083ffac058a.pdf). This might be a good candidate for use of VIZ, both for Black Parrot and to augment BaseJump STL with generic visualization. This would explore the use of generic visualization of SystemVerilog components.

**Required skills**
  - JavaScript and VIZ
  - Many-core CPU microarchitecture
  - SystemVerilog

### Visualization of the TLV Flow Library

This project adds visualization to components in the [TL-Verilog FLow Library](https://github.com/stevehoover/tlv_flow_lib). It explores encapsulation of visualization and aspect-oriented visualization that decouples transaction visualization from component visualization.

**Required skills**
  - JavaScript and VIZ
  - TL-Verilog (expert-level)
  - M4

## Virtual FPGA Lab

1st CLaaS and Makerchip are great online tools to enable virtual FPGA lab classes. This project aims to provide lab resources that mimic the physical lab experience to provide an easy path for migration of physical lab classes.

This project will utilize VIZ to represent the FPGA board, matching the spec of one(s) commonly used in labs, with LEDs, 7-segment displays, and/or video monitors. The experience will be enhanced by additional support in Makerchip for a VCD streaming interface for 1st CLaaS (where each time-step is a 1st CLaaS chunk plus a timestamp). Shell logic will provide a shim between FPGA kernel logic as spec'ed for the virtualized FPGA and the 1st CLaaS interface.

**Required skills** (for multiple participants)
  - JavaScript and VIZ
  - TL-Verilog
  - 1st CLaaS

## Tutorial/Gamification Content Creation

There are many opportunities to provide fun tutorials and gamified learning content for TL-Verilog that could be incorporated into Makerchip.

**Required skills**
  - TL-Verilog
  - Makerchip
  - VIZ
  - Web development (JavaScript, HTML, CSS, React(?), npm)

## WARP-V Configurator

This project adds a web front-end to WARP-V for configuration. The configured WARP-V core (or many-core) can be opened in Makerchip.

**Required skills**
  - TL-Verilog
  - M4
  - Web development (JavaScript, HTML, CSS, React(?), NodeJS/npm)

## WARP-V Many-core Accelerator Microservice

This project brings together three others:
  - WARP-V
  - TL-Verilog Flow Library
  - 1st CLaaS
It will provide a configurable, easily-modifiable many-core-on-FPGA hardware accelerator deployed as a microservice to accelerate web and cloud applications.

A ring-based WARP-V many-core is WIP in the WARP-V repo. This project will continue the momentum and explore this new compute paradigm.

**Required skills** (for multiple participants)
  - TL-Verilog
  - Many-core CPU microarchitecture
  - 1st CLaaS
  - Xilinx FPGA development

## FractalValley

[FractalValley.net](http://www.fractalvalley.net) is a fun demo of 1st CLaaS and TL-Verilog. This project turns the demo into a robust site showcasing the value of hardware-acceleration in the cloud and the fun world of fractals.

**Required skills**
  - Web development (JavaScript, HTML, CSS, React, NodeJS, etc.)

## TL-Verilog Editor Modes

This general category of smaller projects improves the ecosystem for TL-Veriog development by creating editor support for various text editors and IDEs. Many editor modes already exist. A few possibilities include:
  - Adding JavaScript editing support within the TL-Verilog mode for Code Mirror (used by Makerchip) for `\viz` blocks
  - Improved support for M4 editing in TL-Verilog mode for Code Mirror.
  - GitHub support for TL-Verilog
