OpenSourceEconomics
===================

`OpenSourceEconomics <https://github.com/OpenSourceEconomics>`_ was started by `Philipp Eisenhauer <https://peisenha.github.io/build/html/index.html>`_ in 2018. It is a collection of model packages and tool packages. All code is unit tested and can be installed with pip or conda. The model packages are mainly targeted at advanced users who want to estimate large structural models. The tool packages have a wider user base

Model Packages
--------------

`respy <https://github.com/OpenSourceEconomics/respy>`_
*******************************************************

respy is an open-source Python package for the simulation and estimation of a prototypical finite-horizon discrete choice dynamic programming model. It covers a range of models typically used in structural labor economics. Among the most notable examples are the models presented in:

    Keane, M. P. and Wolpin, K. I. (1994). `The Career Decisions of Young Men. <https://www.jstor.org/stable/10.1086/262080>`_ Journal of Political Economy, 105(3): 473-522.

    Keane, M. P. and Wolpin, K. I. (1994). `The Solution and Estimation of Discrete Choice Dynamic Programming Models by Simulation and Interpolation: Monte Carlo Evidence. <https://doi.org/10.2307/2109768>`_ The Review of Economics and Statistics, 76(4): 648-672.

If you are interested in using respy for your own work, check out the comprehensive `online documentation <https://respy.readthedocs.io/en/latest/>`_


`grmpy <https://github.com/OpenSourceEconomics/grmpy>`_
********************************************************

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
