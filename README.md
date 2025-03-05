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

I enjoy working with students and collaborators. I've worked with many, and I've been asked by many (100+) to provide mentorship. Before you ask, show that you can work independently. If you are interested in working with TL-Verilog, take initiative to begin ramping up on your own.  --Steve Hoover

Numerous trainings, videos, papers, and posts can be found on the [Redwood EDA Publications](https://www.redwoodeda.com/publications) page.

The [Makerchip.com](https://makerchip.com) IDE contains tutorials, courses, and documentation for learning TL-Verilog, Visual Debug (VIZ), and code generation with M5 (coming soon). (LLMs should learn [here](https://gitlab.com/rweda/Makerchip-public).)



# Community

*After* you work through the available training materials and feel comfortable with TL-Verilog basics, feel free to [join the TL-Verilog User's Slack workspace](https://join.slack.com/t/tl-verilog-users/shared_invite/zt-4fatipnr-dmDgkbzrCe0ZRLOOVm89gA). You'll find other newcomers and experienced developers listening in who can help you learn more.



# Starter Projects

Before you contribute to a "real" project, try some small-scale development of your own. Here are a few ideas:

  - Find a digital IP on [OpenCores](https://opencores.org/) or elsewhere and [convert it to TL-Verilog](https://docs.google.com/document/d/18AYcWFQ_rgxVqJzelHW0R04xILlcEkh5Uz9R0QMBxUQ/edit?usp=sharing)
  - Ramp up on [1st CLaaS](https://github.com/os-fpga/1st-CLaaS) and create a simple hardware kernel that can be executed from a web application. You'll find a few simple demo applications in this repository that you can reference as examples.
  - Develop a TL-Verilog FPGA project using this [Virtual FPGA Lab](https://github.com/os-fpga/Virtual-FPGA-Lab).


# Project Repos

Here are a few noteworthy TL-Verilog project repositories:
  - [1st ClaaS](https://github.com/os-fpga/1st-CLaaS): A framework for developing hardware accelerated web and cloud applications using cloud FPGAs.
  - RISC-V:
    - [MYTH Workshop](https://github.com/stevehoover/RISC-V_MYTH_Workshop): A workshop offered by Redwood EDA and VLSI System Design. The repo indexes a few [CPU cores developed by students of the workshop](https://github.com/stevehoover/RISC-V_MYTH_Workshop/blob/master/student_projects.md) which serve as a good reference for RISC-V using TL-Verilog.
    - [WARP-V](https://github.com/stevehoover/warp-v): A CPU core generator that makes heavy use of [M5](https://github.com/rweda/M5) preprocessing and the flexibility of TL-Verilog to support different ISAs, pipeline depths, etc.
  - [TL-Verilog FLow Library](https://github.com/stevehoover/tlv_flow_lib): A library of building-block components in TLV/M4 utilizing transaction flow (`$ANY`) to enable microarchitectures to be constructed quickly and easily.
  - [Makerchip Examples](https://github.com/stevehoover/makerchip_examples): In addition to those examples that can be found inside the Makerchip IDE, these are a few more examples of TL-Verilog logic for Makerchip.
  - [Virtual FPGA Lab](https://github.com/os-fpga/Virtual-FPGA-Lab): A virtual FPGA lab environment for Makerchip and supporting scripts for local FPGA deployment.
  - [Block-Based TL-Verilog](https://github.com/ninja3011/Block_Based_Circuit_Design): A WIP block-based programming utility for developing in TL-Verilog.
  - [Rapid Prototyping of Hardware Accelerators on Xilinx FPGAs (RPHAX)](https://github.com/shariethernet/RPHAX): RPHAX provides a quick automation flow to develop and prototype hardware accelerators on Xilinx FPGAs, including deployment of these FPGAs in the cloud.



# TL-Verilog-Related Project Ideas

A number of open-source projects have been proposed that you might want to participate in.

## AI Circuit Design

AI opens up a world of possibilities.

### AI Writing TL-Verilog

TL-Verilog creates an important separation between behavior and implementation. Implementation (especially timing, today) can be safely modified without introducing bugs. This enables implementation engineers to safely change RTL without disturbing designers and verification engineers. The same separation that helps humans work together is particularly valuable when working with AI. TL-Verilog elevates the abstraction level below which we can safely allow AI to optimize our circuits.

Furthermore, the elevated thought process embodied in TL-Verilog provides a framework for AI reasoning as it does for human reasoning. While today's AI models do not understand TL-Verilog, future AI models will be more capable of designing correct and optimal logic using TL-Verilog than Verilog.

The future of AI circuit design is destined to use TL-Verilog.


### Code Conversion

Code conversion (Verilog -> TL-Verilog) automation is one of the key missing enablers for the proliferation of TL-Verilog. AI is the perfect tool to fill this gap. LLMs are capable of addressing the nuances of code conversion in ways that traditional software never would. For example, rewriting comments to make sense in the context of a TL-Verilog representation of a design versus a Verilog representation.


### AI Writing VIZ Code

The challenge with releasing AI on a hardware model is preventing the introduction of bugs. There is more opportunity for AI in verification, which is the largest pool of effort in the design process anyway. One aspect of verification where AI can play a valuable role is in helping designers write [Visual Debug](https://redwoodeda.com/viz) code. This code improves productivity, and it can be wrong without significant repercussions. LLMs are already competent with JavaScript. They must be taught the VIZ API, best practices, and common patterns.


## Community Platform

Just as GitHub builds a community of open-source developers and [Scratch](https://scratch.mit.edu/) fosters interest in software development in a younger audience, this project aims to build momentum for open-source hardware. Similar efforts include [OpenCores](http://opencores.org/) and [LibreCores](https://www.librecores.org/). This project could be a collaboration or integration with those platforms or a project of its own. Specifically, this project aims to integrate seamlessly with the Makerchip IDE for a community of Makerchip users.

Features would include:
  - Project/IP cataloging:
    - sharing
    - characterizing
    - searching
    - evaluating/scoring
  - User profiles with skill certification.
  - Discussion boards (probably external).

**Status**: Underway (no github link yet)

**Required skills**
 - React, databases, and generally full-stack web development

**Discussion**: [TL-Verilog User's Slack workspace](https://join.slack.com/t/tl-verilog-users/shared_invite/zt-4fatipnr-dmDgkbzrCe0ZRLOOVm89gA) `#community-platform` channel.


## 1st CLaaS for Local FPGAs

[1st ClaaS](https://github.com/os-fpga/1st-CLaaS) supports web application communication with FPGA logic in the cloud. It would be nice to support local FPGA use cases as well. This is useful for local applications as well as to support development that will ultimately be deployed to the cloud.

[F4PGA](https://f4pga.org/) and [Apio](https://github.com/FPGAwars/apio) are worth considering.

**Discussion**: [TL-Verilog User's Slack workspace](https://join.slack.com/t/tl-verilog-users/shared_invite/zt-4fatipnr-dmDgkbzrCe0ZRLOOVm89gA) `#1st-claas` channel.

**Required skills**:
  - FPGAs
  - 1st CLaaS


## World CLaaS: Open FPGA Cloud

The vision is to enable individuals with FPGAs (World CLaaS Citizens) to share their hardware with the world. The system would include three (open-source) parts:

  - Citizens (of the World): An FPGA resource contributed to the World.
  - World: A registry of World Citizens available for Jobs/Missions. Interest (permission) is based on tokens (that can be provided to certain Causes, users, etc.).
  - Mission/Job API: API for a Citizen to serve a Cause (aka the API to run an FPGA accelerator)..

Billing support would come after the open system for voluntary contributions and could be based on Stripe and/or digital currencies. Vendor licenses might restrict this to open-source FPGA tools. Some notes on hosting FPGAs can be found here: https://medium.com/@shariethernet/quick-remote-fpga-lab-setup-without-vpn-port-forwarding-firewall-configurations-and-other-ccd45489ab35.

This would build on "1st CLaaS for Local FPGAs" above, and relates to [RPHAX](https://github.com/shariethernet/RPHAX).

**Related Tech**:
  - the [Boinc](https://boinc.berkeley.edu/) framework for distributed democratized compute clouds and the backbone for [Seti at Home](https://setiathome.berkeley.edu/)
  - the [HTCondor](https://htcondor.org/htcondor/overview/) software suite serving the [Open Science Pool](https://osg-htc.org/services/open_science_pool.html) operated by the [OSG Consortium](https://osg-htc.org/about/introduction/)

**Status**: [RPHAX](https://github.com/shariethernet/RPHAX) is a step in this direction.

**Required skills**
  - Cloud development


## TL-VHDL/TL-C/TL-Clash/etc.

TL-Verilog is a Verilog implementation of TL-X, and currently Verilog is the only target language for TL-X. This project would see through the vision of layering transaction-level support on other languages. TL-VHDL would help to broaden the reach of the technology. TL-C would connect transaction-level design with System-C and therefore high-level synthesis. And, TL-Clash would explore the integration of transaction-level modeling with a stronger type system among other language benefits.

**Required skills**
  - Hardware modeling in TL-Verilog, VHDL, System-C, and/or [Clash](https://qbaylogic.com/).
  - Java


## TL-UVM

Timing abstration and transaction flow are beneficial to verification modeling as well as to hardware modeling. [Verifying a RISC-V in 1 Page of Code!](https://www.semiwiki.com/forum/content/7850-verifying-risc-v-1-page-code-e.htmlTL-X) demonstrates extreme benefits for test harness modeling. In this work the verification modeling is SystemVerilog. We have yet to explore what can be done with UVM. With rapid progess recently on open-source
UVM support in Verilator, experimenting with UVM is becoming more feasible. Also, It looks like Modelsim supports
UVM and is freely available for Intel FPGAs. This project would expore what is possible with the two technologies
today and where further development might be necessary to achieve the combined benefits.

**Required skills**
  - UVM
  - TL-Verilog


## Visualization

Makerchip supports "Visual Debug" (VIZ), a feature that enables custom visualization of circuit simulation, coded in JavaScript. The following projects aim to bring the hardware world in life in beautiful colors.

**Discussion**: [TL-Verilog User's Slack workspace](https://join.slack.com/t/tl-verilog-users/shared_invite/zt-4fatipnr-dmDgkbzrCe0ZRLOOVm89gA) `#viz` channel.


### Visualization for basic digital logic instruction

VIZ can be used to illustrate basic logic functions and concepts like logic gates, K-maps, pipelines, etc. This project would develop these visualizations.

**Status**: Bala Dhinesh implemented [basic logic gates](http://www.makerchip.com/sandbox?code_url=https:%2F%2Fraw.githubusercontent.com%2Fstevehoover%2Fmakerchip_examples%2Fmaster%2Flogic_gates.tlv).

**Required skills**
  - JavaScript and VIZ
  - Basic TL-Verilog


### Control and Status Registers

Control and status registers (CSRs) are key elements of a digital design. Register description languages (RDLs), are used to provide a single source for their definitions that can be shared by RTL, system-level modeling, software, documentation, etc. SystemRDL seems to be the leading standard. There are open-source options for SystemRDL compilation.
Here are two:

  - [SystemRDL-Compiler](https://github.com/SystemRDL/systemrdl-compiler)
  - [Open Register Design Tool](https://github.com/Juniper/open-register-design-tool).

There are lighter-weight options as well:

  - [RgGen](https://github.com/rggen/rggen)

This project would support a TL-Verilog output target, including Visual Debug (VIZ). The hardware output could simply be
TL-Verilog wrappers around the Verilog output, or it could be custom TL-Verilog. More interesting, though, is the
VIZ output, and it might be best for this to support the least-common-denominator Verilog output. With this,
any design using SystemRDL gets "live documentation" of it's CSRs containing CSR values from simulation in the context
of the hardware that uses them.

**Required skills**
  - SystemRDL
  - JavaScript and VIZ
  - Basic TL-Verilog


### Visualization of SweRV

The SweRV core is an open-source SystemVerilog RISC-V CPU core developed by Western Digital. It is an interesting core for college course and is being highlighted in the [RVfpga course](https://www.imgtec.com/news/press-release/imagination-announces-the-first-risc-v-computer-architecture-course/) for one. Visualizing the operation of the core can greatly enhance the learning experience. This project aims to do so.

**Status**: SweRV has been built and simulated within Makerchip in [this repo](https://github.com/stevehoover/SweRV_VIZ).

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
  - [M5](https://github.com/rweda/M5)


## Virtual FPGA Lab

![virtual lab](https://user-images.githubusercontent.com/64545984/130665673-63e52c11-f5e4-4290-8d05-a5a0741fbbbd.png)

1st CLaaS and Makerchip are great online tools to enable virtual FPGA lab classes. This project provides lab resources that mimic the physical lab experience to provide an easy path for migration of physical lab classes.

This project uses VIZ to represent the FPGA board, matching the spec of ones commonly used in labs, with LEDs, 7-segment displays, and/or video monitors. The experience will be enhanced by additional support in Makerchip for a VCD (waveform) streaming interface for 1st CLaaS (where each time-step is a 1st CLaaS chunk plus a timestamp). Shell logic will provide a shim between FPGA kernel logic as spec'ed for the virtualized FPGA and the 1st CLaaS interface.

Possible enhancements:
  - Support for additional FPGA boards can be added.
  - Course content can be enhanced.
  - An integration with [F4PGA](https://f4pga.org/) and/or [Apio](https://github.com/FPGAwars/apio) may makes sense.

**Repo**: https://github.com/os-fpga/Virtual-FPGA-Lab

**Status**: Developed as a Google Summer of Code 2021 project [here](https://github.com/BalaDhinesh/Virtual-FPGA-Lab), written up in this [blog](https://medium.com/@m.baladhinesh/fpgas-in-your-browser-bb92be1c1fa3), and used in this [free course](https://github.com/stevehoover/GettingStartedWithFPGAs).

**Required skills** (for multiple participants)
  - JavaScript and VIZ
  - TL-Verilog
  - 1st CLaaS

**Discussion**: [TL-Verilog User's Slack workspace](https://join.slack.com/t/tl-verilog-users/shared_invite/zt-4fatipnr-dmDgkbzrCe0ZRLOOVm89gA) `#virtual-fpga-lab` channel.


## TL-Verilog Support in Edalize

[Edalize](https://github.com/olofk/edalize) automates EDA build flows, and wouldn't it be great to have TL-Verilog support using [SandPiper-SaaS](https://pypi.org/project/sandpiper-saas/).

**Status**: Done, mergeed from this [pull request](https://github.com/shariethernet/edalize/tree/sandpiper), and here's a [usage example](https://github.com/shariethernet/edalize_sandpiper_example).


## Tutorial/Gamification Content Creation

There are many opportunities to provide fun tutorials and gamified learning content for TL-Verilog that could be incorporated into Makerchip.

**Status**: Grant application with TUe and U. Wisc. under consideration.

**Required skills**
  - TL-Verilog
  - Makerchip
  - VIZ
  - Web development (JavaScript, HTML, CSS, React(?), npm)


## WARP-V Configurator

![warp-v_org](https://user-images.githubusercontent.com/11302288/218320194-a705f143-ab50-4aac-8d29-1128e3eb101d.png)

This project adds a web front-end to WARP-V for configuration. The configured WARP-V core (or many-core) can be opened in Makerchip. This project is sketched out in a [WARP-V repo wiki page](https://github.com/stevehoover/warp-v/wiki/WARP-V-Configuration-Front-End)

**Status**: Launched! (http://warp-v.org)

**Required skills**
  - TL-Verilog
  - M4
  - Web development (JavaScript, HTML, CSS, React(?), NodeJS/npm)

**Discussion**: [TL-Verilog User's Slack workspace](https://join.slack.com/t/tl-verilog-users/shared_invite/zt-4fatipnr-dmDgkbzrCe0ZRLOOVm89gA) `#warp-v-configurator` channel.

## Connect Compiler Explorer with WARP-V

Compiler Explorer is an open-source online tool that allows a user to explore how compilers turn source code in various languages into assembly code.

WARP-V is an open-source CPU core generator that can be configured, then loaded, simulated, and edited online. Custom
assembly code can be provided for simulation.

By combining Compiler Explorer with WARP-V we would have a full online experimentation platform to go from high-level
software to circuit simulation of the program in a customized CPU core.

**Required Skills**
  - Node.js and general web dev.
  - [M5](https://github.com/rweda/M5) in order to bring the WARP-V assembler to full compliance (which could be left for someone else).

## WARP-V Many-core Accelerator Microservice

This project brings together three others:
  - [WARP-V](https://github.com/stevehoover/warp-v)
  - [TL-Verilog FLow Library](https://github.com/stevehoover/tlv_flow_lib)
  - [1st ClaaS](https://github.com/os-fpga/1st-CLaaS)
It will provide a configurable, easily-modifiable many-core-on-FPGA hardware accelerator deployed as a microservice to accelerate web and cloud applications.

Development from Google Summer of Code 2021 is merged into the [WARP-V repo](https://github.com/stevehoover/warp-v). Student: Vineet Jain. Primary Mentor: Akos Hadnagy. [Blog](https://medium.com/@vineetajm1999/developing-applications-for-cloud-fpgas-are-easier-than-you-think-6b39b7010412).

**Status**: Google Summer of Code 2021 project. Constructed in simulation, running simple assembly tests. One known bug.

**Required skills** (for multiple participants)
  - TL-Verilog
  - Many-core CPU microarchitecture
  - 1st CLaaS
  - Xilinx FPGA development

**Discussion**: [TL-Verilog User's Slack workspace](https://join.slack.com/t/tl-verilog-users/shared_invite/zt-4fatipnr-dmDgkbzrCe0ZRLOOVm89gA) `#warp-v-manycore` channel.


## Implementing other ISAs in WARP-V 

WARP-V currently has support for RISC-V, (incomplete) MIPS, and a toy educational ISA. PowerPC is also open now and could be implemented. Apparently, there are several open-source, out of patent versions of Arm1 on github. And any other open ISAs can be implemented.


## Neural Net

Vineet Jain created a simple <a href="https://github.com/vineetjain07/DNN_TL-V">configurable neural network model in TL-Verilog</a>. This could follow a similar path to WARP-V w/ a configurator and cloud FPGA implementation. The WARP-V configurator is build in a modular fashion to support this easily.

**Required skills**
  - Web development (JavaScript, HTML, CSS, React, NodeJS, etc.)
  - TL-Verilog
  - M4


## TensorCore Accelerator for Machine Learning

This was a Google Summer of Code 2021 project.

![TensorCore](https://user-images.githubusercontent.com/11302288/134257557-0132a79d-da4c-4435-b952-7a9cda1537b3.png)

**Status**: Nitin Mishra began this project in Google Summer of Code 2021, mentored by Theodore Omtzigt. More in [the repo](https://github.com/natu4u/GSOC_TensorCore) and this [blog post](https://medium.com/@nmishra9/tensorcore-extension-for-deep-learning-41728fc22495). Theo has since gone on to found [Lemurian Labs](https://www.lemurianlabs.com/) and was last seen hiring TL-Verilog developers.


## FractalValley

![fractalvalley](https://user-images.githubusercontent.com/11302288/134257481-e43618a9-a3de-4623-9c6d-75a1b009c076.png)

[FractalValley.net](http://www.fractalvalley.net) is a fun demo of 1st CLaaS and TL-Verilog. This project turns the demo into a robust site showcasing the value of hardware-acceleration in the cloud and the fun world of fractals.

**Required skills**
  - Web development (JavaScript, HTML, CSS, React, NodeJS, etc.)


## TL-Verilog Editor Modes

![TLX_code](https://user-images.githubusercontent.com/11302288/134257374-6fa3667f-e160-494e-92ee-e47f0ab6a394.png)

This general category of smaller projects improves the ecosystem for TL-Veriog development by creating editor support for various text editors and IDEs. Many editor modes already exist. A few possibilities include:
  - Tree-sitter support. This seems to currently have the strongest momentum across editors. It is used by Atom. There is a conversion flow for CodeMirror 6. VSCode does not currently support it, but this is likely coming soon.
  - Adding JavaScript and/or M5 editing support within the TL-Verilog mode for Code Mirror (used by Makerchip) for `\viz` blocks and `\m5` regions.
  - GitHub support for TL-Verilog (DONE, but awaiting acceptance)


## TL-Blockly

![TL-Blockly](https://raw.githubusercontent.com/ninja3011/Block_Based_Circuit_Design/1802073c6e71c49b56cf544a3d3c5c6db43d926a/assets/Pythagorean.gif)

[Blockly](https://developers.google.com/blockly) is a framework for creating drag-and-drop block-based programming environments that are especially great for kids. It looks like it would be fairly straight-forward to create a block-based TL-Verilog edito that could be incorporated into Makerchip.

**Status**: Google Summer of Code 2021 project, Ninad Jangle. [blog](https://ninja3011.github.io/Block_Based_Circuit_Design/) [repo](https://github.com/ninja3011/Block_Based_Circuit_Design), [application](https://gsoc-block-based-circuit-design-site.netlify.app/)

**Discussion**: [TL-Verilog User's Slack workspace](https://join.slack.com/t/tl-verilog-users/shared_invite/zt-4fatipnr-dmDgkbzrCe0ZRLOOVm89gA) `#blockly` channel.


## EDA Microservices
  
Makerchip currently supports simulation of Verilog and TL-Verilog code. It is expanding to support logic synthesis and other physical flows as well as support for other HDLs. This project will provide various microservices that run open-source EDA tools that can be incorporated into Makerchip.
  
**Required skills**
  - Open-source EDA
  - Cloud development
  - Docker


## TL-Verilog Timing Reports

This project will help designers to relate timing information from synthesis tools back to TL-Verilog's higher-level context (hierarchy, pipelines, and transactions). Scripts are needed to map RTL signal names to their original TL-Verilog names. This will be applied to timing reports from open source synthesis tools so timing information can be reported with respect to TL-Verilog source code.

