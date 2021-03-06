Installation
============

Installing with conda
-----------------------
SImMER is distributed through `conda-forge <https://conda-forge.org/>`_, and can be installed via conda. 
This is the recommended installation method. To do so, run

.. code-block:: bash

    conda config --add channels conda-forge
    conda install simmer

Installing with pip
-----------------------
SImMER is also distributed on `PyPI <https://pypi.org/>`_. It can be installed with

.. code-block:: bash

    pip install simmer

Installing from source
-----------------------

SImMER is developed on `GitHub <https://github.com/arjunsavel/simmer>`_. If you received the code as a tarball or zip, skip to below the :code:`git clone` line. It is recommended to run the below lines in a fresh `conda <https://docs.conda.io/projects/conda/en/latest/user-guide/concepts/environments.html>`_ environment.

.. code-block:: bash

    python3 -m pip install -U pip
    python3 -m pip install -U setuptools setuptools_scm pep517
    git clone https://github.com/arjunsavel/SImMER.git
    cd simmer
    python3 -m pip install -e .


Test the installation
---------------------

To ensure that the installation has been performed smoothly, feel free to run the unit and integration tests included with the package. The entire test suite should take on the order of 10 minutes to run. In the process, a few (~2) gigabytes of data will be downloaded from this project's associated Dropbox files; they'll be automatically deleted once the test suite is finished. 

From the :code:`simmer` directory, then run

.. code-block:: bash

    python3 -m unittest discover src
