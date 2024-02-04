.. _installation_instruction:


Installation
============

Pre-build binaries
------------------

The Python package can be installed with Pypi:

.. code-block:: bash

    pip install HieTaSumm


Supported systems:

 - Python 3.5, 3.6, 3.7, 3.8
 - Linux 64 bits, macOS, Windows 64 bits

With setuptools
***************

The file ``setup.py`` is a thin wrapper around the cmake script.
The following commands will download the library, create a binary wheel and install it with *pip*.


.. code-block:: bash

    git clone link-para-github
    cd HieTaSum
    python setup.py
