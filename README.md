# About this Repo

This repo is a starting-point for folks interested in getting involved in TL-Verilog projects.

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

  - Find an IP on [Open Cores](https://opencores.org/) and convert to TL-Verilog
  - Ramp up on [1st CLaaS](https://github.com/stevehoover/1st-CLaaS) and create a simple hardware kernel that can be executed from a web application. You'll find a few simple demo applications in this repository that you can reference as examples.


# Project Repos

Here are a few noteworthy TL-Verilog project repositories:
  - [1st ClaaS](https://github.com/stevehoover/1st-CLaaS): A framework for developing hardware accelerated web and cloud applications using cloud FPGAs.
  - RISC-V:
    - [MYTH Workshop](https://github.com/stevehoover/RISC-V_MYTH_Workshop): A workshop offered by Redwood EDA and VLSI System Design. The repo indexes a few [CPU cores developed by students of the workshop](https://github.com/stevehoover/RISC-V_MYTH_Workshop/blob/master/student_projects.md) which serve as a good reference for RISC-V using TL-Verilog.
    - [WARP-V](https://github.com/stevehoover/warp-v): A CPU core generator that makes heavy use of M4 macro preprocessing and the flexibility of TL-Verilog to support different ISAs, pipeline depths, etc.
  - ...
