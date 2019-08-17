install-jenkins
=========

Role do Ansible para instalação de um servidor Jenkins (com OpenJDK 8).

Distribuições Suportadas pela Role
------------

- Debian
- RedHat ou CentOS

Tags da Role 
--------------

- main: Tag a ser utilizada em conjunto com outras tags, se alguma tag for especificada no comando.
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

Exemplo de Comandos
----------------

Comando para executar todas as tasks:

    ansible-playbook -i <caminho_inventario> <caminho_playbook>

Comando para executar a tag "repo" (em caso de uso de tags, a tag "main" é obrigatória):

    ansible-playbook -i <caminho_inventario> <caminho_playbook> --tags "main, repo"
