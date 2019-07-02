OpenSourceEconomics
===================

`OpenSourceEconomics <https://github.com/OpenSourceEconomics>`_ was founded in 2018 at the University of Bonn as a platform for discussion between students and academic researchers on issues regarding scientific programming. Apart from providing participants with an opportunity to present on and inform themselves about different software solutions during `monthly meetings <https://github.com/OpenSourceEconomics/hackathon>`_, the organization also offers a collection of open-source model and tool packages. All code is unit tested and can be installed with pip or conda. The model packages are mainly targeted at advanced users who want to estimate large structural models.

The following list provides an overview of the flagship projects:

Model Packages
--------------

`respy <https://github.com/OpenSourceEconomics/respy>`_
*******************************************************

respy is an open-source Python package for the simulation and estimation of a prototypical finite-horizon discrete choice dynamic programming model. It covers a range of models typically used in structural labor economics. Among the most notable examples are the models presented in `Keane and Wolpin (1994, 1997) <file:///home/sebastian/Desktop/team_meeting/struct-resources/docs/build/html/bibliography.html>`_.

If you are interested in using respy for your own work, check out the comprehensive `online documentation <https://respy.readthedocs.io/en/latest/>`_


`grmpy <https://github.com/OpenSourceEconomics/grmpy>`_
********************************************************

grmpy is an open-source package for the simulation and estimation of the generalized Roy model. It serves as a teaching tool to promote the conceptual framework of the generalized Roy model, illustrate a variety of issues in the econometrics of policy evaluation, and showcase basic software engineering practices. The developers build mainly on scientific contributions by `Abbring and Heckman (2007) <file:///home/sebastian/Desktop/team_meeting/struct-resources/docs/build/html/bibliography.html>`_ and `Heckman and Vytlacil (2007a, 2007b) <file:///home/sebastian/Desktop/team_meeting/struct-resources/docs/build/html/bibliography.html>`_.

If you are interested in using grmpy for your own work, check out the `online documentation <https://grmpy.readthedocs.io/en/latest/>`_


`soepy <https://github.com/OpenSourceEconomics/soepy>`_
*******************************************************

soepy is an open-source Python package for the simulation and estimation of a dynamic model of human capital accumulation tailored to the German Socio-Economic Panel (SOEP). It is based on the seminal paper by `Blundell, Dias, Meghir and Shaw. (2016) <file:///home/sebastian/Desktop/team_meeting/struct-resources/docs/build/html/bibliography.html>`_.

If you are interested in using soepy for your own work, check out the `online repository <https://github.com/OpenSourceEconomics/soepy>`_


Tool Packages
-------------

`estimagic <https://github.com/OpenSourceEconomics/estimagic>`_
***************************************************************

estimagic is a Python package that helps to build high-quality and user friendly implementations of (structural) econometric models.

It is designed with large structural models in mind. However, it is also useful for any other estimator that numerically minimizes or maximizes a criterion function (Extremum Estimator). Examples are maximum likelihood estimation, generalized method of moments, method of simulated moments and indirect inference. It is in a very early stage and should not be used for major projects yet. However, we do encourage interested users to try it out, report bugs and provide feedback.

If you are interested, check out the `online documentation <https://estimagic.readthedocs.io/en/latest/>`_
