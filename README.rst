MDSynthesis: a Python package enabling data-driven molecular dynamics research
==============================================================================

|zen|

This poster was presented at SciPy 2015 in Austin, TX, on July 8, 2015.

Authors
-------
David L. Dotson  /  david.dotson@asu.edu

Oliver Beckstein  /  oliver.beckstein@asu.edu

Abstract
----------------------------
Proteins are the molecular machines of life, and molecular dynamics (MD)
simulation permits atomically-detailed access to the interactions that define
their behavior. MD trajectories give a sequence of structural snapshots--a
timeseries of thousands to many millions of atom positions. With ever-faster
computational resources we can routinely generate many terabytes of data,
perhaps spread over hundreds of individual simulation trajectories. Often these
trajectories are not just repeats of the same simulation system, but instead
sample a wide range of different starting configurations, forcefield
parameters, protein conformations, mutations, protonation states, etc., which
can make data management difficult. Furthermore, because of their cost to
calculate, it is necessary to store intermediate data--often timeseries for
specific structural or thermodynamic quantities of interest. This adds to the
complexity of managing data, and serves as a barrier to answering scientific
questions. MDSynthesis, a Python package that handles the tedious and
time-consuming logistics of intermediate data storage and retrieval, is in
active development to address this problem. MDSynthesis features container
objects that use the robust MDAnalysis library for dissecting the details of
individual MD trajectories, and they store their states to disk on-the-fly
using the PyTables HDF5 interface. These containers are memory efficient and
built for aggregation, including convenience methods for quickly combining and
comparing datasets (pandas, numpy, or other pure python structures) across
hundreds of simulations in arbitrary ways. This makes data exploration feasible
with MD data, and the abstraction the containers provide make it easier to
write analysis code that works across many variants of a simulation system. The
package is actively developed and freely available under the GPLv2 from
https://github.com/Becksteinlab/MDSynthesis.

.. |zen| image:: https://zenodo.org/badge/doi/10.5281/zenodo.20385.svg
    :alt: Citation
    :target: http://dx.doi.org/10.5281/zenodo.20385

