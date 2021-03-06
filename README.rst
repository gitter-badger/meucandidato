Meu Candidato
=============

.. image:: https://readthedocs.org/projects/meucandidato/badge/?version=latest
   :target: http://facefind.readthedocs.io/pt/latest/?badge=latest
   :alt: Documentation Status

.. image:: https://travis-ci.org/gilsondev/meucandidato.svg?branch=master
   :target: https://travis-ci.org/gilsondev/meucandidato
   :alt: Travis-CI build status


.. image:: https://coveralls.io/repos/github/gilsondev/meucandidato/badge.svg?branch=master
   :target: https://coveralls.io/github/gilsondev/meucandidato?branch=master
   :alt: Coverage status

.. image:: https://www.quantifiedcode.com/api/v1/project/d7900427efab4a648b1707032945046e/badge.svg
  :target: https://www.quantifiedcode.com/app/project/d7900427efab4a648b1707032945046e
  :alt: Code issues


Sistema voltado para centralizar informações do seu candidato, e tornar acessível para qualquer eleitor sobre sua vida, carreira e qualquer
notícia relacionado a ele e seu partido.



:License: GPLv3


Objetivo
--------

Essa idéia surgiu quando este idealizador (Gilson Filho) procurava informações de candidatos na última eleição. Como as informações estão em vários
lugares, como também dados do TSE não são tão acessíveis como deveria, pensei em uma forma de criar um aplicação web que possa pesquisar
pelo nome do candidato do seu interesse, e capturar tudo o que é possível dele em:

- Portais de notícias
- Dados do TSE como: credenciamento eleitoral, doações de campanha e seus gastos
- Dados processuais de tribunais do estado do candidato
- E outras informações acessíveis pela Internet

Dessa forma, teriamos nas nossas mãos uma linha do tempo de tudo que ele fez ou não fez, propôs, os partidos que passou e sua associação
a outros candidatos e políticos.

Instalação
----------

1. Faça o checkout do projeto:

.. code-block::

   $ git clone https://github.com/gilsondev/meucandidato.git

2. Crie um ambiente virtualizado com virtualenv:

.. code-block::

   $ cd meucandidato
   $ python3 -m venv .venv

3. Ative e instale as dependências:

.. code-block::

   $ source .venv/bin/activate
   (.venv) $ pip install -r requirements.txt

4. Cria o arquivo `.env` baseado no `contrib/env.sample` no diretório de trabalho:

.. code-block::

   $ cp -Rvf contrib/env.sample .env

5. Execute o servidor local:

.. code-block::

   $ python manage.py runserver


TODO
----

- Pesquisar notícias do candidato nos grandes portais (G1, R7, Folha, etc)
- Importar dados eleitorais do TSE (Dados do candidato, relação de bens)
- Importar dados de doações para candidatos
