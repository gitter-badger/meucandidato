Meu Candidato
=============

.. image:: https://travis-ci.org/gilsondev/meucandidato.svg?branch=master
   :target: https://travis-ci.org/gilsondev/meucandidato
   :alt: Travis-CI build status


.. image:: https://coveralls.io/repos/github/gilsondev/meucandidato/badge.svg?branch=master
   :target: https://travis-ci.org/gilsondev/meucandidato
   https://coveralls.io/github/gilsondev/meucandidato?branch=master
   :alt: Coverage status


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

1. Faça o checkout do projeto::

   $ git clone https://github.com/gilsondev/meucandidato.git

2. Crie um ambiente virtualizado com virtualenv::

   $ cd meucandidato
   $ python3 -m venv .venv

3. Ative e instale as dependências::

   $ source .venv/bin/activate
   (.venv) $ pip install -r requirements.txt

4. Cria o arquivo `.env` baseado no `contrib/env.sample` no diretório de trabalho::

   $ cp -Rvf contrib/env.sample .env

4. Execute o servidor local::

   $ python manage.py runserver
