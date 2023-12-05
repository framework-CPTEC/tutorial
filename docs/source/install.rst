Instalação
==========

- Criar ambiente conda

.. code-block:: console

  conda create -n cptec python=3.10

  conda activate cptec

**Via pip**
  
.. code-block:: console

  pip install cptec-model
  
**Via fonte**

- Instalar Pacotes Requeridos

.. code-block:: console

  conda install -c conda-forge matplotlib pycurl cfgrib netCDF4 pynio xarray dask esmpy scipy mpi4py xesmf ipykernel

- Instalar Pacote cptec-model

.. code-block:: console
 
  git clone https://github.com/framework-CPTEC/CPTEC-user.git

  cd CPTEC-user

  python setup.py install


