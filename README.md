install-jenkins
=========

Role do Ansible para instalação de um servidor Jenkins.

Distribuições Suportadas pela Role
------------

- Debian
- RedHat ou CentOS

Tags da Role 
--------------

- deps: Instala as dependências do Jenkins.
- repo: Insere o repositório do Jenkins.
- jenkins: Realiza a instalação do pacote do Jenkins.

Variáveis da Role 
--------------


Examplos de Playbook
----------------

Exemplo de uso da Role:

    - hosts: servers
      roles:
         - install-jenkins

License
-------

BSD
