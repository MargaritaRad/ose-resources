Econ-ARK
========

The `Econ-ARK <https://econ-ark.org/>`_ project provides open-source toolkits for researchers trying to understand how economic and social outcomes result from the actions of heterogeneous individuals.

The primary goals of the project are:

- to make entry into the world of such modeling easy
- to accelerate the development of this kind of modeling for policy-making and academic research
- to increase the openness, replicability, and interoperability of modeling tools.

Econ-Ark is headed by `Christopher D. Carroll <https://econ.jhu.edu/directory/christopher-carroll/>`_, Professor of Economics at the Johns Hopkins University.

Originally, ``econ-ark`` was mainly targeted at macroeconomic applications, but is now extending their tools to support typical microeconomic models.

The main features of Econ-ARK are:

HARK
----

``econ-ark``, the `Heterogeneous Agents Resources and Toolkit (HARK) <https://github.com/econ-ark/HARK>`_ is motivated by a sense that quantitative structural modeling of economic agents' behavior (consumers; firms), at present, is roughly like econometric modeling in the 1960s: Lots of theoretical results are available and a great deal can be done in principle, but actually using such tools for any specific research question requires an enormous investment of a scholar's time and attention to learn techniques that are fundamentally not related to economics but instead are algorithmic/computational (in the 1960s, e.g., inverting matrices; now, e.g., solving dynamic stochastic optimization problems). The toolkit is built using the suite of open source, transparent tools for collaborative software development that have become ubiquitous in other fields in the last few years: Github, object-oriented coding, and methods that make it much easier to produce plug-and-play software modules that can be (relatively) easily combined, enhanced and adapted to address new problems.

Check out the `online documentation <https://hark.readthedocs.io/en/latest/>`_.


REMARK
------

`This <https://github.com/econ-ark/REMARK>`_ is the resting place for self-contained and complete projects written using the Econ-ARK. The content here should be executable by anyone with a suitably configured computer (see "Installation.md" in this directory).

Types of content include (see below for elaboration):

- Explorations: Use the ``econ-ark``/HARK toolkit to demonstrate some set of modeling ideas
- Replications: Attempts to replicate the results of published papers written using other tools
- Reproductions: Code that reproduces the results of some paper that was originally written using the toolkit
