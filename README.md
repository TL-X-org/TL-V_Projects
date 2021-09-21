# About this Repo

This repo (containing just this README) is a starting-point for folks interested in getting involved in TL-Verilog-related projects (for both hardware folks and software/web-dev folks). These projects are a great opportunity to:
  - showcase your talents
  - develop new skills
  - build your resume
  - get involved with technology that can shape the future of the silicon industry
  - prepare to apply for Google Summer of Code
  - collaborate in academic research
  - publish a papers



# Learning Resources for TL-Verilog

I (Steve Hoover) enjoy working with students and collaborators. I've worked with many, and I've been asked by many (~100) to provide mentorship. Before you ask, show that you can be of value. If you are interested in working with TL-Verilog, take initiative to begin ramping up on your own.

Numerous trainings, videos, papers, and posts can be found on the [Redwood EDA Publications](https://www.redwoodeda.com/publications) page.

The [Makerchip.com](https://www.makerchip.com) IDE contains tutorials for learning TL-Verilog.

TL-Verilog is an evolving language with evolving tools and infrastructure. Several important features are actively being explored and documentation for these is limited:
  - M4 macro preprocessing is being used to explore parameterization and code generation in TL-Verilog before proper TL-Verilog features are defined. [M4 docs](https://www.gnu.org/software/m4/manual/m4.html) are available, but the particular use of M4 with TL-Verilog is considered transitional, and is currently undocumented.
  - Visualization features are under development at Redwood EDA and have been utilized in online workshops. Documentation is not yet available, but several projects are underway to benefit from these features. Ask me ([Steve Hoover](mailto:steve.hoover@redwoodeda.com)) about early access.



# Community

*After* you work through the available training materials and feel comfortable with TL-Verilog basics, feel free to [join the TL-Verilog User's Slack workspace](https://join.slack.com/t/tl-verilog-users/shared_invite/zt-4fatipnr-dmDgkbzrCe0ZRLOOVm89gA). You'll find other newcomers and experienced developers listening in who can help you learn more.



# Starter Projects

Before you contribute to a "real" project, try some small-scale development of your own. Here are a few ideas:

  - Find an IP on [OpenCores](https://opencores.org/) and [convert it to TL-Verilog](https://docs.google.com/document/d/18AYcWFQ_rgxVqJzelHW0R04xILlcEkh5Uz9R0QMBxUQ/edit?usp=sharing)
  - Ramp up on [1st CLaaS](https://github.com/stevehoover/1st-CLaaS) and create a simple hardware kernel that can be executed from a web application. You'll find a few simple demo applications in this repository that you can reference as examples.
  - Develop a TL-Verilog FPGA project using this [Virtual FPGA Lab](https://github.com/BalaDhinesh/Virtual-FPGA-Lab).


# Project Repos

Here are a few noteworthy TL-Verilog project repositories:
  - [1st ClaaS](https://github.com/stevehoover/1st-CLaaS): A framework for developing hardware accelerated web and cloud applications using cloud FPGAs.
  - RISC-V:
    - [MYTH Workshop](https://github.com/stevehoover/RISC-V_MYTH_Workshop): A workshop offered by Redwood EDA and VLSI System Design. The repo indexes a few [CPU cores developed by students of the workshop](https://github.com/stevehoover/RISC-V_MYTH_Workshop/blob/master/student_projects.md) which serve as a good reference for RISC-V using TL-Verilog.
    - [WARP-V](https://github.com/stevehoover/warp-v): A CPU core generator that makes heavy use of M4 macro preprocessing and the flexibility of TL-Verilog to support different ISAs, pipeline depths, etc.
  - [TL-Verilog FLow Library](https://github.com/stevehoover/tlv_flow_lib): A library of building-block components in TLV/M4 utilizing transaction flow (`$ANY`) to enable microarchitectures to be constructed quickly and easily.
  - [Makerchip Examples](https://github.com/stevehoover/makerchip_examples): In addition to those examples that can be found inside the Makerchip IDE, these are a few more examples of TL-Verilog logic for Makerchip.
  - [Virtual FPGA Lab](https://github.com/BalaDhinesh/Virtual-FPGA-Lab): A virtual FPGA lab environment for Makerchip and supporting scripts for local FPGA deployment.
  - [Block-Based TL-Verilog](https://github.com/ninja3011/Block_Based_Circuit_Design): A WIP block-based programming utility for developing in TL-Verilog.



# TL-Verilog-Related Project Ideas

A number of open-source projects have been proposed that you might want to participate in.

## Community Platform

**Status**: Underway (no github link yet)

Just as GitHub builds a community of open-source developers and [Scratch](https://scratch.mit.edu/) fosters interest in software development in a younger audience, this project aims to build momentum for open-source hardware. Similar efforts include [OpenCores](http://opencores.org/) and [LibreCores](https://www.librecores.org/). This project could be a collaboration or integration with those platforms or a project of its own. Specifically, this project aims to integrate seamlessly with the Makerchip IDE for a community of Makerchip users.

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

**Discussion**: [TL-Verilog User's Slack workspace](https://join.slack.com/t/tl-verilog-users/shared_invite/zt-4fatipnr-dmDgkbzrCe0ZRLOOVm89gA) `#community-platform` channel.


## 1st CLaaS for Local FPGAs

[1st ClaaS](https://github.com/stevehoover/1st-CLaaS) supports web application communication with FPGA logic in the cloud. It would be nice to support local FPGA use cases as well. This is useful for local applications as well as to support development that will ultimately be deployed to the cloud.

**Discussion**: [TL-Verilog User's Slack workspace](https://join.slack.com/t/tl-verilog-users/shared_invite/zt-4fatipnr-dmDgkbzrCe0ZRLOOVm89gA) `#1st-claas` channel.

**Required skills**:
  - FPGAs
  - 1st CLaaS


## World CLaaS: Open FPGA Cloud

The vision is to enable individuals with FPGAs (World CLaaS Citizens) to share their hardware with the world. The system would include three (open-source) parts:

  - Citizens (of the World): An FPGA resource contributed to the World.
  - World: A registry of World Citizens available for Jobs/Missions. Interest (permission) is based on tokens (that can be provided to certain Causes, users, etc.).
  - Mission/Job API: Use by an application of a Citizen of the World (categorized by "Causes").

Billing support would come after the open system for voluntary contributions and could be based on Stripe and/or digital currencies.

This would build on "1st CLaaS for Local FPGAs" above.

**Required skills**
  - Cloud development


## TL-VHDL/TL-C/TL-Clash/etc.

TL-Verilog is a Verilog implementation of TL-X, and currently Verilog is the only target language for TL-X. This project would see through the vision of layering transaction-level support on other languages. TL-VHDL would help to broaden the reach of the technology. TL-C would connect transaction-level design with System-C and therefore high-level synthesis. And, TL-Clash would explore the integration of transaction-level modeling with a stronger type system among other language benefits.

**Required skills**
  - Hardware modeling in TL-Verilog, VHDL, System-C, and/or [Clash](https://qbaylogic.com/).
  - Java


## TL-UVM

In theory, TL-X should be applicable to UVM as well. Since UVM does not have open-source support, no one has yet tried. But it would be great to uncover issues and put together examples. It looks like Modelsim supports UVM and is freely available for Intel FPGAs. There might be other options.

**Required skills**
  - UVM
  - TL-Verilog


## Visualization

Makerchip supports "Visual Debug" (VIZ), a feature that enables custom visualization of circuit simulation, coded in JavaScript. Though a documented API with long-term support is not yet available, several folks are using it in its current, temporary form in projects like these.

**Discussion**: [TL-Verilog User's Slack workspace](https://join.slack.com/t/tl-verilog-users/shared_invite/zt-4fatipnr-dmDgkbzrCe0ZRLOOVm89gA) `#viz` channel.


### Visualization for basic digital logic instruction

VIZ can be used to illustrate basic logic functions and concepts like logic gates, K-maps, pipelines, etc. This project would develop these visualizations. Bala Dhinesh implemented [basic logic gates](http://www.makerchip.com/sandbox?code_url=https:%2F%2Fraw.githubusercontent.com%2Fstevehoover%2Fmakerchip_examples%2Fmaster%2Flogic_gates.tlv).

**Required skills**
  - JavaScript and VIZ
  - Basic TL-Verilog


### Visualization of SweRV

The SweRV core is an open-source SystemVerilog RISC-V CPU core developed by Western Digital. It is an interesting core for college course and is being highlighted in the [RVfpga course](https://www.imgtec.com/news/press-release/imagination-announces-the-first-risc-v-computer-architecture-course/) for one. Visualizing the operation of the core can greatly enhance the learning experience. This project aims to do so. SweRV is be built and simulated within Makerchip in [this repo](https://github.com/stevehoover/SweRV_VIZ).

**Required skills**
  - JavaScript and VIZ
  - CPU microarchitecture
  - SystemVerilog

**Discussion**: [TL-Verilog User's Slack workspace](https://join.slack.com/t/tl-verilog-users/shared_invite/zt-4fatipnr-dmDgkbzrCe0ZRLOOVm89gA) `#swerv-viz` channel.


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

![virtual lab](https://user-images.githubusercontent.com/64545984/130665673-63e52c11-f5e4-4290-8d05-a5a0741fbbbd.png)

**Status**: Developed as a Google Summer of Code 2021 project [here](https://github.com/BalaDhinesh/Virtual-FPGA-Lab), written up in this [blog](https://medium.com/@m.baladhinesh/fpgas-in-your-browser-bb92be1c1fa3), and used in this [free course](https://github.com/stevehoover/GettingStartedWithFPGAs).

1st CLaaS and Makerchip are great online tools to enable virtual FPGA lab classes. This project provides lab resources that mimic the physical lab experience to provide an easy path for migration of physical lab classes.

This project uses VIZ to represent the FPGA board, matching the spec of ones commonly used in labs, with LEDs, 7-segment displays, and/or video monitors. The experience will be enhanced by additional support in Makerchip for a VCD (waveform) streaming interface for 1st CLaaS (where each time-step is a 1st CLaaS chunk plus a timestamp). Shell logic will provide a shim between FPGA kernel logic as spec'ed for the virtualized FPGA and the 1st CLaaS interface.

Possible enhancements:
  - Support for additional FPGA boards can be added.
  - Course content can be enhanced.
  - An integration with [FuseSoC](https://github.com/olofk/fusesoc) probably makes sense.

**Required skills** (for multiple participants)
  - JavaScript and VIZ
  - TL-Verilog
  - 1st CLaaS

**Discussion**: [TL-Verilog User's Slack workspace](https://join.slack.com/t/tl-verilog-users/shared_invite/zt-4fatipnr-dmDgkbzrCe0ZRLOOVm89gA) `#virtual-fpga-lab` channel.


## TL-Verilog Support in Edalize

Just a thought. Haven't explored it at all, but a few lines of code should be sufficient to call [SandPiper-SaaS](https://pypi.org/project/sandpiper-saas/). Here's [Edalize](https://github.com/olofk/edalize).


## Tutorial/Gamification Content Creation

There are many opportunities to provide fun tutorials and gamified learning content for TL-Verilog that could be incorporated into Makerchip.

**Required skills**
  - TL-Verilog
  - Makerchip
  - VIZ
  - Web development (JavaScript, HTML, CSS, React(?), npm)


## WARP-V Configurator

**Status**: Done (http://warp-v.org)

This project adds a web front-end to WARP-V for configuration. The configured WARP-V core (or many-core) can be opened in Makerchip. This project is sketched out in a [WARP-V repo wiki page](https://github.com/stevehoover/warp-v/wiki/WARP-V-Configuration-Front-End)

**Required skills**
  - TL-Verilog
  - M4
  - Web development (JavaScript, HTML, CSS, React(?), NodeJS/npm)

**Discussion**: [TL-Verilog User's Slack workspace](https://join.slack.com/t/tl-verilog-users/shared_invite/zt-4fatipnr-dmDgkbzrCe0ZRLOOVm89gA) `#warp-v-configurator` channel.


## WARP-V Many-core Accelerator Microservice

**Status**: Google Summer of Code 2021 project

This project brings together three others:
  - [WARP-V](https://github.com/stevehoover/warp-v)
  - [TL-Verilog FLow Library](https://github.com/stevehoover/tlv_flow_lib)
  - [1st ClaaS](https://github.com/stevehoover/1st-CLaaS)
It will provide a configurable, easily-modifiable many-core-on-FPGA hardware accelerator deployed as a microservice to accelerate web and cloud applications.

Development from Google Summer of Code 2021 is merged into the [WARP-V repo](https://github.com/stevehoover/warp-v). Student: Vineet Jain. Primary Mentor: Akos Hadnagy. [Blog](https://medium.com/@vineetajm1999/developing-applications-for-cloud-fpgas-are-easier-than-you-think-6b39b7010412).

**Required skills** (for multiple participants)
  - TL-Verilog
  - Many-core CPU microarchitecture
  - 1st CLaaS
  - Xilinx FPGA development

**Discussion**: [TL-Verilog User's Slack workspace](https://join.slack.com/t/tl-verilog-users/shared_invite/zt-4fatipnr-dmDgkbzrCe0ZRLOOVm89gA) `#warp-v-manycore` channel.


## Implementing other ISAs in WARP-V 

WARP-V currently has support for RISC-V, (incomplete) MIPS, and a toy educational ISA. PowerPC is also open now and could be implemented, in addition to any other open ISAs.


## Neural Net

Vineet Jain created a simple <a href="https://github.com/vineetjain07/DNN_TL-V">configurable neural network model in TL-Verilog</a>. This could follow a similar path to WARP-V w/ a configurator and cloud FPGA implementation. The WARP-V configurator is build in a modular fashion to support this easily.

**Required skills**
  - Web development (JavaScript, HTML, CSS, React, NodeJS, etc.)
  - TL-Verilog
  - M4


## TensorCore Accelerator for Machine Learning

![TensorCore](https://user-images.githubusercontent.com/11302288/134257557-0132a79d-da4c-4435-b952-7a9cda1537b3.png)

Nitin Mishra began this project in Google Summer of Code 2021, mentored by Theodore Omtzigt. More in [the repo](https://github.com/natu4u/GSOC_TensorCore) and this [blog post](https://medium.com/@nmishra9/tensorcore-extension-for-deep-learning-41728fc22495).


## FractalValley

![fractalvalley](https://user-images.githubusercontent.com/11302288/134257481-e43618a9-a3de-4623-9c6d-75a1b009c076.png)

[FractalValley.net](http://www.fractalvalley.net) is a fun demo of 1st CLaaS and TL-Verilog. This project turns the demo into a robust site showcasing the value of hardware-acceleration in the cloud and the fun world of fractals.

**Required skills**
  - Web development (JavaScript, HTML, CSS, React, NodeJS, etc.)


## TL-Verilog Editor Modes

![TLX_code](https://user-images.githubusercontent.com/11302288/134257374-6fa3667f-e160-494e-92ee-e47f0ab6a394.png)

This general category of smaller projects improves the ecosystem for TL-Veriog development by creating editor support for various text editors and IDEs. Many editor modes already exist. A few possibilities include:
  - Adding JavaScript editing support within the TL-Verilog mode for Code Mirror (used by Makerchip) for `\viz` blocks
  - Improved support for M4 editing in TL-Verilog mode for Code Mirror.
  - GitHub support for TL-Verilog


## TL-Blockly

![TL-Blockly](https://raw.githubusercontent.com/ninja3011/Block_Based_Circuit_Design/1802073c6e71c49b56cf544a3d3c5c6db43d926a/assets/Pythagorean.gif)

**Status**: Google Summer of Code 2021 project, Ninad Jangle. [blog](https://ninja3011.github.io/Block_Based_Circuit_Design/) [repo](https://github.com/ninja3011/Block_Based_Circuit_Design), [application](https://gsoc-block-based-circuit-design-site.netlify.app/)

[Blockly](https://developers.google.com/blockly) is a framework for creating drag-and-drop block-based programming environments that are especially great for kids. It looks like it would be fairly straight-forward to create a block-based TL-Verilog edito that could be incorporated into Makerchip (without support for M4).

**Discussion**: [TL-Verilog User's Slack workspace](https://join.slack.com/t/tl-verilog-users/shared_invite/zt-4fatipnr-dmDgkbzrCe0ZRLOOVm89gA) `#blockly` channel.


## EDA Microservices
  
Makerchip currently supports simulation of Verilog and TL-Verilog code. It is expanding to support logic synthesis and other physical flows as well as support for other HDLs. This project will provide various microservices that run open-source eda tools that can be incorporated into Makerchip.
  
  **Required skills**
    - Open-source EDA
    - Cloud development
    - Docker


## TL-Verilog Timing Reports

This project will help designers to relate timing information from synthesis tools back to TL-Verilog's higher-level context (hierarchy, pipelines, and transactions). Scripts are needed to map RTL signal names to their original TL-Verilog names. This will be applied to timing reports from open source synthesis tools so timing information can be reported with respect to TL-Verilog source code.

