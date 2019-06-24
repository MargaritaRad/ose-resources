===============
StructResources
===============


Here we list resources for students or researchers who want to start to solve and estimate structural economic models. Due to our background we focus mainly on microeconomic applications but also try to include a few resources for macroeconomic models. If you know another good tutorial or python package for structural econometrics, please let us know, so we can add it. If you are the author of one of the packages or tutorials we list, and think our description is outdated or not accurate, please open an issue or submit a pull request.



`QuantEcon <https://lectures.quantecon.org/>`_
==============================================

`QuantEcon <https://lectures.quantecon.org/py/>`_ is an initiative by `Thomas J. Sargent <http://www.tomsargent.com/>`_ and `John Stachurski <http://johnstachurski.net/>`_. It is very well suited for inexperienced programmers. Besides explaining some components of structural models in detailed and simple to follow tutorials, it also teaches the basics of Python and Julia.


The most notable links you should check out are:


`Introduction to Python <https://lectures.quantecon.org/py/index_learning_python.html>`_
----------------------------------------------------------------------------------------

This will guide you through the set-up of Python on your computer, explain the basic syntax and data structures. It is quite fast paced but self-contained.


`Scientific Python Libraries <https://lectures.quantecon.org/py/index_python_scientific_libraries.html>`_
---------------------------------------------------------------------------------------------------------

The core Python language is not designed for scientific computing. Instead, this is delegated to other packages. Here you will get an overview of the main Python packages you will need:

- Numpy: provides multi-dimensional arrays and functions to work on them.
- Matplotlib: simple plotting in Python. While it is good to understand the basics of matplotlib, we would suggest that users use the much simpler `seaborn library <https://seaborn.pydata.org/>`_ that builds on top of matplotlib and produces beautiful graphs out of the box
- Scipy: Toolkit for scientific computing. Examples are optimization, numerical integration and random number generation.
- Numba: A just in time compiler for Python that can make Python about as fast as Fortran or C. Seriously, try it out. It's amazing!



`Dynamic Programming <https://lectures.quantecon.org/py/index_dynamic_programming.html>`_
-----------------------------------------------------------------------------------------


A great introduction into the theory and implementation of simple dynamic programming models.



`OpenSourceEconomics <https://github.com/OpenSourceEconomics>`_
==============================================================

`OpenSourceEconomics <https://github.com/OpenSourceEconomics>`_ was started by `Philipp Eisenhauer <https://peisenha.github.io/build/html/index.html>`_ in 2018. It is a collection of model packages and tool packages. All code is unit tested and can be installed with pip or conda. The model packages are mainly targeted at advanced users who want to estimate large structural models. The tool packages have a wider user base.


Model Packages
--------------

`respy <https://github.com/OpenSourceEconomics/respy>`_
*******************************************************

respy is an open-source Python package for the simulation and estimation of a prototypical finite-horizon discrete choice dynamic programming model. It covers a range of models typically used in structural labor economics. Among the most notable examples are the models presented in:

    Keane, M. P. and Wolpin, K. I. (1994). `The Career Decisions of Young Men <https://www.jstor.org/stable/10.1086/262080>`_. *Journal of Political Economy*, 105(3): 473-522.

    Keane, M. P. and  Wolpin, K. I. (1994). `The Solution and Estimation of Discrete
    Choice Dynamic Programming Models by Simulation and Interpolation: Monte Carlo
    Evidence <https://doi.org/10.2307/2109768>`_. *The Review of Economics and
    Statistics*, 76(4): 648-672.

If you are interested in using respy for your own work, check out the comprehensive `online documentation <https://respy.readthedocs.io/en/latest/>`_

`grmpy <https://github.com/OpenSourceEconomics/grmpy>`_
*******************************************************

grmpy is an open-source package for the simulation and estimation of the generalized Roy model. It serves as a teaching tool to promote the conceptual framework of the generalized Roy model, illustrate a variety of issues in the econometrics of policy evaluation, and showcase basic software engineering practices.

If you are interested in using respy for your own work, check out the `online documentation <https://grmpy.readthedocs.io/en/latest/>`_


`ruspy <https://github.com/OpenSourceEconomics/ruspy>`_
*******************************************************

ruspy is a Python package that builds on John Rust's seminal Paper on the optimal replacement of bus engines:


    Rust, J. (1987). `Optimal Replacement of GMC Bus Engines: an Empirical Model of Harold Zurcher <https://www.jstor.org/stable/1911259>`_ Econometrica, Vol. 55, No.5, 999-1033.

It is currently extended to allow for robust decision making under ambiguity.


Tool Packages
-------------

`estimagic <https://github.com/OpenSourceEconomics/estimagic>`_
***************************************************************


Estimagic is a Python package that helps to build high-quality and user friendly implementations of (structural) econometric models.

It is designed with large structural models in mind. However, it is also useful for any other estimator that numerically minimizes or maximizes a criterion function (Extremum Estimator). Examples are maximum likelihood estimation, generalized method of moments, method of simulated moments and indirect inference.

Currently we mainly provide a large collection of numerical optimizers. For example we wrap the optimizers from `PYGMO <https://esa.github.io/pagmo2/>`_ and `Scipy <https://docs.scipy.org/doc/scipy/reference/optimize.html>`_ and are working on the support for optimizers from the `Toolkit for Advanced Optimization <https://www.mcs.anl.gov/petsc/petsc-current/docs/manualpages/Tao/>`_


The main advantage of using those optimizers via estimagic are:

- A unified interface
- The optimize work with parameters in the form of a pandas Series or DataFrame whereas other optimizers simply have the parameters in a numpy array or similar container. This leads to much more readable code since parameters can be accessed by label and not by position
- Unified specification of constraints typical in structural models (e.g. a set of parameters has to form a valid covariance matrix, lower and upper bounds, increasing parameters, ...)
- An interactive dashboard with live convergence plots.

Estimagic is in a very early stage and should not be used for major projects yet. However, we do encourage interested users to try it out, report bugs and provide feedback.

If you are interested, check out the `online documentation <https://estimagic.readthedocs.io/en/latest/>`_


`Econ-ARK <https://econ-ark.org/>`_
===================================


The `Econ-ARK <https://econ-ark.org/>`_ project provides open-source toolkits for researchers trying to understand how economic and social outcomes result from the actions of heterogeneous individuals.

The primary goals of the project are:

- to make entry into the world of such modeling easy
- to accelerate the development of this kind of modeling for policy-making and academic research
- to increase the openness, replicability, and interoperability of modeling tools.

Econ-Ark is headed by Christopher D. Carroll, Professor of Economics at the Johns Hopkins University.

Originally, Econ-ARK was mainly targeted at macroeconomic applications, but is now extending their tools to support typical microeconomic models.

The main features of Econ-ARK are:

`HARK <https://github.com/econ-ark/HARK>`_
------------------------------------------

The `Heterogeneous Agents Resources and Toolkit (HARK) <https://github.com/econ-ark/HARK>`_ is motivated by a sense that quantitative structural modeling of economic agents' behavior (consumers; firms), at present, is roughly like econometric modeling in the 1960s: Lots of theoretical results are available and a great deal can be done in principle, but actually using such tools for any specific research question requires an enormous investment of a scholar's time and attention to learn techniques that are fundamentally not related to economics but instead are algorithmic/computational (in the 1960s, e.g., inverting matrices; now, e.g., solving dynamic stochastic optimization problems). The toolkit is built using the suite of open source, transparent tools for collaborative software development that have become ubiquitous in other fields in the last few years: Github, object-oriented coding, and methods that make it much easier to produce plug-and-play software modules that can be (relatively) easily combined, enhanced and adapted to address new problems.


`REMARK <https://github.com/econ-ark/REMARK>`_
----------------------------------------------

This is the resting place for self-contained and complete projects written using the Econ-ARK. The content here should be executable by anyone with a suitably configured computer (see "Installation.md" in this directory).

Each project lives in its own subdirectory in the REMARKs directory

Types of content include (see below for elaboration):

- Explorations: Use the Econ-ARK/HARK toolkit to demonstrate some set of modeling ideas
- Replications: Attempts to replicate the results of published papers written using other tools
- Reproductions: Code that reproduces the results of some paper that was originally written using the toolkit
