Installation
============

Dependencies
------------
pygen-structures depends upon the RDKit_ for molecule representations and numpy_
for representations of the adjacency matrix. Running the full set of tests
requires pytest_ and OpenMM_.

Installation Steps
------------------

There are other ways to install the required dependencies, but the easiest way
by far is to use conda_. Instructions, including the installation of test
dependencies, are outlined below. Alternatively, OpenMM and the RDKit can be
compiled from source; pytest and numpy can be installed using pip.

1. Install the conda_ package manager. Make sure the ``conda`` executable is in
   your PATH.

2. Set up a conda environment with the relevant dependencies (or install them
   in your base distribution). This can be done with the following command:

   .. code-block:: bash

       conda create -n pygen-structures -c rdkit -c omnia 'python>=3.6' 'rdkit>=2018.3' numpy 'openmm>=7.4' pytest

3. Activate the conda environment:

   .. code-block:: bash

       conda activate pygen-structures

4. Use ``pip`` to install pygen-structures in this environment:

   .. code-block:: bash

       pip install pygen-structures

5. Installation complete! You will have to activate this environment using
   ``conda activate pygen-structures`` each time you want to use it.

6. Test the installation:

   .. code-block:: bash

      pytest --pyargs pygen_structures


To install only the runtime dependencies, use the following command in step 2:

.. code-block:: bash

    conda create -n pygen-structures -c rdkit 'python>=3.6' 'rdkit>=2018.3' numpy

.. _RDKit: https://rdkit.org
.. _numpy: https://numpy.org
.. _pytest: https://docs.pytest.org
.. _conda: https://docs.conda.io/en/latest/
