---
layout: page
title: LARS&#58; a 2D Stokes flow solver
description: An algorithm to compute 2D Stokes flows with great speed and accuracy
img: assets/img/publication_preview/heart_closeup.png
importance: 2
# category:
related_publications: false
---

At Oxford Maths, we developed a 2D Stokes flow solver LARS (Lightning-AAA Rational Stokes) using rational approximation. It uses the lightning algorithm for sharp corners (Gopal and Trefethen, 2019; Brubeck and Trefethen, 2022), the AAA algorithm for curved boundaries (Nakatsukasa et al., 2018), and a series method (Trefethen, 2018) for multiply connected domains. The solver works for most 2D Stokes problems with different geometries and boundary conditions. In most cases, a solution can be obtained to 6-digit accuracy in less than 1 second on a laptop. Example MATLAB codes can be found on <a href="https://github.com/YidanXue/LARS">GitHub</a>.