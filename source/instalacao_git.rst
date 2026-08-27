
===========================================
Instalação e Configuração do Git
===========================================

Para versionar a documentação no padrão **Docs as Code** e realizar a publicação automática, é necessário ter o Git instalado no ambiente local.

Instalação Rápida via Terminal (winget)
=======================================
O Windows possui um gerenciador de pacotes nativo em linha de comando (Windows Package Manager). É a forma mais rápida e padronizada de instalar o Git sem precisar navegar até o navegador.

1. Abra o **PowerShell** ou o **Terminal do Windows**.
2. Cole e execute o comando abaixo:

.. code-block:: powershell

   winget install --id Git.Git -e --source winget

3. Aguarde o download e a finalização automática do instalador.

Confirmando a Instalação
========================
Após o término do processo no terminal, feche e reabra o terminal (ou o VS Code) para atualizar as variáveis de ambiente do sistema e execute:

.. code-block:: powershell

   git --version

Se o retorno indicar a versão (ex: ``git version 2.x.x``), a ferramenta está pronta para uso.

Configuração de Identidade
==========================
Antes de realizar o primeiro commit, registre a sua identidade global no Git rodando os comandos no terminal:

.. code-block:: powershell

   git config --global user.name "Seu Nome"
   git config --global user.email "seuemail@exemplo.com"