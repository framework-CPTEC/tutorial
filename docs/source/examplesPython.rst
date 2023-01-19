Exemplos Python
===============

.. warning::
  Alterar a data para os valores exibidos na inicialização

Recuperar Dados de Modelos Numéricos
------------------------------------
.. code-block:: console

  # Importa a ferramenta
  import CPTEC_BAM as BAM

  # Inicializa o construtor
  bam = BAM.model()

  # Data Condição Inicial (IC)
  date = '2022111800'

  # variaveis
  vars = ['t2m', 'u', 'omega']

  # Quantos passos previstos após inicialização do modelo
  steps = 5

  # Niveis desejados (aplicado apenas as variaveis em niveis)
  levels = [1000, 850]

  # Para ativar a função de escrita em disco com uma copia da resição basta alterar a função save_netcdf para True
  bam.dict['save_netcdf'] = True

  # # Diretorio onde serão salvas as requisições
  # # Por padrão, quando não aterado, um diretorio chamado INPE será criado na pasta corrente do usuario

  # bam.dict['path_to_save'] = '/home/framework/modelos'

  # Requisição dos dados
  f = bam.load(date=date, var=vars, level=levels, steps=steps)

  # Um diretorio BAM será criado no diretorio corrente, no caso apresentado os dados serão salvos em:
  # INPE/BAM/TQ0666L064/brutos/hibrido/2022/11/18/00/GPOSNMC20220818002022081906P.fct.TQ0666L064.nc4

  quit()

python get_data_oper.py

python get_netcdf.py

python plot_figure.py

Exemplos Jupyter Notebook
conda install -c anaconda ipykernel

pip install jupyter

jupyter notebook

Example_lib.ipynb

Example_lib_Widgets.ipynb

Example_lib_regrid.ipynb
